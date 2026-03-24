# GovOps — Irradi.ato.rs Governance Authority

This repository defines the **human and procedural governance authority** for the
Irradi‑ato‑rs GovOps system.

It documents **who governs**, **how governance decisions are handled**, and **how governance
questions are escalated**, without performing validation or enforcement itself.

---

## Role in the Governance System

GovOps occupies the **authority and interpretation layer** of the system.

| Component | Role |
|--------|-----|
| **rexce** | Canonical governance contract and validator (hard enforcement) |
| **Xcectua** | Governance orchestration and rollout |
| **Xentred** | Governed reference implementation |
| **GovOps (this repo)** | Human authority, interpretation, escalation |

GovOps **does not validate**, **does not enforce**, and **does not bypass** governance.

---

## What This Repository Is

This repository is used to:

- Define the governance mandate and scope
- Clarify governance intent and interpretation
- Provide escalation and discussion space
- Anchor the `@irradi-ato-rs/govops` GitHub team
- Support audit and external review

GitHub Discussions are enabled here for **clarification and deliberation only**.

---

## What This Repository Is Not

This repository is **not**:

- A validator (that is rexce)
- An enforcement mechanism (that is Xcectua + GitHub)
- A reference implementation (that is Xentred)
- A place to approve or merge governance changes

Governance changes **must** occur via PRs and must pass canonical validation.

---

## Relationship to Xentred

**Xentred** is the governed reference implementation where governance is proven under enforcement.

GovOps:
- Interprets governance intent
- Provides clarification and escalation
- Does **not** override Xentred behavior

Xentred:
- Demonstrates enforcement
- Evolves governance under rexce validation
- Remains the constitutional reference

---

## Discussions Policy

GitHub Discussions in this repository are used for:

- Governance clarification
- Adoption questions
- Pre‑GCP exploration
- Audit and compliance discussion

Discussions **do not approve**, **do not decide**, and **do not override** governance.

---

## Authority Statement

Governance authority is held by **Irradi.ato.rs GovOps**.

Enforcement authority is held **exclusively** by **rexce**.

---

**End of README.**
