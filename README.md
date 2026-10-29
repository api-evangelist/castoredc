# Castor

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

Castor (Castor EDC / CDMS) is a cloud electronic data capture (EDC) and clinical data management platform for clinical trials and real-world research. Its RESTful API at https://data.castoredc.com/api exposes study configuration and collected data - studies, participants (records), institutes (sites), users, fields and field metadata, study data points, repeating data (reports), surveys and survey packages, audit trail, and batch data export - authenticated with OAuth2 client-credentials. The API is used to integrate Castor with external systems, automate data entry and extraction, and support statistical analysis via the official R and Python wrapper packages.

**Areas:** Clinical Trials · Electronic Data Capture · EDC · Clinical Data Management · Healthcare · Life Sciences · Research

## Castor on APIs.io

Everything profiled for Castor is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/castoredc/](https://apis.io/providers/castoredc/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Castor Audit Trail API](https://apis.io/apis/castoredc/castoredc-audit-trail-api/) — Immutable audit trail of study changes.
- [Castor Data Export API](https://apis.io/apis/castoredc/castoredc-data-export-api/) — Bulk export of study data, structure, and option groups.
- [Castor Fields API](https://apis.io/apis/castoredc/castoredc-fields-api/) — Study fields and their metadata (dependencies, option groups, validations).
- [Castor Institutes API](https://apis.io/apis/castoredc/castoredc-institutes-api/) — Institutes (sites / centers) participating in a study.
- [Castor Metadata API](https://apis.io/apis/castoredc/castoredc-metadata-api/) — Reference metadata such as countries.
- [Castor Participants API](https://apis.io/apis/castoredc/castoredc-participants-api/) — Participants (records / subjects) enrolled in a study.
- [Castor Reports API](https://apis.io/apis/castoredc/castoredc-reports-api/) — Reports / repeating data and their instances.
- [Castor Studies API](https://apis.io/apis/castoredc/castoredc-studies-api/) — Studies accessible to the API client.
- [Castor Study Data Points API](https://apis.io/apis/castoredc/castoredc-study-data-points-api/) — Collected values for study forms.
- [Castor Surveys API](https://apis.io/apis/castoredc/castoredc-surveys-api/) — Surveys, survey packages, and ePRO.
- [Castor Users API](https://apis.io/apis/castoredc/castoredc-users-api/) — Users and study membership.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Castoredc Agentic Access](https://apis.io/agentic-access/castoredc/castoredc-agentic-access/)

#### Collections (12)

Postman and Open Collection request collections.

- [Castor EDC / CDMS API](https://apis.io/collections/castoredc/open-castoredc/)
- [Castor EDC / CDMS Audit Trail API](https://apis.io/collections/castoredc/open-castoredc-audit-trail-api/)
- [Castor EDC / CDMS Audit Trail Data Export API](https://apis.io/collections/castoredc/open-castoredc-data-export-api/)
- [Castor EDC / CDMS Audit Trail Fields API](https://apis.io/collections/castoredc/open-castoredc-fields-api/)
- [Castor EDC / CDMS Audit Trail Institutes API](https://apis.io/collections/castoredc/open-castoredc-institutes-api/)
- [Castor EDC / CDMS Audit Trail Metadata API](https://apis.io/collections/castoredc/open-castoredc-metadata-api/)
- [Castor EDC / CDMS Audit Trail Participants API](https://apis.io/collections/castoredc/open-castoredc-participants-api/)
- [Castor EDC / CDMS Audit Trail Reports API](https://apis.io/collections/castoredc/open-castoredc-reports-api/)
- [Castor EDC / CDMS Audit Trail Studies API](https://apis.io/collections/castoredc/open-castoredc-studies-api/)
- [Castor EDC / CDMS Audit Trail Study Data Points API](https://apis.io/collections/castoredc/open-castoredc-study-data-points-api/)
- [Castor EDC / CDMS Audit Trail Surveys API](https://apis.io/collections/castoredc/open-castoredc-surveys-api/)
- [Castor EDC / CDMS Audit Trail Users API](https://apis.io/collections/castoredc/open-castoredc-users-api/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Castoredc Authentication](https://apis.io/security/castoredc/castoredc-authentication/)
- [Castoredc Domain Security](https://apis.io/security/castoredc/castoredc-domain-security/)
- [Castoredc Vulnerability Disclosure](https://apis.io/security/castoredc/castoredc-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Castoredc Scopes](https://apis.io/scopes/castoredc/castoredc-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Castoredc Plans Pricing](https://apis.io/plans/castoredc/castoredc-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Castoredc Rate Limits](https://apis.io/rate-limits/castoredc/castoredc-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Castoredc Finops](https://apis.io/finops/castoredc/castoredc-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.castoredc.com)
- [Documentation](https://helpdesk.castoredc.com/application-programming-interface-api)
- [Blog](https://www.castoredc.com/blog/)

## API Evangelist rating

**Kin Score 29.1** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 46.3 |
| Contract governance | 0.0 |
| Operational transparency | 7.9 |
| Developer ergonomics | 22.6 |
| Access clarity | 7.9 |

**Agent readiness 23.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 27.3** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/castoredc/](https://apis.io/providers/castoredc/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Castor: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/castoredc/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
