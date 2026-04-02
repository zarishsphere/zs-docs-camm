# CAMM L1 — Foundation Stage

> **Level:** 1 | **Name:** Foundation | **Typical Duration:** 3–6 months

---

## What This Level Is About

L1 is proof of concept with real patients. At least one real health facility is running ZarishSphere with real clinical data. The system works. Staff are trained. Core clinical modules are live.

---

## Entry Gate

- L0 exit criteria all met ✅
- MOU signed ✅
- Country distro and infra repos exist ✅

---

## Activities During L1

### 1. Platform Setup
- Fork `zs-iac-template-country` to `zs-infra-{cc}`
- Fork `zs-distro-core` to `zs-distro-{cc}`
- Deploy ZarishSphere to first facility (Raspberry Pi 5, cloud VM, or hosted)
- Configure Keycloak 26.5.6 with facility users and roles
- Load core forms from `zs-content-forms-core`

### 2. Core Clinical Configuration
- Configure patient registration form with local ID types
- Add facility to FHIR Location registry
- Set up user accounts for all clinical staff
- Configure notifications (SMS if available)

### 3. Staff Training
Complete [TRAINING-CURRICULUM.md](../templates/TRAINING-CURRICULUM.md) L1 module:
- Patient registration (2 hours)
- Encounter and vitals entry (2 hours)
- Clinical forms (3 hours)
- Data quality and audit (1 hour)
- Total: 8 hours per staff member

### 4. Pilot Go-Live
- Go live with first facility
- ZarishSphere team provides weekly support for first month
- Collect feedback from clinical staff

### 5. Form Customisation (if needed)
- Identify any gaps in core forms
- Create country-specific forms using `zs-ui-form-builder`
- Submit forms to `zs-content-forms-{domain}` via PR

---

## Exit Criteria (to advance to L2)

- [ ] At least 1 facility live with real patient data
- [ ] Minimum 50 patient encounters recorded in production
- [ ] All clinical staff at pilot facility trained
- [ ] Data quality audit completed (>90% complete records)
- [ ] Country focal point can create/modify forms without core team help
- [ ] Country-specific language added to `zs-data-translations` (if not English)
- [ ] Retrospective conducted with facility staff
- [ ] L1 report submitted to ZarishSphere Health Programs

---

## Deliverables

| Deliverable | Where |
|-------------|-------|
| Pilot facility live in production | `zs-infra-{cc}` deployed |
| Country distro with local forms | `zs-distro-{cc}` |
| Staff training completion records | `zs-docs-camm/countries/{CC}-STATUS.md` |
| L1 retrospective report | `zs-docs-donor/reports/` |
