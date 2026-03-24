## Authority and Escalation Boundary

- **GovOps** provides interpretation, clarification, and escalation.
- **Xentred** is the governed reference implementation.
- **rexce** is the sole validator and enforcement gate.

GovOps:
- May explain *why* governance behaves a certain way
- May recommend *how* governance should evolve
- May not override *what* enforcement does

Xentred:
- Demonstrates governance under real enforcement
- Evolves governance only via validated PRs
- Remains subject to `rexce/validate`

If interpretation and enforcement conflict:
- Enforcement prevails
- Governance must evolve formally
