---
name: Execute a process and monitor via webhooks
description: Run a Spektr compliance process over customer records and receive results via HMAC-signed webhooks.
api: openapi/spektr-openapi.yml
operations: [ExecutionController_executionV3_v3, RecordController_listOpenLoops_v1, RecordController_fetchRecord_v1, EventsController_import_v1]
---

# Execute a process and monitor via webhooks

Run a configured process (KYB/KYC, monitoring, risk, remediation) and consume its results.

## Auth
`x-api-key: <your key>` header on every request.

## Steps
1. **Execute a process** — `ExecutionController_executionV3_v3` (`POST /v3/execution`). Provide the `processId` (from the platform) and the target `spektrId`s and/or reference IDs. Enable token refresh on version mismatch to run the latest process version.
2. **Check pending runs** — `RecordController_listOpenLoops_v1` (`POST /v1/record/listOpenLoops`) to see which records still have pending process runs.
3. **Fetch results** — `RecordController_fetchRecord_v1` (`GET /v1/record/{spektrId}`) to read the processed record, its status, and outputs.
4. **Feed transaction events for monitoring** — `EventsController_import_v1` (`POST /v1/events`) to push `paymentMade` events for transaction monitoring.

## Webhooks (preferred over polling)
Register a webhook URL in Settings → Developer → Export settings. Spektr POSTs HMAC-signed batches (`{ "results": [ ... ] }`) for events like `PROCESS_RUN_END`, `ALERT_ESCALATED`, `CUSTOMER_STATUS_CHANGED`, and `CUSTOMER_TAG_ADDED`. Verify the HMAC signature with your per-workspace secret. Delivery is at-least-once with 3 retries at 1s intervals — dedupe on event `id`. See asyncapi/spektr-webhooks.yml.
