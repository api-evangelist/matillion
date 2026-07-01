# Matillion (matillion)

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
