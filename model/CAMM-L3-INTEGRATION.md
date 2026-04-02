# CAMM L3 — Integration Stage

> **Level:** 3 | **Name:** Integration | **Typical Duration:** 12–18 months

---

## What This Level Is About

L3 is national system integration. ZarishSphere connects to the national health information infrastructure: DHIS2 (bidirectional), laboratory systems (HL7v2), possibly ABDM (India) or SGDB (Bangladesh). The Ministry of Health is an active partner.

---

## Entry Gate

- L2 exit criteria all met ✅
- Ministry of Health endorsement obtained ✅

---

## Activities During L3

### 1. National System Bridges
- **DHIS2 bidirectional:** aggregate + tracker sync via `zs-int-dhis2`
- **HL7v2 lab results:** configure `zs-int-hl7v2` for national lab systems
- **National drug codes:** load into `zs-data-rxnorm` with local mappings
- **India only:** ABDM integration via `zs-int-abdm`

### 2. National Terminology Alignment
- Load national facility registry into `zs-data-facility-registry`
- Map local diagnosis codes to ICD-11 in `zs-data-concept-maps`
- Add national laboratory panels to LOINC mappings

### 3. Government Data Governance
- Establish data sharing agreement with MoH
- Configure data residency (country data stays in country)
- Implement field-level encryption for PHI at rest

### 4. National Indicator Alignment
- Map ZarishSphere indicators to national KPIs
- Automate MoH monthly/quarterly reports
- Configure EWARS national threshold settings

---

## Exit Criteria (to advance to L4)

- [ ] DHIS2 bidirectional sync live
- [ ] At least one national system integrated (lab, pharmacy, or registry)
- [ ] National facility registry loaded
- [ ] Country data stored in-country (data residency verified)
- [ ] MoH signs off on data quality
- [ ] 6 months of stable multi-system operations

---

## Deliverables

| Deliverable | Where |
|-------------|-------|
| Integration configs | `zs-distro-{cc}/config/` |
| National system mapping docs | `zs-docs-standards/` |
| Data residency verification | `zs-docs-security/compliance/` |
