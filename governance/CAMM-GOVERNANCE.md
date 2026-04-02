# CAMM Governance — Level Advancement Process

> **Document:** CAMM-GOVERNANCE.md | **Version:** 2.0.0

---

## Who Can Approve Level Advances?

| From → To | Approver Required |
|-----------|-----------------|
| L0 → L1 | `@arwa-zarish` + `@BGD-Health-Program` |
| L1 → L2 | `@arwa-zarish` |
| L2 → L3 | `@arwa-zarish` + `@code-and-brain` (technical verification) |
| L3 → L4 | All 4 owners (unanimous) |
| L4 → L5 | All 4 owners (unanimous) + community announcement |

---

## Evidence Requirements

For each level advance, the country team must provide evidence for each exit criterion:

- **Screenshots** of the running system showing real (anonymised) patient data
- **GitHub commit history** showing the distro and infra repos are active
- **Training records** (names and completion dates of trained staff)
- **Incident log** showing stability (or documented resolution of incidents)

---

## Process

1. Country focal point opens a GitHub Issue in `zs-docs-camm`
   - Title: `[ADVANCE] {COUNTRY} from L{N} to L{N+1}`
   - Body: evidence checklist with attached screenshots/links

2. `@BGD-Health-Program` reviews evidence within 5 business days

3. Required approvers review and comment

4. If approved: `@arwa-zarish` updates the country STATUS.md and closes the issue

5. If rejected: specific missing criteria are documented and country team has 60 days to address

---

## Dispute Resolution

If a country program disagrees with a level advancement decision, they may:
1. Open a new issue with additional evidence
2. Request a video call with the platform team
3. Escalate to all 4 owners for final decision (majority rules)
