# CAMM L2 — Adoption Stage

> **Level:** 2 | **Name:** Adoption | **Typical Duration:** 6–12 months

---

## What This Level Is About

L2 is expansion. The pilot succeeded. Now the program scales to 10+ facilities, connects to national reporting systems, and builds local capacity to manage the platform independently.

---

## Entry Gate

- L1 exit criteria all met ✅
- Production system stable for 60 days ✅

---

## Activities During L2

### 1. Multi-Facility Rollout
- Scale from 1 to 10+ facilities using `zs-iac-template-site`
- Each new facility takes 1–2 days to onboard (vs weeks at L1)
- Local IT staff manages facility onboarding with template

### 2. DHIS2 Connection
- Configure `zs-svc-dhis2-bridge` for national HMIS
- Map ZarishSphere indicators to DHIS2 data elements
- Establish automated weekly aggregate reporting

### 3. Local Capacity Building
- Train 2 country-level "super users" to manage the platform
- Train facility IT staff on basic troubleshooting
- Establish local helpdesk process

### 4. Country-Specific Forms
- Complete all forms required for national reporting
- All forms validated against ZS Form Schema v1
- Bengali/Burmese/Urdu/Hindi translations complete

### 5. Monitoring and Alerting
- Configure Grafana 12.x dashboards for country program
- Set up EWARS threshold alerts for communicable diseases
- Weekly automated indicator reports to program management

---

## Exit Criteria (to advance to L3)

- [ ] 10+ facilities live with regular clinical data entry
- [ ] DHIS2 aggregate reporting automated
- [ ] 2 trained country super users
- [ ] All required program forms deployed and in use
- [ ] Country can onboard a new facility without ZarishSphere core team
- [ ] 3 months of stable operations without critical incidents

---

## Deliverables

| Deliverable | Where |
|-------------|-------|
| Multi-facility infra state | `zs-infra-{cc}` |
| DHIS2 bridge config | `zs-distro-{cc}/config/dhis2/` |
| Country super user certification | `zs-docs-camm/countries/{CC}-STATUS.md` |
| Quarterly impact report (L2) | `zs-docs-donor/reports/` |
