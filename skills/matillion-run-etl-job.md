---
name: matillion-run-etl-job
description: Validate and then execute an ETL job in a specific group, project, version, and job name.
api: openapi/matillion-etl-jobs-runs-api-openapi.yml
operations:
- validateEtlJob
- runEtlJob
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/matillion-etl-jobs-runs-api-openapi.yml ; every operationId checked against the contract
---

# matillion-run-etl-job

Validate and then execute an ETL job in a specific group, project, version, and job name.

## Steps

1. 1. Call `validateEtlJob` with path parameters `group`, `project`, `version`, `job`.
2. 2. Call `runEtlJob` with path parameters `group`, `project`, `version`, `job`.

## Rules

- Auth: Include an `Authorization` header using either the `dpc_oauth` (OAuth2) or `etl_basic` (HTTP Basic) scheme.
- Rate limiting: No rate limit is defined; on exhaustion the API returns no specific HTTP status.
