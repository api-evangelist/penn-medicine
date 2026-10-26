# Penn Medicine (penn-medicine)

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

Penn Medicine is the University of Pennsylvania Health System (UPHS) plus the Perelman School of Medicine. It is an $11.9 billion enterprise powered by nearly 49,000 faculty and staff, operating six hospitals (Hospital of the University of Pennsylvania, Penn Presbyterian Medical Center, Chester County Hospital, Lancaster General Health, Princeton Health, and Pennsylvania Hospital — the first hospital in the United States, chartered in 1751) plus Penn Medicine at Home, Good Shepherd Penn Partners Rehabilitation, Lancaster Behavioral Health Hospital, and Princeton House Behavioral Health. The Perelman School of Medicine was awarded $580 million in NIH funding in fiscal year 2023.

From an API perspective, Penn Medicine runs a production Epic-backed HL7 FHIR R4 endpoint at `https://ssproxy.pennhealth.com/PRD-FHIR/api/FHIR/R4` (Epic Organization ID 346, implementation description "University of Pennsylvania Health Systems FHIR Server"). The CapabilityStatement instantiates `us-core-server|6.1.0` and the HL7 Bulk Data Access IG, exposes 59 FHIR resource types covering Patient Access (clinical + claims) and Provider Directory per CMS-9115-F, and protects them with OAuth 2.0 / SMART-on-FHIR. Penn Medicine also operates the MyPennMedicine MyChart patient portal and the PhysicianLink referring-provider portal, and publishes open-source informatics work through several Perelman School of Medicine GitHub orgs (Penn-Medicine-CHCI, pennsignals, PMACS, pennbiobank).

**APIs.json:** [https://github.com/api-evangelist/penn-medicine](https://github.com/api-evangelist/penn-medicine)

## Tags

- Healthcare
- Hospital
- Academic Medical Center
- FHIR
- SMART On FHIR
- Patient Access
- Provider Directory
- CMS Interoperability
- US Core
- Bulk Data
- Epic

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### Penn Medicine FHIR R4 API

The University of Pennsylvania Health Systems FHIR Server. Epic (November 2025) on the back end,
conforming to US Core 6.1.0 and the HL7 Bulk Data Access IG. Serves Patient Access (clinical + claims)
and Provider Directory data per CMS-9115-F, exposing 59 FHIR resource types including Patient,
AllergyIntolerance, Condition, Observation, MedicationRequest, Immunization, Procedure, Encounter,
DiagnosticReport, DocumentReference, Coverage, ExplanationOfBenefit, Claim, Practitioner,
PractitionerRole, Organization, Location, and Endpoint. App registration is performed through
Epic on FHIR (https://fhir.epic.com) by selecting Penn Medicine (Organization ID 346) as the target.

- **Human URL:** [https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records](https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records)
- **Base URL:** `https://ssproxy.pennhealth.com/PRD-FHIR/api/FHIR/R4`

#### Tags

- FHIR
- SMART On FHIR
- Patient Access
- Provider Directory
- Bulk Data
- US Core

#### Properties

- [Documentation](https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records)
- [API Reference](https://ssproxy.pennhealth.com/PRD-FHIR/api/FHIR/R4/metadata)
- [OpenAPI](openapi/penn-medicine-fhir-r4-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/penn-medicine-fhir-r4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/penn-medicine-fhir-r4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/penn-medicine-fhir-patient-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/penn-medicine-fhir-organization-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/penn-medicine-fhir-practitioner-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/penn-medicine-fhir-observation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/penn-medicine-fhir-patient-example.json)
- [Example](examples/penn-medicine-fhir-organization-example.json)
- [Example](examples/penn-medicine-fhir-practitioner-example.json)
- [Example](examples/penn-medicine-fhir-observation-example.json)
- [Example](examples/penn-medicine-fhir-bulk-export-example.json)
- [Authentication](https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/authorize)
- [Sandbox](https://fhir.epic.com/Documentation?docId=testpatients)

### MyPennMedicine Patient Portal

MyChart-based patient portal that gives Penn Medicine patients access to medical records, lab
results, secure messaging with their care team, telehealth visits, medication refills, prescription
management, bill pay, and appointment scheduling across UPHS facilities. SMART apps approved via
Epic on FHIR connect to the underlying Penn Medicine FHIR R4 API.

- **Human URL:** [https://www.pennmedicine.org/patient-resources/mypennmedicine](https://www.pennmedicine.org/patient-resources/mypennmedicine)
- **Base URL:** `https://secure.mypennmedicine.org`

#### Tags

- Patient Portal
- MyChart
- Patient Access

#### Properties

- [Portal](https://secure.mypennmedicine.org/)
- [Documentation](https://www.pennmedicine.org/patient-resources/mypennmedicine)
- [Postman Collection](collections/penn-medicine-fhir-r4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/penn-medicine-fhir-r4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhysicianLink Referring Physician Portal

EpicLink-based portal for community and referring physicians that provides secure access to Penn
Medicine patient records: clinical notes, lab and imaging results, medication lists, and the
ability to refer patients and follow care for shared patients.

- **Human URL:** [https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records/physicianlink](https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records/physicianlink)
- **Base URL:** `https://secure3.pennmedicine.org/EpicLink`

#### Tags

- Referring Provider
- EMR Access
- Epic

#### Properties

- [Portal](https://secure3.pennmedicine.org/EpicLink/common/epic_login.asp)
- [Documentation](https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records/physicianlink)
- [Postman Collection](collections/penn-medicine-fhir-r4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/penn-medicine-fhir-r4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Penn Medicine Open Source Health Informatics

Penn Medicine and the Perelman School of Medicine publish open-source health-informatics software
across several GitHub organizations: Penn Medicine Center for Health Care Innovation
(Penn-Medicine-CHCI, behind the Cobalt mental-health platform — cobalt-api in Java and cobalt-web
in TypeScript); Penn Signals / Penn Medicine Predictive Healthcare (pennsignals — Databricks
MCP agent templates; historically the home of CHIME, the COVID-19 Hospital Impact Model); Penn
Medicine Academic Computing Services (PMACS — 17 Rails libraries, JSON:API tools, Oracle adapters,
and Slate API docs); and the Penn Medicine BioBank (pennbiobank).

- **Human URL:** [https://github.com/pennmedicine](https://github.com/pennmedicine)

#### Tags

- Open Source
- Health Informatics
- GitHub

#### Properties

- [GitHub Organization](https://github.com/Penn-Medicine-CHCI)
- [GitHub Organization](https://github.com/pennsignals)
- [GitHub Organization](https://github.com/PMACS)
- [GitHub Organization](https://github.com/pennbiobank)
- [GitHub Organization](https://github.com/pennmedicine)
- [GitHub Repository](https://github.com/Penn-Medicine-CHCI/cobalt-api)
- [GitHub Repository](https://github.com/Penn-Medicine-CHCI/cobalt-web)
- [Postman Collection](collections/penn-medicine-fhir-r4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/penn-medicine-fhir-r4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.pennmedicine.org)
- [Developer Portal](https://fhir.epic.com)
- [GitHub Organization](https://github.com/Penn-Medicine-CHCI)
- [GitHub Organization](https://github.com/pennsignals)
- [GitHub Organization](https://github.com/PMACS)
- [Blog](https://www.pennmedicine.org/news)
- [Privacy Policy](https://www.pennmedicine.org/privacy-policy)
- [Terms of Service](https://www.pennmedicine.org/terms-of-use)
- [Compliance](https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records)
- [Support](https://www.pennmedicine.org/contact-us)
- [LinkedIn](https://www.linkedin.com/company/penn-medicine)
- [Spectral Rules](rules/penn-medicine-fhir-rules.yml)
- [JSON-LD](json-ld/penn-medicine-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/penn-medicine-vocabulary.yml)
- [Plans](plans/penn-medicine-plans-pricing.yml)
- [Rate Limits](rate-limits/penn-medicine-rate-limits.yml)
- [Fin Ops](finops/penn-medicine-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
