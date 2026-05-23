# Penn Medicine

Penn Medicine is the University of Pennsylvania Health System (UPHS) plus the Perelman School of Medicine — an $11.9 billion enterprise powered by nearly 49,000 faculty and staff. UPHS operates six hospitals (Hospital of the University of Pennsylvania, Penn Presbyterian Medical Center, Chester County Hospital, Lancaster General Health, Princeton Health, and Pennsylvania Hospital — the first hospital in the United States, chartered in 1751) plus Penn Medicine at Home, Good Shepherd Penn Partners Rehabilitation, Lancaster Behavioral Health Hospital, and Princeton House Behavioral Health. The Perelman School of Medicine was awarded $580 million in NIH funding in fiscal year 2023.

From an API perspective, Penn Medicine runs a production Epic-backed HL7 FHIR R4 endpoint exposing CMS-9115-F Patient Access and Provider Directory resources, US Core 6.1.0, SMART on FHIR, and HL7 Bulk Data. Penn Medicine also operates the MyPennMedicine MyChart patient portal and the PhysicianLink referring-provider portal, and publishes open-source informatics work through several Perelman School of Medicine GitHub organizations.

## APIs

### Penn Medicine FHIR R4 API
Epic-backed FHIR R4 server, software identified as Epic November 2025 (released 2026-03-19), with `implementation.description` "University of Pennsylvania Health Systems FHIR Server". The live CapabilityStatement instantiates US Core 6.1.0 (`us-core-server|6.1.0`) and the HL7 Bulk Data IG (`bulk-data`), and advertises 59 FHIR resource types covering Patient Access (clinical + claims) and Provider Directory per CMS-9115-F.

- Base URL: `https://ssproxy.pennhealth.com/PRD-FHIR/api/FHIR/R4`
- CapabilityStatement: `https://ssproxy.pennhealth.com/PRD-FHIR/api/FHIR/R4/metadata`
- Authorization: `https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/authorize`
- Token: `https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token`
- App registration: [Epic on FHIR](https://fhir.epic.com) — select Penn Medicine (Organization ID 346).
- Public landing: [Penn Medicine Electronic Medical Records](https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records)

### MyPennMedicine Patient Portal
MyChart-based patient portal: medical records, lab results, secure messaging, telehealth, prescription refills, bill pay, and appointment scheduling across UPHS facilities. SMART apps approved via Epic on FHIR connect to the same underlying FHIR R4 surface.

- Portal: <https://secure.mypennmedicine.org/>
- Overview: <https://www.pennmedicine.org/patient-resources/mypennmedicine>

### PhysicianLink Referring Physician Portal
EpicLink-based portal for community and referring physicians, providing secure access to Penn Medicine patient records and the ability to refer patients into UPHS.

- Portal: <https://secure3.pennmedicine.org/EpicLink/common/epic_login.asp>
- Overview: <https://www.pennmedicine.org/for-health-care-professionals/for-physicians/electronic-medical-records/physicianlink>

### Penn Medicine Open Source Health Informatics
Penn Medicine and the Perelman School of Medicine publish open-source health-informatics software across several GitHub orgs.

- [Penn Medicine Center for Health Care Innovation](https://github.com/Penn-Medicine-CHCI) — Cobalt mental-health platform (cobalt-api in Java, cobalt-web in TypeScript), 3 public repos.
- [Penn Signals / Predictive Healthcare](https://github.com/pennsignals) — Databricks MCP agent templates; historically CHIME (COVID-19 Hospital Impact Model). 1 active public repo.
- [Penn Medicine Academic Computing Services](https://github.com/PMACS) — 17 Rails libraries, JSON:API tools, Oracle adapters, Slate API docs.
- [Penn Medicine BioBank](https://github.com/pennbiobank) — Perelman School of Medicine biorepository.
- [pennmedicine](https://github.com/pennmedicine) — Canonical org (1 public repo: covid-vaccine-scheduling_WWW).

## CMS Interoperability and Patient Access Compliance

| Surface | Status |
|---|---|
| FHIR R4 endpoint | Live at `https://ssproxy.pennhealth.com/PRD-FHIR/api/FHIR/R4` |
| FHIR version | 4.0.1 |
| US Core conformance | 6.1.0 (`us-core-server`) |
| Bulk Data IG | Declared in CapabilityStatement |
| SMART on FHIR | OAuth 2.0 authorize + token endpoints published |
| Provider Directory | Public, unauthenticated (Practitioner, PractitionerRole, Organization, Location, Endpoint) |
| Patient Access | Clinical + claims resources behind patient-context OAuth |
| Epic Organization ID | 346 |
| Resource types exposed | 59 (full list in the CapabilityStatement) |

## Artifacts in this repository

| Folder | Files |
|---|---|
| `openapi/` | 1 OpenAPI 3.1 spec covering Patient Access + Provider Directory + Bulk Data |
| `json-schema/` | 4 JSON Schemas (Patient, Organization, Practitioner, Observation) |
| `json-ld/` | 1 JSON-LD context mapping FHIR + schema.org |
| `examples/` | 5 FHIR example payloads (Patient, Organization, Practitioner, Observation, Bulk export manifest) |
| `rules/` | 1 Spectral ruleset enforcing Penn Medicine API conventions |
| `capabilities/` | 1 shared capability + 3 workflow capabilities (Patient Access, Provider Directory, Bulk Cohort Export) |
| `vocabulary/` | 1 controlled vocabulary covering Penn Medicine, the FHIR surface, and UPHS facilities |
| `plans/` | 1 API Commons Plans 0.1 file describing access tiers |
| `rate-limits/` | 1 API Commons Rate Limits 0.1 file capturing scaffold rate semantics |
| `finops/` | 1 FOCUS 1.3-aligned FinOps framework file for internal cost allocation |

## Notable absences

- Penn Medicine does not publish a self-service developer portal with hosted API keys, public pricing, or formal rate-limit documentation; access is governed via Epic on FHIR (patient and provider apps) or direct UPHS data-sharing agreements (system-level Bulk Data).
- No AsyncAPI / event-streaming spec is published.
- No public status page or changelog dedicated to the FHIR API.
- No SDKs published by Penn Medicine itself for the FHIR API — clients use any standard HL7 FHIR R4 SDK against the documented endpoints.

## Maintainer

Kin Lane — [API Evangelist](https://apievangelist.com)
