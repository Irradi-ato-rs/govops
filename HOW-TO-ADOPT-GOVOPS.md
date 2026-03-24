# How to Adopt Irradi.ato.rs GovOps Governance#Adoption is **explicit**, **opt‑in**, **reviewable**, and **reversible**.

This repository (**govops**) documents the process.
**Adoption itself always occurs in the adopting repository.**

---

## 1. What Adoption Means

By adopting GovOps governance, a repository agrees that:

- **rexce** is the canonical governance validator
- Governance enforcement occurs via **GitHub‑native controls**
- Governance logic does **not** live in the adopting repository
- Governance evolution follows a **formal, evidence‑backed process**
- Human approval cannot bypass automated validation

This is **governance as a contract**, not a template or recommendation.

---

## 2. What Adoption Does *Not* Mean

Adoption does **not**:

- Transfer repository ownership
- Grant Irradi‑ato‑rs merge rights
- Provide legal or regulatory compliance guarantees
- Allow governance exceptions
- Apply enforcement automatically

All enforcement is **explicit and separate**.

---

## 3. Prerequisites

Before adopting, you should:

1. Review the **governed reference implementation**:
   - Xentred (reference behavior under enforcement)

2. Review the **governance adoption terms**:
   - `GOVERNANCE-ADOPTION.md` (published with Xentred)

3. Ensure your repository:
   - Uses pull requests for merges
   - Can support required status checks
   - Has maintainers authorized to approve governance adoption

---

This document describes the **only supported way** for a repository or organization to
**intentionally adopt** governance provided by the **Irradi‑ato‑rs GovOps system**.

## 5. The Adoption Act (Required)

Adoption occurs through **one explicit act**:

> **Opening and merging the standardized repo‑ready governance PR
> in your own repository.**

### The repo‑ready PR:

- Is identical across adopting repositories
- Adds the canonical `rexce/validate` workflow (SHA‑pinned)
- Adds non‑blocking Phase‑3 observability tooling
- Adds governance documentation
- Does **not** auto‑apply enforcement

### Important rules:

- The PR is opened **in your repository**
- The PR is reviewed **by your maintainers**
- The PR is merged **by your maintainers**
- The PR is **never** merged in `govops` or Xentred

The merge of this PR is the **formal ratification event**.

---

## 5. Applying Enforcement (Separate Step, this part of **Xcectua** will soon be ready)

After the adoption PR is merged, enforcement is applied **explicitly** via **Xcectua**.

This typically includes:

- Branch protection configuration
- Required status check registration:

rexce/validate
- Free‑tier fallback handling (if applicable)

Enforcement is:

- Deterministic
- Scripted
- Auditable
- Never implicit

---

## 6. Life After Adoption

Once adopted:

- All PRs are gated by `rexce/validate`
- Governance drift is visible via Phase‑3 tooling
- RER Doctor may emit warnings or violations (non‑blocking)
- Governance evolution requires formal proposals

---

## 7. Governance Evolution (Phase‑3)

To change governance behavior, you must provide:

- A Governance Change Proposal (GCP)
- Before and after governance diffs
- Evidence bundle or trace
- Review under canonical validation

No governance change is effective unless it passes validation.

---

## 8. Escalation and Clarification

For questions or clarification:

- Use **GitHub Discussions** in the `govops` repository
- Discussions are advisory and interpretive only
- Discussions do **not** approve changes or grant exceptions

If interpretation and enforcement differ:
- Enforcement prevails
- Governance must evolve formally

---

## 9. Exiting Governance

A repository may exit governance by:

1. Opening a PR removing governance artifacts
2. Classifying the change as governance removal
3. Providing rationale and evidence
4. Merging under existing enforcement

Exit is explicit and auditable.

---

## 10. Legal and Responsibility Notice

Governance documentation and tooling:

- Are provided “as is”
- Do not constitute legal advice
- Do not guarantee compliance

Legal terms and disclaimers are defined in the **GovOps DISCLAIMER**.

---

## Summary (One‑Line)

> **GovOps documents how governance is adopted; adoption itself always happens by an explicit PR in the adopting repository.**

---

**End of document.**
