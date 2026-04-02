# CAMM — Country Adoption Maturity Model Overview

> **Document:** CAMM-OVERVIEW.md | **Version:** 2.0.0
> **Updated:** 2026-03-24

---

## What Is CAMM?

CAMM is ZarishSphere's structured pathway for guiding countries from first contact to full digital health sovereignty. It prevents the common failure mode of "big bang" health IT implementation by breaking adoption into six incremental, achievable levels.

Each level has:
- **Entry gates** — what must already be true to start this level
- **Activities** — what work happens during this level
- **Exit criteria** — what must be verified before advancing
- **Deliverables** — concrete documents and systems produced

---

## The Six Levels

```
L0: Interest ──► L1: Foundation ──► L2: Adoption ──► L3: Integration ──► L4: Maturity ──► L5: Sovereignty
    MOU signed       1 facility live   10+ facilities   MOH bridges live    National rollout   Self-governed
    1–3 months       3–6 months        6–12 months      12–18 months        18–36 months       Ongoing
```

---

## Level Descriptions

### L0 — Interest
The country or program has expressed interest in ZarishSphere. An initial assessment has been done. A Memorandum of Understanding (MOU) has been signed.

**Who this is for:** Ministries of Health, NGOs, UN agencies, or donor-funded programs in the early evaluation phase.

### L1 — Foundation
A fork of the appropriate country distro exists. At least one real health facility is running ZarishSphere with real patient data. Core clinical modules (patient registration, encounter, vitals) are live.

**Who this is for:** Programs that have completed a pilot and have leadership buy-in.

### L2 — Adoption
10 or more facilities are running. The national DHIS2 instance is connected for aggregate reporting. Local staff can manage forms and basic configurations without ZarishSphere core team involvement.

**Who this is for:** Programs expanding beyond the pilot, typically with government co-ownership.

### L3 — Integration
National health system bridges are live (DHIS2, HL7v2 for labs, or ABDM for India). The Ministry of Health is an active partner. National codes and terminologies are loaded.

**Who this is for:** Programs with full government endorsement and national system connectivity.

### L4 — Maturity
Full national rollout across primary care. All EHR modules active. Public health surveillance feeding national EWARS. Donor reporting is automated.

**Who this is for:** National programs with full deployment and active use.

### L5 — Sovereignty
The country program self-manages all infrastructure. They have their own DevOps team. They contribute forms, protocols, and code back to the community. No longer dependent on ZarishSphere core team for operations.

**Who this is for:** Mature national programs that have internalised the platform.

---

## Level Advancement Process

1. Country team reviews exit criteria for current level
2. Country team opens a GitHub Issue in `zs-docs-camm` with evidence
3. `@BGD-Health-Program` reviews and verifies
4. `@arwa-zarish` approves the level advance
5. Country STATUS.md is updated
6. Celebration email sent to country team 🎉

---

## Why CAMM Matters

Without a structured adoption model:
- Countries get overwhelmed and abandon implementation
- Resources are wasted on features countries aren't ready for
- Core team cannot prioritise support effectively
- Donor reporting lacks a common framework for progress

CAMM gives everyone — country teams, donors, ZarishSphere owners — a shared language for progress.
