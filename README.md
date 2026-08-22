# Apache Livy (apache-livy)

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
