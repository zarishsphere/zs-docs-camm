# CAMM L0 — Interest Stage

> **Level:** 0 | **Name:** Interest | **Typical Duration:** 1–3 months

---

## What This Level Is About

At L0, a country, program, or organisation has discovered ZarishSphere and is evaluating it. The goal of L0 is to move from "we heard about this" to "we have a signed commitment and a clear plan."

---

## Entry Gate

No prerequisites — any organisation can start at L0.

---

## Activities During L0

### 1. Initial Outreach and Discovery
- Introductory call with ZarishSphere Health Programs team
- Share ZarishSphere overview deck and BLUEPRINT.md
- Review CAMM model and understand the journey

### 2. Needs Assessment
Complete the [NEEDS-ASSESSMENT.md](../templates/NEEDS-ASSESSMENT.md) questionnaire:
- Number of health facilities in scope
- Current HIS systems in use
- Connectivity situation (internet, power reliability)
- Device types available (Android phones, tablets, computers)
- Key clinical domains needed (maternal health, EPI, nutrition...)
- Staff capacity (number of health workers, IT staff)
- Data sovereignty requirements

### 3. Technical Readiness Assessment
Complete [TECHNICAL-READINESS.md](../templates/TECHNICAL-READINESS.md):
- Server/hosting situation (cloud, on-premise, Raspberry Pi)
- Network infrastructure
- Android device availability for community health workers

### 4. MOU Signing
Both parties sign the [MOU-TEMPLATE.md](../templates/MOU-TEMPLATE.md):
- ZarishSphere commits: platform access, documentation, community support
- Country/program commits: designated focal point, participation in community, sharing back

---

## Exit Criteria (to advance to L1)

- [ ] Needs assessment completed and documented
- [ ] Technical readiness assessment completed
- [ ] MOU signed by authorized representative of both parties
- [ ] Country distro repository created (e.g., `zs-distro-bgd`)
- [ ] Country infrastructure repository created (e.g., `zs-infra-bgd`)
- [ ] Designated country focal point added as GitHub org member
- [ ] Country/program-specific forms requirements documented

---

## Deliverables

| Deliverable | Where It Lives |
|-------------|---------------|
| Completed needs assessment | `zs-docs-camm/countries/{CC}-STATUS.md` |
| Signed MOU | `zs-docs-donor/grants/` (private copy) |
| Country distro repo | `github.com/zarishsphere/zs-distro-{cc}` |
| Country infra repo | `github.com/zarishsphere/zs-infra-{cc}` |
