# Spektr

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Spektr is an AI-powered compliance automation platform for banks and fintechs, backed by Northzone and Seedcamp. It automates KYB and KYC onboarding, continuous customer monitoring, risk scoring, remediation, and transaction monitoring using configurable processes and a library of AI agents (KYB, document review, network/ownership discovery, address and license verification, source-of-funds, and false-positive reduction). The REST API (documented on ReadMe at spektr.readme.io, served from ingest.spektr.com) covers dataset and customer-record import, process execution and onboarding orchestration, event and transaction ingestion, workspace field definitions, and HMAC-signed webhooks. Authentication is via an x-api-key header, with idempotency-key support and Live/Sandbox/Test environments.

**Areas:** Company · Compliance · RegTech · KYB · KYC · Onboarding · Transaction Monitoring · Financial Services · Artificial Intelligence · Enterprise

## Spektr on APIs.io

Everything profiled for Spektr is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/spektr/](https://apis.io/providers/spektr/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Spektr Action API](https://apis.io/apis/spektr/spektr-action-api-api/) — The Action API API from Spektr — 1 operation(s) for action api.
- [Spektr Events API](https://apis.io/apis/spektr/spektr-events-api-api/) — The Events API API from Spektr — 1 operation(s) for events api.
- [Spektr Execution API](https://apis.io/apis/spektr/spektr-execution-api-api/) — The Execution API API from Spektr — 3 operation(s) for execution api.
- [Spektr Import API](https://apis.io/apis/spektr/spektr-import-api-api/) — The Import API API from Spektr — 2 operation(s) for import api.
- [Spektr Orchestration API](https://apis.io/apis/spektr/spektr-orchestration-api-api/) — The Orchestration API API from Spektr — 6 operation(s) for orchestration api.
- [Spektr Records API](https://apis.io/apis/spektr/spektr-records-api-api/) — The Records API API from Spektr — 9 operation(s) for records api.
- [Spektr Transaction Definitions API](https://apis.io/apis/spektr/spektr-transaction-definitions-api/) — The Transaction Definitions API from Spektr — 2 operation(s) for transaction definitions.
- [Spektr Transactions API](https://apis.io/apis/spektr/spektr-transactions-api/) — The Transactions API from Spektr — 1 operation(s) for transactions.
- [Spektr Workspace Fields API](https://apis.io/apis/spektr/spektr-workspace-fields-api-api/) — The Workspace Fields API API from Spektr — 2 operation(s) for workspace fields api.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Spektr Webhooks](https://apis.io/asyncapis/spektr/spektr-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [spektr](https://apis.io/servers/spektr/spektr/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Spektr Agentic Access](https://apis.io/agentic-access/spektr/spektr-agentic-access/)

#### Collections (9)

Postman and Open Collection request collections.

- [Spektr Action API API](https://apis.io/collections/spektr/open-spektr-action-api-api/)
- [Spektr Action API Events API API](https://apis.io/collections/spektr/open-spektr-events-api-api/)
- [Spektr Action API Execution API API](https://apis.io/collections/spektr/open-spektr-execution-api-api/)
- [Spektr Action API Import API API](https://apis.io/collections/spektr/open-spektr-import-api-api/)
- [Spektr Action API Orchestration API API](https://apis.io/collections/spektr/open-spektr-orchestration-api-api/)
- [Spektr Action API Records API API](https://apis.io/collections/spektr/open-spektr-records-api-api/)
- [Spektr Action API Transaction Definitions API](https://apis.io/collections/spektr/open-spektr-transaction-definitions-api/)
- [Spektr Action API Transactions API](https://apis.io/collections/spektr/open-spektr-transactions-api/)
- [Spektr Action API Workspace Fields API API](https://apis.io/collections/spektr/open-spektr-workspace-fields-api-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Spektr Openapi Overlay](https://apis.io/overlays/spektr/spektr-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Spektr Authentication](https://apis.io/security/spektr/spektr-authentication/)
- [Spektr Domain Security](https://apis.io/security/spektr/spektr-domain-security/)
- [Spektr Trust Center](https://apis.io/security/spektr/spektr-trust-center/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://spektr.com)
- [Documentation](https://spektr.readme.io/reference/welcome-to-spektr-api-documentation)
- [Getting started](https://spektr.readme.io/docs/getting-started)
- [API reference](https://spektr.readme.io/reference/welcome-to-spektr-api-documentation)
- [Support](https://www.spektr.com/talk-to-us)
- [Blog](https://www.spektr.com/blog)
- [Compliance](https://www.spektr.com/trust)
- [Terms of service](https://www.spektr.com/terms-of-service)
- [Privacy policy](https://www.spektr.com/privacy-policy)
- [Status](https://spektr.statuspage.io)

## API Evangelist rating

**Kin Score 50.8** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 58.7 |
| Contract governance | 18.2 |
| Operational transparency | 47.4 |
| Developer ergonomics | 54.2 |
| Access clarity | 36.8 |

**Agent readiness 39.6** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 27.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/spektr/](https://apis.io/providers/spektr/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Spektr: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/spektr/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
