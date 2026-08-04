# Matillion (matillion)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Matillion is a data integration and transformation (ETL/ELT) company whose Data Productivity Cloud (DPC) lets teams build, orchestrate, and schedule data pipelines against cloud data warehouses. The DPC API is an OAuth2-secured REST control plane for projects, environments, pipeline executions, schedules, and Agents, while the legacy instance-hosted Matillion ETL API exposes groups, projects, versions, jobs, tasks, and schedules over HTTP Basic auth.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/apis.yml)

> **State note (2026):** The Data Productivity Cloud API documentation was rebranded to [docs.maia.ai](https://docs.maia.ai) ("Maia"). The runtime hosts are unchanged — the DPC control plane is still served from `eu1.api.matillion.com/dpc` and `us1.api.matillion.com/dpc`, the OAuth2 token endpoint is still `id.core.matillion.com/oauth/dpc/token` (audience `https://api.matillion.com`), and the legacy Matillion ETL API is still served from the customer's own instance at `https://{instance}/rest/v1`.

## Tags

- Data Integration
- ETL
- ELT
- Data Pipelines
- Cloud Data Warehouse

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### DPC Projects

List, create, and delete Data Productivity Cloud projects via the regional DPC control plane (eu1.api.matillion.com/dpc or us1.api.matillion.com/dpc), secured with an OAuth2 client-credentials Bearer JWT. Branches are managed in the UI only and are not exposed as a public API.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://eu1.api.matillion.com/dpc`

#### Tags

- Projects
- Data Productivity Cloud
- Control Plane

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DPC Environments

List and create the environments (warehouse connection contexts) that belong to a Data Productivity Cloud project, on the OAuth2-secured DPC control plane.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://eu1.api.matillion.com/dpc`

#### Tags

- Environments
- Data Productivity Cloud
- Warehouse Connections

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DPC Pipeline Executions

Launch pipeline executions, list executions for a project, retrieve execution status and step detail, and cancel a running execution (PATCH status CANCELLED). Long-running execution is observed by polling the status endpoint, not by a push transport.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://eu1.api.matillion.com/dpc`

#### Tags

- Pipeline Executions
- Data Productivity Cloud
- Orchestration

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DPC Schedules

Create, list, read, update, and delete the schedules that trigger pipeline executions for a Data Productivity Cloud project, on the OAuth2-secured DPC control plane.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://eu1.api.matillion.com/dpc`

#### Tags

- Schedules
- Data Productivity Cloud
- Automation

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DPC Agents

List and register Data Productivity Cloud Agents (the hybrid/customer-hosted runtime that executes pipelines), retrieve an Agent, and read its credentials, on the OAuth2-secured DPC control plane.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://eu1.api.matillion.com/dpc`

#### Tags

- Agents
- Data Productivity Cloud
- Hybrid Runtime

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ETL Groups & Projects (legacy)

Manage groups, projects, and versions on the legacy instance-hosted Matillion ETL API (base `https://{instance}/rest/v1`, HTTP Basic auth) — list, read, export, import, create, and delete groups, projects, and version artifacts.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://{instance}/rest/v1`

#### Tags

- Groups
- Projects
- Matillion ETL
- Legacy

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ETL Jobs & Runs (legacy)

Run and validate orchestration/transformation jobs on the legacy instance-hosted Matillion ETL API (base `https://{instance}/rest/v1`, HTTP Basic auth); run accepts scalar and grid variables and returns a task id for polling.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://{instance}/rest/v1`

#### Tags

- Jobs
- Runs
- Matillion ETL
- Legacy

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ETL Tasks (legacy)

Monitor and control task execution on the legacy instance-hosted Matillion ETL API (base `https://{instance}/rest/v1`, HTTP Basic auth) — list running tasks, read a task by id, cancel a task, and page task history.

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://{instance}/rest/v1`

#### Tags

- Tasks
- Monitoring
- Matillion ETL
- Legacy

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ETL Schedules (legacy)

Read, export, import, update, and delete schedules on the legacy instance-hosted Matillion ETL API (base `https://{instance}/rest/v1`, HTTP Basic auth).

- **Human URL:** [https://docs.matillion.com](https://docs.matillion.com)
- **Base URL:** `https://{instance}/rest/v1`

#### Tags

- Schedules
- Automation
- Matillion ETL
- Legacy

#### Properties

- [Documentation](https://docs.matillion.com)
- [OpenAPI](openapi/matillion-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/matillion.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/matillion.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/matillion)
- [LinkedIn](https://www.linkedin.com/company/matillion)
- [Website](https://www.matillion.com)
- [Documentation](https://docs.matillion.com)
- [Plans](plans/matillion-plans-pricing.yml)
- [Rate Limits](rate-limits/matillion-rate-limits.yml)
- [Fin Ops](finops/matillion-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
