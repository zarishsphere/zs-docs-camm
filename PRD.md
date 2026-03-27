# PRD — `zs-docs-camm`

> **Document Class:** PRD | **Version:** 1.0.0 | **Status:** Bootstrapping
> **Repository:** [https://github.com/zarishsphere/zs-docs-camm](https://github.com/zarishsphere/zs-docs-camm)
> **Layer:** Layer 0 — Governance | **Catalog #:** 6
> **License:** Apache 2.0 | **Governance:** RFC-0001

---

## 1. Overview

Country Adoption Maturity Model (CAMM) documentation. Defines the L0–L5 framework for onboarding countries to ZarishSphere, with checklists, gates, and templates for each maturity level.

---

## 2. Repository Metadata

- **Name:** `zs-docs-camm`
- **Organization:** [https://github.com/zarishsphere](https://github.com/zarishsphere)
- **Language / Runtime:** Markdown
- **Visibility:** Public
- **License:** Apache 2.0
- **Default Branch:** `main`
- **Branch Protection:** Required (2-owner review for critical paths)

---

## 3. Platform Context

This repository is part of the **ZarishSphere** sovereign digital health operating platform — a free, open-source, FHIR R5-native system for South and Southeast Asia.

**Non-negotiable constraints:**
- Zero cost — all tooling must use genuinely free tiers
- FHIR R5 native — all clinical data modelled as FHIR R5 resources
- Offline-first — must work without network connectivity
- No-coder friendly — GUI-first, template-driven
- Documentation as Code — all decisions in GitHub

---

## 4. Goals & Objectives

- Define clear, measurable criteria for each CAMM maturity level (L0–L5)
- Provide actionable checklists for country program teams
- Track and publish adoption progress for all target countries

## 5. Functional Requirements

| ID | Requirement | Priority |
|----|------------|---------|
| F-01 | L0–L5 model definition with clear entry/exit gates | P0 |
| F-02 | Country onboarding checklist per level | P0 |
| F-03 | Signed MOU template for L0 | P1 |
| F-04 | Technical readiness assessment template | P1 |
| F-05 | Country status dashboard (published) | P2 |
| F-06 | Training curriculum outline per level | P2 |

## 6. Repository Tree

```
zs-docs-camm/
├── README.md                          # CAMM overview and country status
├── LICENSE
├── .github/
│   ├── CODEOWNERS
│   └── workflows/
│       └── ci.yml
├── model/
│   ├── CAMM-OVERVIEW.md               # L0–L5 model summary
│   ├── CAMM-L0-INTEREST.md            # Interest stage: MOU, needs assessment
│   ├── CAMM-L1-FOUNDATION.md          # Foundation: first facility, training
│   ├── CAMM-L2-ADOPTION.md            # Adoption: 10+ facilities, DHIS2
│   ├── CAMM-L3-INTEGRATION.md         # Integration: MOH bridges live
│   ├── CAMM-L4-MATURITY.md            # Maturity: national rollout
│   └── CAMM-L5-SOVEREIGNTY.md         # Sovereignty: self-managed
├── countries/
│   ├── BGD-STATUS.md                  # Bangladesh CAMM progress
│   ├── IND-STATUS.md                  # India CAMM progress
│   ├── MMR-STATUS.md                  # Myanmar CAMM progress
│   ├── PAK-STATUS.md                  # Pakistan CAMM progress
│   └── THA-STATUS.md                  # Thailand CAMM progress
├── templates/
│   ├── MOU-TEMPLATE.md                # Memorandum of Understanding template
│   ├── NEEDS-ASSESSMENT.md            # L0 needs assessment form
│   ├── TECHNICAL-READINESS.md         # Technical readiness checklist
│   └── TRAINING-CURRICULUM.md         # Training outline per level
└── governance/
    └── CAMM-GOVERNANCE.md             # Who approves level promotions
```

## 9. Ownership & Governance

| Role | GitHub User |
|------|-------------|
| Platform Lead | `@arwa-zarish` |
| Technical Lead | `@code-and-brain` |
| DevOps Lead | `@DevOps-Ariful-Islam` |
| Health Programs | `@BGD-Health-Program` |

All changes go through Pull Request → 1+ owner review → CI pass → merge.
Breaking changes require RFC + ADR.

---

## 10. Definition of Done

- [ ] All listed files exist with content
- [ ] CI pipeline passes (test + lint + security)
- [ ] README.md reflects current state
- [ ] OpenAPI / AsyncAPI spec present (services only)
- [ ] At least 1 integration test using testcontainers-go (Go) or Playwright (UI)
- [ ] No secrets committed (GitGuardian verified)
- [ ] CODEOWNERS file present
- [ ] Linked to CATALOGS.md and TODO.md

---

*This PRD is the canonical source of truth for this repository's purpose, structure, and requirements.*
*Changes require a PR against this file with owner approval.*
