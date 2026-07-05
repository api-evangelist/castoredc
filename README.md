# Castor (castoredc)

Castor (Castor EDC / CDMS) is a cloud electronic data capture (EDC) and clinical data management platform for clinical trials and real-world research. Its RESTful API at `https://data.castoredc.com/api` exposes study configuration and collected data - studies, participants (records), institutes (sites), users, fields and field metadata, study data points, repeating data (reports), surveys and survey packages, audit trail, and batch data export - authenticated with OAuth2 client-credentials. The API powers integrations with external systems, automated data entry and extraction, and statistical analysis via the official R and Python wrapper packages.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/apis.yml)

## Tags

- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- Healthcare
- Life Sciences
- Research

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## Authentication

The Castor API uses OAuth2 with the Client Credentials flow. Generate an API Client ID and Client Secret from your Castor **User Settings**, then request an access token from `POST https://data.castoredc.com/api/oauth/token` with `grant_type=client_credentials`. Tokens are valid for 5 hours and are passed as a `Bearer` token on every request. Most IDs (study, field, report/repeating-data instance, survey package instance) are uppercase GUIDs in `8-4-4-4-12` format; the participant ID is the exception.

## APIs

### Castor Studies API

List the studies your API client can access and retrieve a single study's configuration and metadata. A study is the top-level container in Castor; its GUID (the `study_id`) is required by nearly every other endpoint.

- **Human URL:** [https://helpdesk.castoredc.com/hc/en-us/articles/27149233860509-Castor-EDC-CDMS-Application-Programming-Interface-API](https://helpdesk.castoredc.com/hc/en-us/articles/27149233860509-Castor-EDC-CDMS-Application-Programming-Interface-API)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Studies
- Metadata
- Configuration

#### Properties

- [Documentation](https://helpdesk.castoredc.com/hc/en-us/articles/27149233860509-Castor-EDC-CDMS-Application-Programming-Interface-API)
- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Participants (Records) API

Create, list, and retrieve participants (records / subjects) enrolled in a study, including their institute assignment, randomization status, progress, and lifecycle. Participants are the entities that data points are collected against.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Participants
- Records
- Subjects

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Institutes API

List and retrieve the institutes (sites / centers) participating in a study, and create new institutes. Institutes group participants for multi-center trials and drive site-level access control and reporting.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Institutes
- Sites
- Multi-Center

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Users API

List the users the authenticated account can see, retrieve a single user, and list the users who are members of a given study. Used to reconcile study membership and site staff with external identity and CTMS systems.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Users
- Access
- Membership

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Fields API

Retrieve the data-capture fields that define a study's forms, plus their supporting metadata - field dependencies (conditional logic), option groups (answer choices), and field validations. This is the schema you need to interpret and write study data points correctly.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Fields
- Field Metadata
- Option Groups

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Study Data Points API

Read and write the actual collected values (data points) for the study forms of a participant - retrieve all study data points for a study or a single participant, and create or update participant study data points programmatically.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Data Points
- Data Entry
- Data Extraction

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Reports (Repeating Data) API

Work with reports (now called repeating data) - unscheduled or repeatable forms such as adverse events or medications. List report definitions, list and create repeating-data instances for a participant, and read or write their data points.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Reports
- Repeating Data
- Instances

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Surveys API

Manage surveys and electronic patient-reported outcomes (ePRO) - list survey definitions, send survey packages to participants (creating survey-package instances), check survey compliance, and read survey data points and instances.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Surveys
- ePRO
- Survey Packages

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Audit Trail API

Retrieve the immutable audit trail for a study - the who, what, and when of every data and configuration change - to support GCP / 21 CFR Part 11 compliance, monitoring, and reconciliation with external quality systems.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Audit Trail
- Compliance
- GCP

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Castor Data Export API

Request and download bulk exports of a study - the collected data, the study structure, and the option groups - for downstream statistical analysis, archiving, and data warehousing.

- **Human URL:** [https://data.castoredc.com/api](https://data.castoredc.com/api)
- **Base URL:** `https://data.castoredc.com/api`

#### Tags

- Export
- Bulk Data
- Structure

#### Properties

- [API Reference](https://data.castoredc.com/api)
- [OpenAPI](openapi/castoredc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/castoredc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/castoredc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/castoredc)
- [Website](https://www.castoredc.com)
- [Documentation](https://helpdesk.castoredc.com/application-programming-interface-api)
- [Plans](plans/castoredc-plans-pricing.yml)
- [Rate Limits](rate-limits/castoredc-rate-limits.yml)
- [Fin Ops](finops/castoredc-finops.yml)
- [Blog](https://www.castoredc.com/blog/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
