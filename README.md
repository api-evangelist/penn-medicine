# Penn Medicine

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

Penn Medicine is the University of Pennsylvania Health System (UPHS) plus the Perelman School of Medicine. It is an $11.9 billion enterprise powered by nearly 49,000 faculty and staff, operating six hospitals (Hospital of the University of Pennsylvania, Penn Presbyterian Medical Center, Chester County Hospital, Lancaster General Health, Princeton Health, and Pennsylvania Hospital — the first hospital in the United States, chartered in 1751) plus Penn Medicine at Home, Good Shepherd Penn Partners Rehabilitation, Lancaster Behavioral Health Hospital, and Princeton House Behavioral Health. The Perelman School of Medicine was awarded $580 million in NIH funding in fiscal year 2023. From an API perspective, Penn Medicine runs a production Epic-backed HL7 FHIR R4 endpoint at `https://ssproxy.pennhealth.com/PRD-FHIR/api/FHIR/R4` (Epic Organization ID 346, implementation description "University of Pennsylvania Health Systems FHIR Server"). The CapabilityStatement instantiates `us-core-server|6.1.0` and the HL7 Bulk Data Access IG, exposes 59 FHIR resource types covering Patient Access (clinical + claims) and Provider Directory per CMS-9115-F, and protects them with OAuth 2.0 / SMART-on-FHIR. Penn Medicine also operates the MyPennMedicine MyChart patient portal and the PhysicianLink referring-provider portal, and publishes open-source informatics work through several Perelman School of Medicine GitHub orgs (Penn-Medicine-CHCI, pennsignals, PMACS, pennbiobank).

**Areas:** Healthcare · Hospitals · Academic Medical Center · FHIR · SMART on FHIR · Patient Access · Provider Directory · CMS Interoperability · US Core · Bulk Data · Epic

## Penn Medicine on APIs.io

Everything profiled for Penn Medicine is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/penn-medicine/](https://apis.io/providers/penn-medicine/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [MyPennMedicine Patient Portal](https://apis.io/apis/penn-medicine/mypennmedicine-patient-portal/) — MyChart-based patient portal that gives Penn Medicine patients access to medical records, lab results, secure messaging with their care team, telehealth…
- [PhysicianLink Referring Physician Portal](https://apis.io/apis/penn-medicine/physicianlink-referring-physician-portal/) — EpicLink-based portal for community and referring physicians that provides secure access to Penn Medicine patient records: clinical notes, lab and imaging…
- [Penn Medicine Open Source Health Informatics](https://apis.io/apis/penn-medicine/penn-medicine-open-source-health-informatics/) — Penn Medicine and the Perelman School of Medicine publish open-source health-informatics software across several GitHub organizations: Penn Medicine Center…
- [Penn Medicine Bulk Data API](https://apis.io/apis/penn-medicine/penn-medicine-bulk-data-api/) — HL7 FHIR Bulk Data Access (Flat FHIR) Group-level export.
- [Penn Medicine Patient Access API](https://apis.io/apis/penn-medicine/penn-medicine-patient-access-api/) — Patient-mediated clinical and claims data resources required under CMS-9115-F.
- [Penn Medicine Provider Directory API](https://apis.io/apis/penn-medicine/penn-medicine-provider-directory-api/) — Public provider, organization, location, and endpoint resources required under CMS-9115-F.
- [Penn Medicine SMART API](https://apis.io/apis/penn-medicine/penn-medicine-smart-api/) — SMART on FHIR launch and discovery endpoints.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Penn Medicine Agentic Access](https://apis.io/agentic-access/penn-medicine/penn-medicine-agentic-access/)

#### JSON Schema (4)

The data models the API reads and writes.

- [Penn Medicine FHIR Observation](https://apis.io/schemas/penn-medicine/penn-medicine-fhir-observation/)
- [Penn Medicine FHIR Organization](https://apis.io/schemas/penn-medicine/penn-medicine-fhir-organization/)
- [Penn Medicine FHIR Patient](https://apis.io/schemas/penn-medicine/penn-medicine-fhir-patient/)
- [Penn Medicine FHIR Practitioner](https://apis.io/schemas/penn-medicine/penn-medicine-fhir-practitioner/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Penn Medicine Context](https://apis.io/jsonld/penn-medicine/penn-medicine-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Penn Medicine Vocabulary](https://apis.io/vocabularies/penn-medicine/penn-medicine-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Penn Medicine Fhir Bulk Export Example](https://apis.io/examples/penn-medicine/penn-medicine-fhir-bulk-export-example/)
- [Penn Medicine Fhir Observation Example](https://apis.io/examples/penn-medicine/penn-medicine-fhir-observation-example/)
- [Penn Medicine Fhir Organization Example](https://apis.io/examples/penn-medicine/penn-medicine-fhir-organization-example/)
- [Penn Medicine Fhir Patient Example](https://apis.io/examples/penn-medicine/penn-medicine-fhir-patient-example/)
- [Penn Medicine Fhir Practitioner Example](https://apis.io/examples/penn-medicine/penn-medicine-fhir-practitioner-example/)

#### Collections (5)

Postman and Open Collection request collections.

- [Penn Medicine FHIR R4 Bulk Data API](https://apis.io/collections/penn-medicine/open-penn-medicine-bulk-data-api/)
- [Penn Medicine FHIR R4 API](https://apis.io/collections/penn-medicine/open-penn-medicine-fhir-r4/)
- [Penn Medicine FHIR R4 Bulk Data Patient Access API](https://apis.io/collections/penn-medicine/open-penn-medicine-patient-access-api/)
- [Penn Medicine FHIR R4 Bulk Data Provider Directory API](https://apis.io/collections/penn-medicine/open-penn-medicine-provider-directory-api/)
- [Penn Medicine FHIR R4 Bulk Data SMART API](https://apis.io/collections/penn-medicine/open-penn-medicine-smart-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Penn Medicine — fhir rules](https://apis.io/rules/penn-medicine/penn-medicine-fhir-rules/)
- [Penn Medicine — jsonschema rules](https://apis.io/rules/penn-medicine/penn-medicine-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Penn Medicine Authentication](https://apis.io/security/penn-medicine/penn-medicine-authentication/)
- [Penn Medicine Domain Security](https://apis.io/security/penn-medicine/penn-medicine-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Penn Medicine Scopes](https://apis.io/scopes/penn-medicine/penn-medicine-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Penn Medicine Plans Pricing](https://apis.io/plans/penn-medicine/penn-medicine-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Penn Medicine Rate Limits](https://apis.io/rate-limits/penn-medicine/penn-medicine-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Penn Medicine Finops](https://apis.io/finops/penn-medicine/penn-medicine-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.pennmedicine.org/)
- [Support](https://www.pennmedicine.org/contact-us)
- [Blog](https://www.pennmedicine.org/news)
- [Compliance](https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records)
- [Terms of service](https://www.pennmedicine.org/terms-of-use)
- [Privacy policy](https://www.pennmedicine.org/privacy-policy)
- [GitHub](https://github.com/Penn-Medicine-CHCI)

## API Evangelist rating

**Kin Score 38.1** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 62.0 |
| Contract governance | 27.3 |
| Operational transparency | 21.1 |
| Developer ergonomics | 35.7 |
| Access clarity | 7.9 |

**Agent readiness 28.0** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 26.6** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/penn-medicine/](https://apis.io/providers/penn-medicine/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Penn Medicine: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/penn-medicine/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
