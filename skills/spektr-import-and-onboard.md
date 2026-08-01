---
name: Import a customer and start onboarding
description: Create a dataset, import a customer record, and launch a Spektr onboarding session for KYB/KYC.
api: openapi/spektr-openapi.yml
operations: [DataImportController_create_v1, DataImportController_update_v1, ActionTicketController_createOnboarding_v1, RecordController_fetchRecordByReference_v1]
---

# Import a customer and start onboarding

Use this flow to bring a customer into Spektr and kick off an onboarding process.

## Auth
Send `x-api-key: <your key>` on every request (generated in the developer dashboard). Use the environment host you need: `https://ingest.spektr.com` (live) or `https://sandbox-ingest.spektr.com` (sandbox).

## Steps
1. **Create a dataset schema** — `DataImportController_create_v1` (`POST /v1/data`). Define fields and their data types. Send an `idempotency-key` header (V4 UUID) so retries are safe. Capture the returned `datasetId`.
2. **Import the customer record** — `DataImportController_update_v1` (`PUT /v1/data/{datasetId}`). Include a unique `reference` so the record can be upserted and looked up later. If a field is a file, the response returns a presigned S3 URL — upload the file to it (expires in 1 hour). A duplicate `reference` returns **409 Conflict**.
3. **Start onboarding** — `ActionTicketController_createOnboarding_v1` (`POST /v1/public/actions/processId/{processId}/workspaceId/{workspaceId}`). Optionally prefill client data. The response returns a session `token`; direct the client to `https://actions.spektr.com/form?token={token}`.
4. **Resolve the spektrId later** — `RecordController_fetchRecordByReference_v1` (`GET /v1/record/reference/{reference}`) to fetch the record (and its `spektrId`) using your own reference.

## Rules
- Reuse the same `idempotency-key` on retries; a mismatched replay returns **422**, an in-flight duplicate returns **409**, and replays carry `idempotent-replayed: true`.
- `reference` must be a non-empty string, not `"root"`, unique per workspace.
- Errors are `{ message, errorCode }` JSON (see errors/spektr-problem-types.yml).
