# Matillion

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

Matillion is a data integration and transformation (ETL/ELT) company whose Data Productivity Cloud (DPC) lets teams build, orchestrate, and schedule data pipelines against cloud data warehouses. The DPC API is an OAuth2-secured REST control plane for projects, environments, pipeline executions, schedules, and Agents, while the legacy instance-hosted Matillion ETL API exposes groups, projects, versions, jobs, tasks, and schedules over HTTP Basic auth.

**Areas:** Data Integration · ETL · ELT · Data Pipeline · Cloud Data Warehouse

## Matillion on APIs.io

Everything profiled for Matillion is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/matillion/](https://apis.io/providers/matillion/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Matillion DPC Agents API](https://apis.io/apis/matillion/matillion-dpc-agents-api/) — Data Productivity Cloud Agents (hybrid runtime).
- [Matillion DPC Environments API](https://apis.io/apis/matillion/matillion-dpc-environments-api/) — Data Productivity Cloud environments (warehouse connection contexts).
- [Matillion DPC Pipeline Executions API](https://apis.io/apis/matillion/matillion-dpc-pipeline-executions-api/) — Launch, inspect, and cancel Data Productivity Cloud pipeline executions.
- [Matillion DPC Projects API](https://apis.io/apis/matillion/matillion-dpc-projects-api/) — Data Productivity Cloud projects.
- [Matillion DPC Schedules API](https://apis.io/apis/matillion/matillion-dpc-schedules-api/) — Data Productivity Cloud pipeline schedules.
- [Matillion ETL Groups & Projects API](https://apis.io/apis/matillion/matillion-etl-groups-projects-api/) — Legacy Matillion ETL groups, projects, and versions.
- [Matillion ETL Jobs & Runs API](https://apis.io/apis/matillion/matillion-etl-jobs-runs-api/) — Legacy Matillion ETL job execution and validation.
- [Matillion ETL Schedules API](https://apis.io/apis/matillion/matillion-etl-schedules-api/) — Legacy Matillion ETL schedules.
- [Matillion ETL Tasks API](https://apis.io/apis/matillion/matillion-etl-tasks-api/) — Legacy Matillion ETL task monitoring and control.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Matillion Agentic Access](https://apis.io/agentic-access/matillion/matillion-agentic-access/)

#### JSON Schema (20)

The data models the API reads and writes.

- [Agent](https://apis.io/schemas/matillion/matillion-agent/)
- [AgentCreate](https://apis.io/schemas/matillion/matillion-agent-create/)
- [AgentCredentials](https://apis.io/schemas/matillion/matillion-agent-credentials/)
- [AgentList](https://apis.io/schemas/matillion/matillion-agent-list/)
- [Environment](https://apis.io/schemas/matillion/matillion-environment/)
- [EnvironmentCreate](https://apis.io/schemas/matillion/matillion-environment-create/)
- [EnvironmentList](https://apis.io/schemas/matillion/matillion-environment-list/)
- [EtlJobRunRequest](https://apis.io/schemas/matillion/matillion-etl-job-run-request/)
- [EtlJobRunResponse](https://apis.io/schemas/matillion/matillion-etl-job-run-response/)
- [PipelineExecution](https://apis.io/schemas/matillion/matillion-pipeline-execution/)
- [PipelineExecutionList](https://apis.io/schemas/matillion/matillion-pipeline-execution-list/)
- [PipelineExecutionRequest](https://apis.io/schemas/matillion/matillion-pipeline-execution-request/)
- [PipelineExecutionStatus](https://apis.io/schemas/matillion/matillion-pipeline-execution-status/)
- [PipelineExecutionSteps](https://apis.io/schemas/matillion/matillion-pipeline-execution-steps/)
- [Project](https://apis.io/schemas/matillion/matillion-project/)
- [ProjectCreate](https://apis.io/schemas/matillion/matillion-project-create/)
- [ProjectList](https://apis.io/schemas/matillion/matillion-project-list/)
- [Schedule](https://apis.io/schemas/matillion/matillion-schedule/)
- [ScheduleCreate](https://apis.io/schemas/matillion/matillion-schedule-create/)
- [ScheduleList](https://apis.io/schemas/matillion/matillion-schedule-list/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Matillion Context](https://apis.io/jsonld/matillion/matillion-context/)

#### Collections (10)

Postman and Open Collection request collections.

- [Matillion API](https://apis.io/collections/matillion/open-matillion/)
- [Matillion DPC Agents API](https://apis.io/collections/matillion/open-matillion-dpc-agents-api/)
- [Matillion DPC Agents DPC Environments API](https://apis.io/collections/matillion/open-matillion-dpc-environments-api/)
- [Matillion DPC Agents DPC Pipeline Executions API](https://apis.io/collections/matillion/open-matillion-dpc-pipeline-executions-api/)
- [Matillion DPC Agents DPC Projects API](https://apis.io/collections/matillion/open-matillion-dpc-projects-api/)
- [Matillion DPC Agents DPC Schedules API](https://apis.io/collections/matillion/open-matillion-dpc-schedules-api/)
- [Matillion DPC Agents ETL Groups & Projects API](https://apis.io/collections/matillion/open-matillion-etl-groups-projects-api/)
- [Matillion DPC Agents ETL Jobs & Runs API](https://apis.io/collections/matillion/open-matillion-etl-jobs-runs-api/)
- [Matillion DPC Agents ETL Schedules API](https://apis.io/collections/matillion/open-matillion-etl-schedules-api/)
- [Matillion DPC Agents ETL Tasks API](https://apis.io/collections/matillion/open-matillion-etl-tasks-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Matillion API Rules](https://apis.io/rules/matillion/matillion-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Matillion Authentication](https://apis.io/security/matillion/matillion-authentication/)
- [Matillion Domain Security](https://apis.io/security/matillion/matillion-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Matillion Scopes](https://apis.io/scopes/matillion/matillion-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Matillion Plans Pricing](https://apis.io/plans/matillion/matillion-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Matillion Rate Limits](https://apis.io/rate-limits/matillion/matillion-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Matillion Finops](https://apis.io/finops/matillion/matillion-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.matillion.com)
- [Documentation](https://docs.matillion.com)
- [Getting started](https://docs.matillion.com/data-productivity-cloud/cdc/docs/cdc-getting-started/)
- [Pricing](https://www.matillion.com/pricing)
- [Support](https://support.matillion.com/s/)
- [Changelog](https://roadmap.matillion.com/changelog)
- [Blog](https://www.matillion.com/blog)
- [Security](https://www.matillion.com/security)
- [Trust centre](https://www.matillion.com/trust-center)
- [Privacy policy](https://www.matillion.com/privacy/)
- [GitHub](https://github.com/matillion)
- [Status](https://status.matillion.com/)

## API Evangelist rating

**Kin Score 47.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 69.6 |
| Contract quality | 53.0 |
| Contract governance | 19.7 |
| Operational transparency | 52.6 |
| Developer ergonomics | 42.3 |
| Access clarity | 36.8 |

**Agent readiness 33.4** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/matillion/](https://apis.io/providers/matillion/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Matillion: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/matillion/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
