---
name: matillion-launch-pipeline-execution
description: Launch a pipeline execution and monitor its progress.
api: openapi/matillion-dpc-pipeline-executions-api-openapi.yml
operations:
- createPipelineExecution
- getPipelineExecutionStatus
- getPipelineExecutionSteps
- cancelPipelineExecution
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/matillion-dpc-pipeline-executions-api-openapi.yml ; every operationId checked against the contract
---

# matillion-launch-pipeline-execution

Launch a pipeline execution and monitor its progress.

## Steps

1. 1. `createPipelineExecution` – requires the `projectId` path parameter and a request body describing the pipeline to launch.
2. 2. `getPipelineExecutionStatus` – requires `projectId` and `id` path parameters to poll the execution status.
3. 3. `getPipelineExecutionSteps` – requires `projectId` and `id` path parameters to retrieve the steps of the execution.
4. 4. `cancelPipelineExecution` – optional; requires `projectId` and `id` path parameters with a body containing `status: CANCELLED` to stop a running execution.

## Rules

- Authentication: include an Authorization header using the `dpc_oauth` OAuth2 scheme or the `etl_basic` HTTP Basic scheme.
- Pagination: the `listPipelineExecutions` operation supports pagination, but it is not used in this skill.
