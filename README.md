# zs-docs-camm — Country Adoption Maturity Model

> **Repository:** https://github.com/zarishsphere/zs-docs-camm
> **Layer:** Governance (Layer 0) | **Catalog #:** 6
> **License:** Apache 2.0 | **Status:** Active

---

## What Is CAMM?

The **Country Adoption Maturity Model (CAMM)** is ZarishSphere's framework for guiding countries from initial interest to full digital health sovereignty.

It defines 6 levels (L0–L5), each with clear entry gates, exit criteria, checklists, and templates. A country cannot advance to the next level without meeting all exit criteria of the current level.

---

## Country Status Dashboard

| Country | Current Level | Status | Since |
|---------|--------------|--------|-------|
| 🇧🇩 Bangladesh | **L1 — Foundation** | 🟡 In Progress | 2026-03 |
| 🇮🇳 India | **L0 — Interest** | 🟡 MOU Pending | 2026-03 |
| 🇲🇲 Myanmar | **L0 — Interest** | 🔴 Outreach | 2026-03 |
| 🇵🇰 Pakistan | **L0 — Interest** | 🔴 Outreach | — |
| 🇹🇭 Thailand | **L0 — Interest** | 🔴 Outreach | — |

---

## CAMM Level Summary

| Level | Name | Key Milestone | Approximate Duration |
|-------|------|--------------|---------------------|
| L0 | Interest | Signed MOU | 1–3 months |
| L1 | Foundation | First facility live with real patient data | 3–6 months |
| L2 | Adoption | 10+ facilities, DHIS2 connected | 6–12 months |
| L3 | Integration | MOH bridges live, national systems integrated | 12–18 months |
| L4 | Maturity | National rollout, full EHR active | 18–36 months |
| L5 | Sovereignty | Country self-manages and contributes back | Ongoing |

---

## Repository Contents

```
zs-docs-camm/
├── README.md                      ← This file — country status + overview
├── LICENSE
├── model/
│   ├── CAMM-OVERVIEW.md           ← Full L0–L5 model description
│   ├── CAMM-L0-INTEREST.md        ← Level 0: Interest stage
│   ├── CAMM-L1-FOUNDATION.md      ← Level 1: Foundation stage
│   ├── CAMM-L2-ADOPTION.md        ← Level 2: Adoption stage
│   ├── CAMM-L3-INTEGRATION.md     ← Level 3: Integration stage
│   ├── CAMM-L4-MATURITY.md        ← Level 4: Maturity stage
│   └── CAMM-L5-SOVEREIGNTY.md     ← Level 5: Sovereignty stage
├── countries/
│   ├── BGD-STATUS.md              ← Bangladesh detailed status
│   ├── IND-STATUS.md              ← India detailed status
│   ├── MMR-STATUS.md              ← Myanmar detailed status
│   ├── PAK-STATUS.md              ← Pakistan detailed status
│   └── THA-STATUS.md              ← Thailand detailed status
├── templates/
│   ├── MOU-TEMPLATE.md            ← Memorandum of Understanding template
│   ├── NEEDS-ASSESSMENT.md        ← L0 needs assessment questionnaire
│   ├── TECHNICAL-READINESS.md     ← Technical readiness checklist
│   └── TRAINING-CURRICULUM.md     ← Training curriculum per CAMM level
└── governance/
    └── CAMM-GOVERNANCE.md         ← Who approves level promotions
```

---

## Owners

| Role | GitHub Handle | Responsibility |
|------|--------------|----------------|
| Platform Lead | `@arwa-zarish` | CAMM governance, level approvals |
| Health Programs | `@BGD-Health-Program` | Country-level implementation |
| Technical Lead | `@code-and-brain` | Technical readiness assessment |
