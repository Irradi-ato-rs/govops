# Security Policy — GovOps

This document defines **security reporting and handling** for the **Irradi.ato.rs GovOps**
repository.

The GovOps repository represents the **human and procedural governance authority layer**.
It does **not** contain enforcement logic, validators, or production workloads.

---

## 1. Scope

This security policy applies to:

- The `govops` repository
- Governance documentation and process artifacts
- GitHub Discussions and Issues within this repository
- Governance coordination tooling (non‑enforcing)

This policy does **not** apply to:

- Governance validation (see `rexce`)
- Enforcement or rollout tooling (see `Xcectua`)
- Governed reference behavior (see `Xentred`)
- Third‑party governed repositories

---

## 2. What Is a Security Issue

A security issue in the context of GovOps includes:

- Unauthorized access to governance coordination tooling
- Compromise of governance communication channels
- Credential or token exposure related to governance operations
- Malicious modification of governance authority artifacts
- Impersonation of governance authority
- Abuse of Discussions or Issues to misrepresent governance decisions

These issues affect **integrity and trust**, even if no code execution occurs.

---

## 3. What Is *Not* a Security Issue

The following are **not** security issues and must not be reported as such:

- Governance disagreements or disputes
- Interpretation questions
- Phase‑3 governance proposals
- Validation failures in other repositories
- Enforcement outcomes (`rexce/validate`)
- Policy dissatisfaction or requests for exception

These are **governance or process matters**, not security vulnerabilities.

---

## 4. Relationship to Enforcement

GovOps **does not enforce governance**.

Security handling in this repository **cannot**:

- Override validation results
- Grant enforcement exceptions
- Bypass required checks
- Modify governed repositories directly

All enforcement remains exclusively under **rexce** and GitHub native controls.

---

## 5. Reporting a Security Issue

Security issues related to GovOps must be reported **privately**.

Preferred channels:

- GitHub Private Security Advisory (if enabled)
- Designated security contact for Irradi‑ato‑rs GovOps

Do **not** open public Issues or Discussions for active security concerns.

---

## 6. Responsible Disclosure

Please allow reasonable time for:

- Triage
- Impact assessment
- Coordination with affected components
- Remediation planning

Public disclosure without coordination may undermine governance trust.

---

## 7. Governance Interaction

If remediation affects governance artifacts:

- Changes must occur via PR
- Changes must be reviewable
- Changes must respect Phase‑2 invariants
- No emergency bypasses are permitted

Security does **not** supersede governance process.

---

## 8. Audit Statement

This policy exists to ensure:

- Clear separation of security and governance concerns
- Protection of governance authority integrity
- Proper escalation paths
- Audit‑ready handling of security issues

---

**End of SECURITY policy.**
