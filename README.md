# Apache Livy (apache-livy)
Apache Livy is a service that enables easy interaction with a Spark cluster over a REST interface. It allows submitting Spark jobs or snippets of Spark code, retrieving results synchronously or asynchronously, and managing Spark contexts across multiple users.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Big Data, Interactive Computing, Open Source, REST, Spark

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Apache Livy REST API
The Livy REST API provides endpoints for creating and managing interactive Spark sessions, submitting batch Spark jobs, executing code statements, and retrieving job results and logs.

**Human URL:** [https://livy.apache.org/docs/latest/rest-api.html](https://livy.apache.org/docs/latest/rest-api.html)

#### Tags:

 - Batch Jobs, REST, Sessions, Spark

#### Properties

- [Documentation](https://livy.apache.org/docs/latest/rest-api.html)
- [OpenAPI](openapi/apache-livy-rest-api.yaml)

## Common Properties

- [GitHubOrganization](https://github.com/apache)
- [GitHubRepository](https://github.com/apache/incubator-livy)
- [Documentation](https://livy.apache.org/docs/latest/)
- [GettingStarted](https://livy.apache.org/get-started/)
- [TermsOfService](https://www.apache.org/licenses/LICENSE-2.0)
- [Versioning](https://livy.apache.org/download/)
- [SpectralRules](rules/apache-livy-spectral-rules.yml)
- [Vocabulary](vocabulary/apache-livy-vocabulary.yaml)
- [NaftikoCapability](capabilities/spark-job-management.yaml)

## Features

| Name | Description |
|------|-------------|
| Interactive Spark Sessions | Create persistent Spark contexts for interactive code execution in Python, Scala, R, and SQL. |
| Batch Job Submission | Submit batch Spark jobs without creating an interactive session. |
| Multi-Language Support | Execute code in PySpark, Spark (Scala), SparkR, and SQL. |
| Multi-User Impersonation | Proxy user support for multi-tenant Spark cluster access. |
| Asynchronous Execution | Submit jobs and poll for results asynchronously. |
| Log Access | Retrieve driver and executor logs for debugging. |
| REST Interface | Simple HTTP REST API for Spark cluster interaction without native clients. |

## Use Cases

| Name | Description |
|------|-------------|
| Notebook Integration | Power Jupyter, Zeppelin, and other notebooks with Spark backends via Livy. |
| Data Engineering Pipelines | Submit Spark batch jobs from orchestration tools like Airflow and Oozie. |
| Interactive Data Exploration | Execute ad-hoc Spark code for exploratory data analysis. |
| Multi-Tenant Spark Access | Enable multiple users to share a Spark cluster with isolation via Livy sessions. |

## Integrations

| Name | Description |
|------|-------------|
| Apache Spark | Livy requires a Spark cluster and acts as the REST gateway to Spark. |
| Apache Zeppelin | Zeppelin notebook backend using Livy for distributed Spark execution. |
| Jupyter Notebook | Jupyter sparkmagic extension uses Livy for remote Spark kernel access. |
| Apache Airflow | Airflow LivyOperator for submitting Spark batch jobs from DAGs. |
| Amazon EMR | Livy is available as an EMR application for REST-based Spark access. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Apache Livy REST API](openapi/apache-livy-rest-api.yaml)

### JSON Schema

12 schema files extracted from the REST API OpenAPI specification.

### JSON Structure

12 JSON Structure files converted from JSON Schema files.

### Examples

12 example JSON files generated from JSON Schema definitions.

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Apache Livy REST API](capabilities/shared/livy-rest-api.yaml) — 7 operations for session, statement, and batch management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Apache Livy Spark Job Management](capabilities/spark-job-management.yaml) | Apache Livy REST API | 7 | Data Engineer, Data Scientist |

## Vocabulary

- [Apache Livy Vocabulary](vocabulary/apache-livy-vocabulary.yaml) — Unified taxonomy mapping 3 resources, 7 actions, 1 workflow, and 2 personas

## Rules

- [Apache Livy Spectral Rules](rules/apache-livy-spectral-rules.yml) — 13 rules across 7 categories enforcing Apache Livy REST API conventions

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
