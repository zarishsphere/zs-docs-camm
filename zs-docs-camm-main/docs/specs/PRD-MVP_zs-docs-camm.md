# PRD-MVP — `zs-docs-camm`

> **Document:** Product Requirements (MVP) | **Version:** 1.0.0-mvp
> **Repository:** [https://github.com/zarishsphere/zs-docs-camm](https://github.com/zarishsphere/zs-docs-camm)
> **Layer:** Layer 0 — Governance | **Catalog #:** 6
> **Language:** Markdown | **License:** Apache 2.0

---

## Executive Summary

**Country Adoption Maturity Model — L0–L5 framework for country onboarding.**

This document defines the **Minimum Viable Product (MVP)** scope for `zs-docs-camm` within the ZarishSphere sovereign digital health platform. It covers what must be built first, acceptance criteria, user stories, and the complete repository file structure.


### Platform Non-Negotiables (apply to every repository)

| Constraint | Rule |
|-----------|------|
| **Zero Cost** | All tooling, hosting, and services must use genuinely free tiers |
| **Open Source** | Apache 2.0 license; all code public |
| **FHIR R5 Native** | All clinical data modelled as FHIR R5 resources |
| **Offline-First** | Must function without network connectivity |
| **No-Coder Friendly** | GUI-first, template-driven, automatable |
| **Documentation as Code** | All decisions in GitHub via RFC/ADR |
| **Multi-tenant** | tenant_id scoping on all data operations |
| **HIPAA/GDPR** | AuditEvent on all PHI access; field-level encryption |

---

## Problem Statement

Without this repository, platform contributors and country program teams lack the governance documentation they need. Decisions become tribal knowledge, standards are inconsistently applied, and the platform cannot scale across countries.

## MVP Goals

1. L0–L5 model fully documented with entry/exit gates
2. Bangladesh (BGD) status page current
3. MOU template available for L0 countries

## MVP Functional Requirements

| ID | Requirement | Acceptance Criteria | Priority |
|----|------------|---------------------|---------|
| M-01 | CAMM-OVERVIEW.md with L0-L5 descriptions and gates | All 6 levels defined | P0 |
| M-02 | One checklist per CAMM level | 6 checklist files present | P0 |
| M-03 | BGD-STATUS.md shows current CAMM level | File shows L1 Foundation | P0 |
| M-04 | MOU-TEMPLATE.md for L0 countries | Template present in templates/ | P1 |

## MVP Complete Repository Tree

```
zs-docs-camm/
├── README.md
├── LICENSE
├── .github/
│   ├── CODEOWNERS
│   └── workflows/
│       └── ci.yml
├── model/
│   ├── CAMM-OVERVIEW.md
│   ├── CAMM-L0-INTEREST.md
│   ├── CAMM-L1-FOUNDATION.md
│   ├── CAMM-L2-ADOPTION.md
│   ├── CAMM-L3-INTEGRATION.md
│   ├── CAMM-L4-MATURITY.md
│   └── CAMM-L5-SOVEREIGNTY.md
├── countries/
│   ├── BGD-STATUS.md
│   ├── IND-STATUS.md
│   ├── MMR-STATUS.md
│   ├── PAK-STATUS.md
│   └── THA-STATUS.md
└── templates/
    ├── MOU-TEMPLATE.md
    ├── NEEDS-ASSESSMENT.md
    └── TECHNICAL-READINESS.md
```

---


## Owners & Governance

| Role | GitHub Handle | Responsibility |
|------|--------------|----------------|
| Platform Lead | `@arwa-zarish` | Final approval, RFC votes |
| Technical Lead | `@code-and-brain` | Architecture, Go/TS review |
| DevOps Lead | `@DevOps-Ariful-Islam` | CI/CD, infra, deployment |
| Health Programs | `@BGD-Health-Program` | Clinical content, country programs |

**PR Policy:** All changes via Pull Request. Minimum 1 owner review. CI must pass. No direct commits to `main`.


---

## MVP Acceptance Checklist

- [ ] All MVP files exist in repository with real content (not placeholders)
- [ ] CI pipeline passes on `main` branch
- [ ] No secrets, credentials, or PHI committed
- [ ] README.md reflects current state with setup instructions
- [ ] CODEOWNERS file present
- [ ] All MVP functional requirements verified manually or via automated tests
- [ ] Linked to `CATALOGS.md` and `TODO.md` in `zs-docs-platform`

---

*This document is the authoritative MVP specification for `zs-docs-camm`.*
*Changes require a Pull Request with at least 1 owner approval.*
