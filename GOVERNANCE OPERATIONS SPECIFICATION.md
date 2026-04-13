# Governance Operations Specification
## Final v0.9

**Document Status:** Final Draft for Ratification
**Version:** 0.9
**Date:** April 2026
**Classification:** Public Release
**Document Authority:** This specification is self-authorising. It contains no references to external frameworks, standards bodies, or prior publications. Every term, formula, requirement, and definition within this document is defined by this document. Where formulas are used, they are expressed in the language of this specification and are not borrowed from any external source without ignoring the fact how governance capacity came about and made to be part of this document.

---

> **Purpose of this Document:** This specification defines a complete operational architecture for any entity that exercises governance authority over digital systems, human organisations, or critical infrastructure. It is designed to stand alone. An implementer who has read nothing else can implement this specification in full without consulting any other document.

---

## Table of Contents

1. Definitions and Language
2. The Governance Capacity Law
3. The Three Constitutional Conditions
4. Foundational Principles
5. Governance Architecture
6. The Governance Operations Centre
7. Operating Modes
8. The Threat Architecture
9. Reality Integrity
10. Continuous Adversarial Intelligence
11. Cryptographic Security
12. Formal Correctness
13. Governance Enforcement
14. Authority and Decision Structures
15. Identity and Access Governance
16. Data Sovereignty
17. Operational Disciplines
18. Human and Machine Authority
19. Observability
20. Federation
21. Compliance Mapping
22. Stakeholder Enforcement Capacity
23. Scalability and Maturity
24. Implementation Roadmap
25. Glossary

---

## 1. Definitions and Language

This section defines every term used in this specification. A term defined here has precisely the meaning given here and no other meaning within this document. Where a common word is given a specific technical meaning, that technical meaning governs throughout.

**Accountability:** The obligation of an authority holder to answer for the use of authority. Accountability cannot be transferred. The entity that authorises an action remains accountable for it regardless of who or what executes it.

**Adaptive Transparency:** The independently observed capacity of a governance system to detect changes in its environment and its own internal state, understand their implications, adapt its behaviour in response, and remain observable to those it governs throughout. One of the four components of Governance Capacity. See Section 2.

**Adversarial Observer:** An independent observer whose function is to actively seek to discover discrepancies, fabrications, or failures in the observations made by other observers. The adversarial observer does not accept the existing observation as correct — it attempts to disprove it.

**AI System:** Any automated system that uses machine learning, statistical inference, or similar computational techniques to generate outputs — including recommendations, analyses, detections, or proposed decisions — without direct human generation of each output.

**Authority:** The formally conferred right to take a defined class of action or make a defined class of decision within a governed system. Authority is always bounded. Authority to act in one domain does not imply authority to act in any other.

**Bounded Capability:** The operational scope assigned to an AI system within which it may act autonomously. All AI system activity must remain within its Bounded Capability. Any action outside Bounded Capability requires human approval before execution.

**Capacity to Act:** The independently observed structural ability of the governance system to make decisions, enforce them, and produce observable effects on the governed system. One of the four components of Governance Capacity. See Section 2.

**Certification Hash:** A cryptographic digest of a governance record, produced by a defined algorithm, enabling subsequent verification that the record has not been altered. All governance records subject to this specification must carry Certification Hashes.

**Constitutional Condition:** One of three requirements defined in Section 3 that must hold at all times for a governed system to be considered governed. Violation of any Constitutional Condition is a governance failure regardless of all other measures.

**Continuous Adversarial Intelligence:** The function of continuously operating adversarial AI analysis against the governance system's own infrastructure, seeking vulnerabilities before adversaries find them. Defined in Section 10.

**Continuous Governance Assurance:** The state in which compliance with governance requirements is verified in real time through automated mechanisms, not through periodic review. Periodic review supplements but does not substitute for Continuous Governance Assurance.

**Controlled Execution:** The state in which an AI system executes actions only within its approved Bounded Capability, every action is logged before completion, and a human authority can halt, modify, or reverse execution at any point.

**Crisis State:** The operating condition that activates when Governance Capacity falls below the Governance Risk Level. Defined in Section 7.3.

**Cryptographic Provenance:** A chain of Certification Hashes and digital signatures establishing the origin, integrity, and authenticity of a governance record, telemetry input, or software component. Any record, input, or component without verifiable Cryptographic Provenance is treated as untrusted.

**Data Residency:** The requirement that governed data be stored and processed within boundaries explicitly defined by the governing entity.

**Data Sovereignty:** The principle that governed data is subject to the authority of the governing entity that created or collected it. Data Sovereignty is the default condition. Any departure requires explicit authorisation.

**Decision Contract:** The minimum information record that must accompany every governance decision. Contents defined in Section 14.4. A decision without a complete Decision Contract is not a valid governance decision.

**Delegation:** The transfer of authority to act within a defined scope to a subordinate actor or system, while retaining accountability for all actions taken under that authority.

**Disagreement Condition:** The state that exists when two or more independent observers produce materially different assessments of the same governance reality. When the Disagreement Condition exists, the Governance Risk Level increases and no decision based on the contested observation is valid until the disagreement is resolved.

**External Observer:** An observer that operates independently of the governance system's own infrastructure, is not funded or directed by the governed entity, and whose observations the governed entity cannot suppress or modify.

**Fidelity:** The independently observed degree to which the governance system acts in the interests of those it governs. Fidelity is not a stated commitment — it is a measured condition. One of the four components of Governance Capacity. See Section 2.

**Formal Verification:** The application of mathematical proof techniques to demonstrate that software or system behaviour satisfies a defined specification under all possible inputs and conditions. Formal Verification provides guarantees that testing alone cannot.

**Governance Capacity:** The total independently observed governance capability of a system — its ability to maintain authority, accountability, adaptability, and fidelity simultaneously under risk. Defined formally in Section 2.

**Governance Failure:** The condition in which any Constitutional Condition is violated, regardless of the values of any other governance measures.

**Governance Operations Centre:** The operational brain of this specification's governance architecture. The mandatory runtime mechanism through which governance is exercised continuously rather than periodically. Defined in Section 6.

**Governance Record:** Any document, log entry, decision, telemetry reading, or other information that is required by this specification to be created, retained, and made available to oversight.

**Governance Risk Level:** The aggregate, time-varying measure of all forces threatening the stability and continuity of the governed system. The Governance Risk Level always tends to increase in the absence of active governance effort. See Section 2.4.

**Governing Entity:** Any entity that exercises formal authority over the decisions, resources, rights, or interests of others, whether through legal mandate, contractual authority, institutional position, or practical control.

**Human Authority:** The right of a designated human to make final governance decisions, override AI system outputs, halt or reverse execution, and exercise sovereign control over any function of the governance system.

**Identity Assurance Level:** A defined degree of confidence that an actor is who they assert they are, expressed on a graduated four-level scale defined in Section 15.1.

**Immutable Ledger:** A governance record store designed so that once a record is written, it cannot be modified or deleted by any actor within the governance system, including administrators.

**Independent Observation:** Observation and measurement conducted by a process that is structurally separate from the actors whose governance it measures, whose independence is itself independently verifiable, and whose findings cannot be modified or suppressed by the measured actors.

**Institutional Integrity:** The independently observed degree to which structures, constraints, norms, and processes preserve, stabilise, and protect governance actors and the governed system. One of the four components of Governance Capacity. See Section 2.

**Internal Observer:** An observer that operates within the governance system's own infrastructure. An Internal Observer is necessary but insufficient alone — its observations must be corroborated by an External Observer and an Adversarial Observer.

**Minimum Viability Floor:** The lowest value of any Governance Capacity component below which the component is treated as structurally absent. When any component falls below the Minimum Viability Floor, Governance Capacity is zero regardless of the values of other components. Each governing entity defines its Minimum Viability Floor based on scale, risk profile, and operational context.

**Multi-Observer Verification:** The process of collecting observations of the same governance reality from three independent observer types — Internal, External, and Adversarial — simultaneously and comparing them for consistency.

**Normal State:** The operating condition when Governance Capacity substantially exceeds the Governance Risk Level. Defined in Section 7.1.

**Oversight Body:** An independent body with authority to investigate, declare, and require remedy of governance failures. The Oversight Body must be structurally independent of the Governing Entity it oversees.

**Post-Quantum Cryptography:** Cryptographic algorithms designed to resist attacks by sufficiently capable automated reasoning systems, including systems that can solve problems that defeat conventional public-key cryptography. Required for all governance-critical cryptographic applications under this specification.

**Principal Officer:** Any individual who exercises governance authority on behalf of a Governing Entity, including executives, directors, appointed officials, and delegated decision-makers.

**Reality Integrity Protocol:** The sub-system within the Governance Operations Centre that validates the authenticity and integrity of all observations before they are processed. Defined in Section 9.

**Response Cascade:** The four-phase governance recovery process that activates when the governed system enters Crisis State. Defined in Section 7.4.

**Rollback Capability:** The ability to reverse a deployed change and restore the prior state of a governed system.

**Self-Declared Value:** A measurement of any governance component produced by the entity whose governance is being measured, without independent corroboration. Self-Declared Values are not valid inputs to the Governance Capacity calculation. They are evidence of potential governance failure.

**Software Bill of Provenance:** A complete, cryptographically signed inventory of every component, dependency, library, and toolchain element used to build a software artefact, enabling independent verification of the artefact's composition.

**Sovereign Decision:** Any governance decision that materially affects the rights, resources, or welfare of those the Governing Entity governs. All Sovereign Decisions require Human Authority approval.

**Stakeholder:** Any person, entity, or group whose rights, interests, or welfare are materially affected by the decisions of a Governing Entity.

**Stress State:** The operating condition when Governance Capacity approaches the Governance Risk Level. Defined in Section 7.2.

**Three-Observer Rule:** The requirement that all governance-critical observations be produced simultaneously by three structurally independent observer types. Defined in Section 19.3.

**Verified Reality:** The state of knowledge about a governed system that has been confirmed through Multi-Observer Verification with no Disagreement Condition. Decisions may only be based on Verified Reality.

**Zero-Trust Architecture:** A security design principle requiring that no actor, system, or network connection is trusted by default, regardless of location or prior authorisation. Every access request is verified independently.

---

## 2. The Governance Capacity Law

### 2.1 The Foundational Statement

The governance capacity of any governed system can be expressed as a relationship between four independently observed properties of that system. This relationship is a law of governance — not a recommendation, framework, or guideline — because it describes the structural conditions under which governance either exists or does not.

The four properties are:

**Fidelity** — the independently observed degree to which the governance system acts in the interests of those it governs.

**Capacity to Act** — the independently observed structural ability to make decisions and produce real effects.

**Institutional Integrity** — the independently observed degree to which structures and constraints genuinely govern those who exercise authority.

**Adaptive Transparency** — the independently observed capacity to detect, understand, and respond to changes in the governed environment and the governance system itself.

### 2.2 The Governance Capacity Formula

Governance Capacity is the product of all four independently observed components:

```
Governance Capacity  =  Fidelity(observed)
                     ×  Capacity to Act(observed)
                     ×  Institutional Integrity(observed)
                     ×  Adaptive Transparency(observed)
```

The use of multiplication — not addition — is the most important structural property of this formula. It means:

**Zero in any component produces zero total Governance Capacity**, regardless of the strength of all other components. A governance system with no Institutional Integrity has zero Governance Capacity even if it has absolute Fidelity, maximum Capacity to Act, and perfect Adaptive Transparency. A governance system with zero Fidelity has zero Governance Capacity even if every other component is at maximum.

This is not a mathematical convenience. It reflects an observable truth about governance: a governance system missing any one of the four properties is not a diminished governance system. It is not a governance system at all.

**The components cannot substitute for each other.** Exceptional Capacity to Act does not compensate for absent Institutional Integrity. Perfect Adaptive Transparency does not compensate for zero Fidelity. Each component is a co-requirement — all four must be present simultaneously.

**The weakest component determines the operational ceiling.** When components have significantly different values, the product is dominated by the smallest. A governance system with Fidelity = 0.9, Capacity to Act = 0.8, Institutional Integrity = 0.1, and Adaptive Transparency = 0.85 has effective Governance Capacity close to 0.1, regardless of the strength of the other three. This is the Weakest-Link Property. It defines the governance investment priority: address the weakest component first. Strengthening strong components while a weak component remains unaddressed produces negligible improvement in total Governance Capacity.

### 2.3 The Sustainability Condition

For a governed system to remain governed, its Governance Capacity must exceed its Governance Risk Level at all times:

```
Governance Capacity(at time T)  >  Governance Risk Level(at time T)
```

This condition must hold continuously. It is not satisfied by a historical calculation or a periodic assessment. A system that achieved Governance Capacity greater than Governance Risk Level at a past point in time is not thereby governed at a current point in time.

### 2.4 The Entropic Risk Property

The Governance Risk Level always tends to increase in the absence of active governance effort:

```
Rate of change of Governance Risk Level  ≥  0
(in the absence of active governance investment)
```

This is the Entropic Risk Property. It establishes that:

**Governance is an anti-entropic activity.** A governed system that is not actively maintained is a governed system in which the Governance Risk Level is increasing while Governance Capacity holds constant or declines. Governance complacency is not neutral. It is active decline.

**Stability is an achievement, not a default state.** Governed systems do not naturally tend toward stability. They tend toward disorder, capture, and failure. Sustained governance is the continuous investment that resists this tendency.

**The Sustainability Condition must be actively maintained, not periodically verified.** A governance system that checks compliance once per year and does nothing in between is a governance system in which the Governance Risk Level may have grown to exceed Governance Capacity before the next check occurs.

### 2.5 The Observation Condition

All four components of the Governance Capacity formula must be Independently Observed to be valid inputs. Self-Declared Values are not valid.

A governance system cannot determine its own Governance Capacity. It can only create conditions under which its Governance Capacity can be determined by independent observers. When a governance system reports its own Governance Capacity, that report is a governance claim — an input to the Independent Observation process, not a substitute for it.

This has one critical consequence: **a governance system that has not established independent observation infrastructure for each of the four components has Governance Capacity of zero by definition.** Not because the components are necessarily absent — but because without independent observation, their values are unknown and therefore must be treated as zero.

### 2.6 The Cascade Property

When Adaptive Transparency degrades, the degradation tends to propagate through the other components in sequence:

```
Adaptive Transparency degrades
    →  Institutional Integrity begins to erode
         (the governance system cannot detect the erosion)
    →  Capacity to Act becomes misdirected
         (actions are based on false or stale information)
    →  Fidelity degrades
         (the governance system drifts from serving those it governs
          without detecting the drift)
```

This cascade is not merely correlational. It has a causal mechanism: Adaptive Transparency is the component through which the governance system receives information about its own state. When it degrades, the governance system loses the ability to detect that other components are failing. The degradation of the other components then proceeds undetected and uncorrected.

The Cascade Property establishes that Adaptive Transparency has a special structural role: it is the first link in the governance feedback loop, and its failure initiates cascading failure in all other components. Investment in Adaptive Transparency — particularly in its independence, speed, and coverage — is therefore the highest-leverage governance investment in any system where overall Governance Capacity is below the target level.

### 2.7 The Scale Limit Property

The maximum complexity of a governed system is proportional to the independently observed Adaptive Transparency of the Governing Entity:

```
Maximum sustainable governance scope  ∝  Independently Observed Adaptive Transparency
```

A governance system that expands its scope without expanding its independent observation capability is accumulating Governance Risk Level faster than it can respond. Scope expansion without proportional Adaptive Transparency expansion is a governance failure in formation, not merely a risk to be managed.

---

## 3. The Three Constitutional Conditions

The following three conditions are constitutional requirements binding on all implementations of this specification. They must hold at all times. Violation of any Constitutional Condition is a governance failure that cannot be offset by the values of any other measures.

### Constitutional Condition I — The Existence Condition

```
Governance exists if and only if Governance Capacity exceeds
the Governance Risk Level as independently observed.

Governance Capacity ≤ Governance Risk Level  means governance has failed.
```

A governed system that does not maintain Governance Capacity greater than Governance Risk Level as independently observed is not a governed system experiencing difficulty. It is a system that is not governed. This condition is monitored continuously. There is no partial compliance — the condition holds or governance does not exist.

### Constitutional Condition II — The Human Sovereignty Condition

```
No automated system holds, exercises, or is delegated Sovereign Decision authority.

All Sovereign Decisions require Human Authority approval.

Automated systems operate as bounded tools within Capacity to Act.
They are never constitutive of Capacity to Act, Institutional Integrity,
Adaptive Transparency, or Fidelity as independent governance actors.
```

This condition cannot be waived by any authority at any tier. A governance system that allows automated systems to make Sovereign Decisions has violated this condition regardless of how capable, accurate, or efficient those systems are. The Human Sovereignty Condition is not a performance limitation on automated systems. It is a structural requirement of governance.

A governance system that cannot function without automated systems has, by design, transferred Sovereign Decision authority to those systems. This violates the Human Sovereignty Condition. All governance systems must maintain the operational capability to govern without any automated system. This is a design requirement, not a contingency plan.

### Constitutional Condition III — The Verified Reality Condition

```
No governance decision is valid unless the reality on which it is based
has been confirmed through Multi-Observer Verification with no Disagreement Condition.

Where independent observers disagree, the Governance Risk Level increases.
No decision based on contested observation is valid until the disagreement is resolved.
```

A governance system that makes decisions based on Self-Declared Values or unverified observations is not making governance decisions. It is making unaccountable assertions. The Verified Reality Condition operationalises the distinction: governance requires independently verified knowledge, not asserted knowledge.

The Disagreement Condition increases the Governance Risk Level because disagreement between independent observers is itself information: it indicates that the governance system's understanding of its own state or environment is unreliable. Unreliable understanding is the beginning of Adaptive Transparency failure. It must therefore be treated as a risk increase, not as an observation conflict to be averaged or adjudicated away.

---

## 4. Foundational Principles

The following principles apply universally across all implementations. They cannot be waived, modified, or derogated by any authority within the governed system.

### 4.1 Governance-Native Design
Governance requirements are embedded into system design from the beginning. They are not compliance layers added after implementation.

### 4.2 Stakeholder Trust as the Primary Obligation
The governance system exists to serve the interests and rights of those it governs. Where operational efficiency and stakeholder trust conflict, stakeholder trust governs. This is not aspirational — it is the definition of the Fidelity component in the Governance Capacity formula.

### 4.3 Accountability Without Exception
Every action taken within the governed system must be attributable, auditable, and reviewable by authorised oversight. This includes all automated actions. Accountability for automated actions rests with the human authority that authorised the automated system's Bounded Capability.

### 4.4 Authority Boundaries
Every actor — human or automated — operates within defined authority boundaries. Actions outside those boundaries are not governance decisions; they are violations.

### 4.5 Security as a Structural Requirement
Security controls are governance requirements, not technical choices. Security failures are governance failures. The threat architecture of Section 8 defines the minimum security requirements that all implementations must meet.

### 4.6 Interoperability Without Capture
Systems support interoperability through openly documented interfaces while maintaining the operational independence required to govern effectively.

### 4.7 Least Privilege
Every actor receives only the minimum access and authority necessary to perform its authorised function. Elevated access is time-limited and subject to review.

### 4.8 Modular Scalability
This specification applies from small operational teams to global federated environments without requiring architectural redesign. The Minimum Viability Floor and Governance Operations Centre architecture scale to context.

### 4.9 Sovereignty by Default
Governed data, processes, and infrastructure are subject to the authority of the Governing Entity by default. Any departure from this default requires explicit authorisation from an authority with standing to grant it.

### 4.10 Continuous Governance
Governance is a continuous operational condition, not a periodic audit state. Continuous Governance Assurance is the mechanism by which this principle is operationalised.

### 4.11 Verified Reality
No governance decision is valid without Verified Reality. Where independent observers disagree, the Governance Risk Level increases and decisions based on the contested observation are suspended until the disagreement is resolved.

### 4.12 Human Sovereignty
Automated systems are tools. Human authorities make Sovereign Decisions. A governance system that cannot function without automated systems is not a governance system under this specification — it is a system that has transferred Human Sovereignty to machines.

---

## 5. Governance Architecture

This specification defines a three-layer architecture in which the governance function is the superordinate layer.

```
┌──────────────────────────────────────────────────────────────────┐
│                     GOVERNANCE LAYER                              │
│  Authority · Fidelity · Accountability · Oversight               │
│  [ Expressed operationally through the GOC — Section 6 ]        │
├──────────────────────────────────────────────────────────────────┤
│                    INTEGRATION LAYER                              │
│  Identity · Interoperability · Telemetry · Standards             │
├────────┬────────┬────────┬────────┬────────┬────────────────────┤
│Delivery│Security│Config  │Finance │AI Ops  │ + Operational Svc  │
│               OPERATIONAL DISCIPLINES LAYER                      │
└──────────────────────────────────────────────────────────────────┘
```

### 5.1 The Governance Layer

The Governance Layer defines authority, Fidelity obligations, accountability structures, and oversight. It is the only layer with the authority to define what the layers beneath it may do. It is expressed operationally through the Governance Operations Centre defined in Section 6.

The Governance Layer is never passive. It continuously monitors, enforces, and reports across all lower layers. A Governance Layer that operates only at defined intervals, or only when problems are reported to it, is not functioning as a Governance Layer under this specification.

### 5.2 The Integration Layer

The Integration Layer provides the coordination mechanisms that allow operational disciplines to function coherently. It maintains shared identity frameworks, interoperability standards, data exchange protocols, and telemetry aggregation. It enforces Governance Layer requirements across all operational disciplines simultaneously.

### 5.3 The Operational Disciplines Layer

The Operational Disciplines Layer delivers technical capability within governance constraints. Each discipline operates independently within its domain but must comply with all requirements of the Governance Layer and Integration Layer. Discipline boundaries define responsibility, not isolation — disciplines share observability infrastructure, identity frameworks, and compliance enforcement.

---

## 6. The Governance Operations Centre

The Governance Operations Centre — hereafter the Centre — is the operational brain of this specification. It is the mandatory runtime expression of the Governance Layer: the mechanism through which governance moves from defined requirement to continuous operational reality.

```
Centre  =  Human Authority  +  Bounded AI Capability  +  Verified Reality
```

The Centre is required at Tier 2 and above as defined in Section 23. At Tier 1, a Centre function of equivalent logical structure must exist, scaled to context. No Governing Entity subject to this specification operates without a functioning Centre.

### 6.1 The Six-Layer Architecture

The Centre operates through six functional layers forming a closed-loop system:

```
Sense  →  Verify  →  Think  →  Decide  →  Act  →  Memory
  ↑                                                    │
  └────────────────────────────────────────────────────┘
                      (closed loop)
```

#### Layer 1 — Sense: Reality Intake

The Sense Layer is the Centre's primary interface with reality. It receives:

- Operational telemetry from all ten disciplines across all governed systems
- Economic, financial, and resource indicators
- Legal, regulatory, and policy signals
- Stakeholder feedback — treated as a primary governance signal, not secondary noise, because it is the primary source of independent evidence about Fidelity
- Adversarial signals: external threat intelligence, attack indicators, and anomaly patterns
- Independently observed Governance Capacity component measurements

The Sense Layer passes all inputs through the Reality Integrity Protocol defined in Section 9 before forwarding them to the Verify Layer. Any input that fails Reality Integrity validation is quarantined, logged, and treated as a potential Governance Risk Level increase.

The Sense Layer must be structurally independent of the systems it observes. An observation system that is part of the system it monitors is a self-reporting system, not a Sense Layer. Self-reporting violates the Observation Condition of Section 2.5.

**AI systems in the Sense Layer:** Primary function for data collection, pattern detection, signal fusion, and early-warning analysis. AI systems in the Sense Layer operate within Bounded Capability for sensing functions only.

**Human authority in the Sense Layer:** Audit and validation of AI-generated signal assessments. Calibration of sensing parameters. Authorisation of Governance Risk Level adjustments based on Sense Layer findings.

#### Layer 2 — Verify: Truth Construction

The Verify Layer implements the Three-Observer Rule. Its function is to construct Verified Reality from multiple independent sources, not merely to aggregate observations.

The verification process:

1. Internal, External, and Adversarial observations are received simultaneously for each governance-critical measurement
2. Observations are compared for consistency against defined tolerance parameters
3. Where consistent: Verified Reality is confirmed, the Certification Hash of the verification is recorded, and the verified state passes to the Think Layer
4. Where inconsistent: the Disagreement Condition activates — the Governance Risk Level is increased, the inconsistency is escalated for investigation, and no decision based on the contested observation is valid until resolution is confirmed

The Verify Layer is the operational implementation of the Observation Condition (Section 2.5). It is the structural mechanism by which Self-Declared Values are excluded from governance decisions.

**AI systems in the Verify Layer:** Cross-validation of observations. Detection of fabricated, manipulated, or AI-generated synthetic telemetry. Identification of systematic bias in observation streams. All AI observations in this layer are themselves subject to Adversarial Observer review.

**Human authority in the Verify Layer:** Validation of verification conclusions. Approval of Disagreement Condition findings. Authorisation of Governance Risk Level adjustments.

#### Layer 3 — Think: Decision Intelligence

The Think Layer processes Verified Reality to produce governance intelligence for human review. It does not produce governance decisions — it produces decision proposals that require Human Authority approval.

The Think Layer contains:

- **Policy Engine:** Applies governance policy to Verified Reality, identifying applicable requirements and options
- **Risk Engine:** Computes current Governance Capacity and Governance Risk Level from Independently Observed component values; produces the margin assessment and trend analysis
- **Scenario Modeller:** Generates structured projections of alternative courses of action, with independently assessed probability distributions of consequences across defined time horizons
- **Threat Analyser:** Receives inputs from the Continuous Adversarial Intelligence function (Section 10) and integrates active threat intelligence with decision proposals

Outputs of the Think Layer are Decision Proposals — structured packages that include the options considered, the risk assessment for each option, reversibility classifications, and the minimum Decision Contract fields required for the Decide Layer to approve them.

**AI systems in the Think Layer:** Primary function for scenario modelling, risk computation, threat analysis, and option generation. AI systems produce Decision Proposals. They do not produce governance decisions.

**Human authority in the Think Layer:** Review and challenge of AI projections. Authorisation to elevate a Decision Proposal to the Decide Layer. Authority to reject a Decision Proposal and require revised analysis.

#### Layer 4 — Decide: Sovereign Gate

The Decide Layer is the most critical layer in the Centre. It is the point at which Human Authority is exercised. It is the structural enforcement point for Constitutional Condition II.

Rules binding on the Decide Layer without exception:

- Automated systems do not execute irreversible governance actions
- Human Authority approval is required for all Sovereign Decisions
- All decisions must be accompanied by a complete Decision Contract (Section 14.4)
- No decision may be based on unverified reality — Constitutional Condition III applies
- The Decide Layer has absolute authority to override any AI system output
- All approvals are recorded in the Immutable Ledger with the identity of the approving authority, the timestamp, and the full Decision Contract

The Decide Layer operates the Human Authority Gateway which verifies: the identity of the approving authority at Identity Assurance Level 4 (defined in Section 15.1); the legal authority of the approving authority to make the specific decision; and the completeness of the Decision Contract.

**AI systems in the Decide Layer:** Automated systems may propose decisions and present Decision Contracts. They may flag procedural deficiencies in proposed decisions. They may not approve, authorise, or execute Sovereign Decisions.

**Human authority in the Decide Layer:** Sole valid source of governance decision approvals. Absolute override authority over all AI system outputs at any Centre layer.

#### Layer 5 — Act: Controlled Execution

The Act Layer executes governance decisions approved by the Decide Layer. All execution is:

- **Bounded:** The executed action operates only within the approved scope of the corresponding Decision Contract
- **Logged:** Every action is recorded in the Immutable Ledger before completion, not after
- **Reversible where technically feasible:** The Act Layer maintains Rollback Capability for all approved decision types where rollback is technically possible
- **Monitored:** The consequences of all executed actions are fed back to the Sense Layer, closing the control loop

**AI systems in the Act Layer:** Coordinated execution of complex multi-system governance actions within Bounded Capability. All AI execution in the Act Layer is Controlled Execution.

**Human authority in the Act Layer:** Sovereign control — the authority to halt, modify, or reverse execution at any point, without prior notice to the AI system executing the action.

#### Layer 6 — Memory: Institutional Record

The Memory Layer is the governance system's Immutable Ledger. It maintains:

- A cryptographically protected record of all governance decisions with their complete Decision Contracts
- Complete audit trails of all Centre layer operations, including all AI system outputs and human authority decisions
- Institutional knowledge: accumulated learning from governance decisions and their outcomes, used to improve future Decision Proposals
- Succession data: all information necessary to maintain Fidelity continuity when governance authority transfers between actors or entities

The Memory Layer satisfies the requirement that Fidelity be maintained across transitions in governance personnel. Governance purpose and rationale are preserved in the Memory Layer independently of the actors who created them.

### 6.2 Centre Formal Properties

The Centre must satisfy the following properties at all times:

**No silent failure:** Every failure in any Centre layer is detected, logged in the Memory Layer, and escalated to the oversight function. There is no condition in which the Centre continues to operate while concealing its own failures.

**No unilateral automated control:** No Centre layer produces governance outcomes without Human Authority approval at the Decide Layer.

**No unobserved state:** Every system within the scope of the Governing Entity's authority is within the Sense Layer's observational coverage. A system that cannot be observed by the Centre is a governance gap and is treated as an immediate Governance Risk Level increase.

### 6.3 Centre Deployment

**Architecture:** Centralised command function with distributed observation nodes. The centralised command function ensures governance coherence. Distributed nodes ensure complete coverage of the governed scope.

**Redundancy:** Multiple independent sites at Tier 3 and above. Single site with documented recovery procedures at Tier 2. Logical Centre function at Tier 1.

**Human staffing:** Continuously staffed human governance operators at Tier 3 and above. Defined availability and response times at Tier 1 and 2.

**Communication security:** All Centre communications protected by Post-Quantum Cryptography as defined in Section 11. All communications authenticated and logged.

### 6.4 Centre Performance Requirements

| Measure | Tier 1 | Tier 2 | Tier 3 | Tier 4 |
|---|---|---|---|---|
| Governance Capacity computation | On demand | < 60 seconds | < 5 seconds | < 1 second |
| Observation intake latency | Defined | < 30 seconds | < 5 seconds | < 500 milliseconds |
| Decision approval cycle | Defined | < 5 minutes | < 2 minutes | < 2 seconds for AI proposals |
| Threat detection | Manual trigger | Automated | Real-time | Real-time |
| Observer verification cycle | Defined | Per decision | Continuous | Continuous |

---

## 7. Operating Modes

The Governing Entity's operational posture responds to the real-time relationship between Governance Capacity and Governance Risk Level. Three operating modes are defined. Transitions between modes are triggered automatically by the Risk Engine and confirmed by Human Authority.

### 7.1 Normal State

**Trigger:** Governance Capacity substantially exceeds the Governance Risk Level — a comfortable positive margin

**System behaviour:**
- AI systems assist in all Centre layers within Bounded Capability
- Human authorities supervise and maintain oversight
- Standard decision approval workflow applies
- Continuous optimisation of governance effectiveness
- Full Controlled Execution permitted within approved Bounded Capabilities

**Obligations:** All three Constitutional Conditions apply in Normal State. Normal State does not reduce governance obligations — it reduces the intensity of human involvement required to meet them. The governing entity uses Normal State to strengthen governance components, reduce the Governance Risk Level, and improve institutional resilience.

### 7.2 Stress State

**Trigger:** Governance Capacity approaches the Governance Risk Level — the Sustainability Condition is at risk but not yet violated

**System behaviour:**
- Increased verification frequency — the Verify Layer operates at elevated checking cycles
- Restricted automation — AI proposals require enhanced Human Authority review before execution
- Heightened human involvement in all Decide Layer functions
- Risk Engine operates continuous scenario projections
- Stakeholder telemetry elevated to primary monitoring priority
- All non-essential changes to governance systems suspended pending investigation

**Obligations:** The Governing Entity must investigate the source of the margin reduction and present a remediation plan to the Oversight Body within a defined period. Stress State that persists beyond this period without an approved remediation plan is treated as an approaching governance failure.

**Structural significance:** Stress State is the most important operating mode for preventing governance collapse. It is where early intervention is most effective. A Governing Entity that detects Stress State and acts decisively can prevent Crisis State. A Governing Entity that does not detect Stress State — because its Adaptive Transparency is insufficient — will typically discover it has been in Stress State only when it has already entered Crisis State. This is the Cascade Property in operation.

### 7.3 Crisis State

**Trigger:** Governance Capacity falls below the Governance Risk Level — Constitutional Condition I is violated

**System behaviour:**
- Response Cascade immediately activates (Section 7.4)
- All autonomous AI execution suspended — Human Authority required for every action
- Only governance-critical operations continue
- Sovereign override enabled — designated Human Authority has direct override capability
- External escalation activates — the Oversight Body and, where applicable, the External Escalation Pathway (Section 22.5) are notified
- All stakeholder enforcement capacity measures activate (Section 22)

**Obligations:** Crisis State intensifies governance obligations. It does not reduce them. The Governing Entity must notify the Oversight Body immediately. The Governing Entity cannot conceal Crisis State. The declaration of Crisis State is public.

**Critical rule:** A Governing Entity that invokes emergency circumstances, exceptional conditions, or operational necessity as justification for reduced governance during Crisis State has not identified a valid reason to reduce governance. It has identified a condition requiring greater governance effort. The Governance Risk Level is higher in emergency conditions, not lower. Therefore Governance Capacity must be higher, not lower.

### 7.4 Response Cascade

The Response Cascade activates automatically when Crisis State is declared. It proceeds through four phases. Phases 1 through 3 address the immediate condition. Phase 4 is mandatory — a Governing Entity that completes Phases 1 through 3 without completing Phase 4 has not resolved the Crisis State. It has deferred it.

**Phase 1 — Declaration:** All Stakeholders and oversight bodies are notified. The Governance Capacity less-than Governance Risk Level condition is declared publicly. No concealment of this condition is permitted. All Governance Capacity component values, as independently observed, are published.

**Phase 2 — Correction:** Immediate actions to restore Governance Capacity above the Governance Risk Level are identified by the Think Layer, approved by Human Authority, and executed within the shortest feasible period. Correction focuses on the lowest-value Governance Capacity component — the weakest-link component identified by the Weakest-Link Property of Section 2.2.

**Phase 3 — Containment:** Actions to prevent the Governance Risk Level from growing further while correction is underway. Includes scope restrictions, suspension of expansion activities, and stabilisation measures.

**Phase 4 — Reconstruction:** Structural restoration of the conditions that allowed Governance Capacity to fall below the Governance Risk Level. Reconstruction addresses the structural cause of the failure, not its surface manifestation. The structural cause is always one of: Fidelity decay, Capacity to Act failure, Institutional Integrity erosion, or Adaptive Transparency degradation. Reconstruction must demonstrate, through Independent Observation, that the structural cause has been addressed and the component in question has been restored above the Minimum Viability Floor.

---

## 8. The Threat Architecture

### 8.1 The Primary Threat Class: Automated Adversaries

This specification is designed for a threat environment in which the most capable adversaries operate at machine speed, with automated reasoning capabilities that can discover and exploit vulnerabilities faster than human-speed defences can respond.

The primary threat class consists of adversaries who:

- Autonomously discover zero-day vulnerabilities in production systems without prior knowledge of those specific systems
- Construct working exploits from publicly known vulnerability identifiers within hours, without human intervention
- Chain multiple vulnerabilities together into sophisticated exploit sequences
- Operate at a cost and scale that makes targeted attacks available to a much wider range of adversaries than previously
- Can defeat friction-based security controls — any security measure whose value derives from making attack tedious rather than impossible is not a valid primary defence under this specification

**Critical architectural consequence:** Every security requirement in this specification is designed to provide hard barriers, not friction. A security control that slows an adversary operating at machine speed is not a valid primary defence. All security requirements must impose structural barriers that cannot be bypassed by automation.

### 8.2 Specific Threat Categories

**AI-Native Adversaries:** Automated systems with advanced reasoning capabilities operating autonomously against governance infrastructure. These adversaries can systematically analyse any observable interface, identify vulnerabilities through pattern recognition across vast codebases, and construct working exploits without human involvement.

**Coordinated Multi-Node Deception:** Simultaneous manipulation of multiple observation inputs to create a false picture of governed reality. This attack exploits systems that rely on a small number of observation sources, or that aggregate observations without adequate independent verification. The Three-Observer Rule and Reality Integrity Protocol of Sections 9 and 19.3 are the primary defences.

**Reality Fabrication:** Generation of synthetic telemetry, logs, metrics, and observation data that appears authentic but represents a false state of the governed system. Reality fabrication attacks are designed to defeat conventional anomaly detection by generating statistically normal data that nonetheless does not represent reality. The Cryptographic Provenance requirement of Section 9 is the primary defence.

**Cross-Federation Manipulation:** Exploitation of trust relationships between federated entities to use one entity's compromise as a pathway to attack another. An entity that trusts another entity's governance signals without independent verification is vulnerable to this attack through the trusted entity.

**Model Poisoning and Replacement:** Attacks on AI systems operating within the Centre that alter their behaviour through training data manipulation, weight modification, or component substitution. These attacks can cause AI systems to produce subtly incorrect observations, recommendations, or analysis that appears correct. The AI adversarial defence requirements of Section 18.3 and the formal correctness requirements of Section 12 address this threat.

**Logic and Authentication Attacks:** Exploitation of gaps between the intended behaviour of governance software and its actual implemented behaviour. These attacks exploit not memory errors or execution vulnerabilities but semantic mismatches between specification and implementation. Formal Verification requirements of Section 12 are the primary defence for governance-critical software.

**Succession and Transition Exploitation:** Attacks timed to coincide with governance transitions — personnel changes, restructuring, system migrations — when institutional knowledge is incomplete and verification processes may be degraded.

### 8.3 Security as Structural Governance

Security under this specification is not a technical function separate from governance. Security failures are governance failures. A security compromise of the Centre is a Constitutional Condition II violation if it grants autonomous systems authority they should not have. It is a Constitutional Condition III violation if it introduces false data into the governance decision process. It is a Constitutional Condition I violation if the compromise degrades Governance Capacity below the Governance Risk Level.

Security controls are therefore required to satisfy the same Independent Observation requirements as governance controls. A security system that is self-declared as effective is not independently observed as effective. Security effectiveness must be independently verified continuously.

---

## 9. Reality Integrity

The Reality Integrity Protocol — hereafter the Integrity Protocol — is the sub-system within the Centre's Sense Layer that validates the authenticity and integrity of all observations before they are processed.

### 9.1 Purpose

The Integrity Protocol exists because the threat of Reality Fabrication (Section 8.2) cannot be addressed by conventional anomaly detection. Adversaries capable of generating synthetic telemetry can generate data that is statistically indistinguishable from authentic data. The only valid defence is Cryptographic Provenance: evidence that a piece of data was generated by the source it claims to be from, and has not been altered in transit.

### 9.2 Cryptographic Provenance Requirements

Every telemetry input, observation, and governance signal processed by the Centre must carry Cryptographic Provenance. This means:

- Every observation is digitally signed at the point of generation by the generating system, using the Post-Quantum Cryptography standards defined in Section 11
- The signature chain from observation source to Centre is verifiable at every link
- Any break in the signature chain produces a verification failure, which is treated as a potential Reality Fabrication attack and triggers a Governance Risk Level increase
- Observations without verifiable Cryptographic Provenance are quarantined from the governance decision process and logged as anomalies

### 9.3 Origin Authentication

Before an observation is admitted to the Verify Layer, the Integrity Protocol confirms:

- The observation originates from a registered, authorised observation source
- The observation source's cryptographic identity is valid and has not been revoked
- The observation timestamp is consistent with the observation source's expected reporting cadence
- The observation content is consistent with the observation source's known operational constraints

Failure of any origin authentication check triggers the same response as Cryptographic Provenance failure: quarantine, logging, and Governance Risk Level increase.

### 9.4 Synthetic Observation Detection

In addition to Cryptographic Provenance, the Integrity Protocol operates AI-native analysis specifically designed to detect the signatures of synthetically generated or AI-manipulated observations:

- Cross-correlation of independent observation streams for implausible consistency — authentic observations of the same system typically exhibit natural variance; artificially generated observations may be overly consistent
- Temporal pattern analysis — real systems exhibit characteristic timing patterns; synthetic observations may not replicate these correctly
- Semantic coherence checking — observations from different systems should be semantically consistent; Reality Fabrication attacks that manipulate multiple streams simultaneously may produce semantic inconsistencies across streams

Synthetic observation detection findings are forwarded to the Adversarial Observer function and treated as Disagreement Condition triggers.

### 9.5 Integrity Protocol Independence

The Integrity Protocol itself must be independent of the systems it monitors. It must be:

- Operated on infrastructure that is physically and logically separate from the operational systems being observed
- Cryptographically sealed against modification by operational system administrators
- Subject to its own independent integrity verification by an external observer
- Capable of operation without the cooperation of the systems it monitors

---

## 10. Continuous Adversarial Intelligence

The Continuous Adversarial Intelligence function — hereafter the Intelligence Function — is the governance system's continuously operating adversarial analysis capability. It finds vulnerabilities in the Governing Entity's own infrastructure before adversaries do.

### 10.1 Purpose

The Intelligence Function exists because the threat of AI-Native Adversaries (Section 8.2) cannot be addressed by periodic penetration testing. An adversary operating at machine speed can construct and execute an exploit in less time than a defined testing interval. The only valid defence is continuous adversarial analysis that operates at the same speed as the threat it addresses.

### 10.2 Function

The Intelligence Function continuously:

- Analyses the Governing Entity's production systems for exploitable vulnerabilities using the same class of automated reasoning that adversaries deploy
- Reviews software composition against known vulnerability databases and newly published vulnerability reports
- Constructs test exploitation scenarios to confirm whether identified vulnerabilities are actually exploitable in the Governing Entity's specific configuration
- Monitors for newly published vulnerability information and immediately assesses whether it applies to the Governing Entity's systems

### 10.3 AI-Speed Response

Findings from the Intelligence Function bypass standard change advisory processes for critical-severity vulnerabilities. The response timeline requirements are:

| Severity | Maximum response time | Escalation |
|---|---|---|
| Critical — exploitable vulnerability in governance-critical system | 4 hours to active mitigation | Immediate Crisis State assessment |
| High — exploitable vulnerability in operational system | 24 hours to active mitigation | Immediate Stress State assessment |
| Medium — exploitable vulnerability with significant barriers to exploitation | 72 hours to active mitigation | Standard governance process |
| Low | Standard governance process | Standard governance process |

"Active mitigation" means either a verified patch deployed to the affected system or a verified compensating control in place that eliminates the exploitability of the vulnerability. Acknowledging the finding does not constitute active mitigation.

### 10.4 Independence Requirements

The Intelligence Function must be operationally independent of the systems it analyses. Personnel responsible for the systems being analysed must not have authority to suppress, delay, or modify Intelligence Function findings before they are reviewed by governance oversight. All findings are logged directly to the Memory Layer before any review process.

### 10.5 Intelligence Function Validation

The Intelligence Function itself is subject to adversarial testing. An independent external function must periodically verify that the Intelligence Function is operating correctly by introducing known vulnerabilities into isolated test environments and confirming that the Intelligence Function detects them within the required timeframes.

---

## 11. Cryptographic Security

### 11.1 Post-Quantum Cryptography Requirement

All cryptographic functions used in governance-critical contexts must use Post-Quantum Cryptographic algorithms. The governance cryptography standard — hereafter the Cryptography Standard — defines the specific algorithms, key management requirements, and migration obligations.

The Cryptography Standard applies to:

- All Centre communications
- All Governance Records stored in the Memory Layer
- All Certification Hashes on governance decisions
- All Cryptographic Provenance chains in the Integrity Protocol
- All Identity Assurance Level 3 and Level 4 authentication functions
- All software signing and artefact integrity verification

### 11.2 Cryptographic Agility

The governance cryptographic infrastructure must support algorithm migration without disrupting governance continuity. When a cryptographic algorithm is identified as compromised or below-standard:

- New cryptographic material is generated using the replacement algorithm
- All new governance records are signed with the new algorithm
- Existing records are re-signed with the new algorithm on a defined migration schedule
- The transition is completed within the period defined by the severity of the compromise assessment
- All transition activities are logged in the Memory Layer

### 11.3 Key Management

- All cryptographic keys used in governance-critical functions are generated within Hardware Security Modules or equivalent tamper-resistant hardware
- Private keys used for governance record signing never exist outside tamper-resistant hardware
- Key access requires multi-party authorisation at Identity Assurance Level 4
- Key revocation can be executed within one hour of authorisation
- Emergency re-keying of the entire governance cryptographic infrastructure must be executable within four hours without disrupting governance continuity

### 11.4 Cryptographic Integrity of the Centre

The Centre's own software and infrastructure is subject to continuous cryptographic integrity verification:

- All Centre software components are signed at build time with a verified build chain
- All running Centre components verify their own cryptographic signatures at startup and at defined intervals during operation
- Any component that fails signature verification is quarantined and the event is treated as a potential model poisoning or replacement attack (Section 8.2)
- The cryptographic integrity verification function is itself subject to independent external validation

---

## 12. Formal Correctness

### 12.1 Governance-Critical Software

Software that implements any of the following functions is governance-critical software under this specification and subject to formal correctness requirements:

- Any Centre layer function
- The Reality Integrity Protocol
- The Continuous Adversarial Intelligence function
- Any cryptographic function in the governance infrastructure
- Any function that makes or records governance decisions
- Any function that processes Identity Assurance Level 3 or Level 4 authentication
- Any function that controls access to governance records

### 12.2 Formal Verification Requirement

All governance-critical software must be formally verified against its functional specification. Formal Verification demonstrates, through mathematical proof, that the software behaves in accordance with its specification under all possible inputs and conditions. Testing alone is insufficient for governance-critical software — testing can only demonstrate the absence of detected failures in tested scenarios; it cannot demonstrate the absence of undetected failures in untested scenarios.

Where formal verification of a complete system is not currently technically feasible, formal verification must be applied to the security-critical components of that system, with explicit documentation of which components have been formally verified and which have not. Unverified components are treated as potential vulnerabilities and subject to compensating controls.

### 12.3 Memory Safety

All new governance-critical software must be written in memory-safe programming languages — languages in which the common classes of memory safety vulnerabilities (buffer overflows, use-after-free, null pointer dereferences) cannot occur. Where legacy governance-critical software exists in memory-unsafe languages, a migration plan with defined completion dates must be maintained and reviewed by oversight.

Memory-safe programming languages are those that enforce memory safety at the language level, through the language's type system and ownership model, without requiring programmers to manually verify memory safety in every operation.

### 12.4 Software Bill of Provenance

Every production release of any governance-critical software must be accompanied by a complete Software Bill of Provenance containing:

- A cryptographically signed inventory of every software component, library, and toolchain element included in the release
- The verified source repository location and commit hash of each component
- The complete dependency graph including transitive dependencies
- The result of Intelligence Function analysis of all components against known vulnerability databases
- Any components that could not be verified against authoritative sources, with explicit risk documentation

### 12.5 Build Integrity

The build process for governance-critical software must be:

- Reproducible — the same source code, compiled with the same build environment, produces bit-identical output
- Verified — the build environment itself is subject to Cryptographic Provenance and formal integrity verification
- Isolated — the build environment has no access to production systems and no connection to external networks during the build process

---

## 13. Governance Enforcement

### 13.1 Policy as Executable Code

Governance policies must be expressed in machine-readable, version-controlled, automatically enforceable form. A policy that exists only as a document is not enforced by this specification's mechanisms. All policies subject to this specification must be:

- Expressed in a format that can be automatically evaluated against system state
- Stored in version-controlled repositories with full change history
- Subject to governance review and approval before activation
- Automatically applied at all relevant enforcement points without manual intervention
- Auditable — every policy evaluation, pass or fail, is logged in the Memory Layer

### 13.2 Continuous Compliance

The Centre continuously monitors all governed systems for compliance with all active governance policies. Compliance is not a periodic state. It is a continuous condition that is verified in real time.

The following conditions are monitored continuously:

- Governance Capacity component values against their Minimum Viability Floors
- System configurations against authorised baseline states
- Access patterns against authorised access policies
- Data movements against data sovereignty policies
- Software components against approved component registries and known vulnerability databases

### 13.3 Automated Enforcement

Where technically feasible, governance policy violations are corrected automatically without requiring human intervention:

- Unauthorised configuration changes are automatically reverted to the authorised baseline
- Access that violates current policy is automatically blocked at the point of attempt
- Data movements that violate sovereignty policies are automatically blocked before execution
- Software components that fail integrity verification are automatically quarantined

All automated enforcement actions are logged before execution and are auditable.

### 13.4 Exception Management

Where a governance policy cannot be complied with, the exception must be:

- Formally documented with the specific policy, the period of non-compliance, and the reason
- Approved by an authority with standing to accept the associated risk
- Time-limited — exceptions do not extend automatically
- Tracked in the governance register
- Visible to the Oversight Body

Exceptions are governance decisions. They require Decision Contracts.

---

## 14. Authority and Decision Structures

### 14.1 The Three-Layer Authority Structure

**Strategic Authority:** Defines governance policy, objectives, and the mandate of the Governing Entity. Strategic Authority cannot be delegated — it must always be exercised by accountable leadership. The holders of Strategic Authority are the ultimate Accountable Parties for all governance outcomes.

**Operational Authority:** Manages execution of governance processes within the boundaries set by Strategic Authority. Operational Authority may be delegated. Delegation does not transfer accountability.

**Oversight Authority:** Provides independent verification, audit, and accountability review. Oversight Authority must be structurally independent of Operational Authority — a single actor cannot hold both simultaneously.

### 14.2 Delegation

Authority may be delegated under the following conditions:

- Delegation is explicitly documented in the Memory Layer
- The scope, limits, and duration of the delegation are precisely defined
- Delegated authority cannot exceed the authority of the delegating party
- The delegating party retains full accountability for all actions taken under delegation
- Delegation is revocable at any time by the delegating party
- Automated systems may receive delegated operational authority only for actions explicitly within their defined Bounded Capability

### 14.3 Accountability Separation

Accountability cannot be delegated. The authority holder who approved an action retains accountability for its consequences regardless of who or what executed it. An automated system that executes an action carries no independent accountability — accountability rests entirely with the human authority that approved the system's Bounded Capability.

### 14.4 The Decision Contract

Every governance decision must be accompanied by a Decision Contract. A decision without a complete Decision Contract is not a valid governance decision — it is an unaccountable action, which is prohibited under Section 4.3.

The minimum Decision Contract contains:

| Field | Definition | Requirement |
|---|---|---|
| Statement | A precise statement of the decision in terms understandable to Stakeholders | Always required |
| Justification | The reasoning for this decision over available alternatives | Always required |
| Risk Assessment | An independently assessed evaluation of the risks of this decision and its alternatives | Always required |
| Reversibility | Whether this decision can be undone, and under what conditions | Always required |
| Confidence Basis | The Verified Reality findings on which the decision is based | Always required — Constitutional Condition III |
| Observer Validation | Confirmation that the reality basis has been verified through Multi-Observer Verification | Always required |
| Accountability | The identity and authority of the approving Human Authority | Always required |
| Expiry | The date after which this decision is subject to review | Always required for time-sensitive decisions |

### 14.5 Conflict Resolution

When actions require authority that spans multiple authority holders, conflicts are resolved by:

- Referring the decision to the common superior authority in the hierarchy
- Applying the most restrictive policy where authorities conflict
- Escalating to Oversight Authority when the conflict cannot be resolved within the authority hierarchy

All conflict resolution decisions are documented in the Memory Layer.

---

## 15. Identity and Access Governance

### 15.1 Identity Assurance Levels

Four levels of identity assurance are defined. The required assurance level for any access function is proportional to the sensitivity and authority level of that function.

| Level | Description | Verification Method | Applicable Function |
|---|---|---|---|
| Level 1 | Self-asserted identity | Password or equivalent | Public information access only |
| Level 2 | Credential-verified identity | Multi-factor: password plus time-based code | Standard operational access |
| Level 3 | Strongly authenticated identity | Multi-factor with hardware token or equivalent | Sensitive operational access; governance record access |
| Level 4 | Hardware-bound, phishing-resistant identity | Hardware security key with challenge-response | All Sovereign Decisions; all Decide Layer approvals; all cryptographic key operations |

Level 4 identity assurance is mandatory for all governance decisions that enter the Memory Layer. A governance decision approved by an identity verified at less than Level 4 is not a valid governance decision under this specification.

### 15.2 Authorisation Architecture

- Role-based access as the baseline authorisation model for all standard access
- Context-sensitive, attribute-based access for elevated or sensitive functions
- Just-in-time access elevation for privileged functions, with automatic expiry after the approved duration
- Separation of duties enforced for functions where concentration of access creates governance risk — the same individual may not both approve a governance decision and execute it
- No persistent standing privileged access — elevated access is always time-limited

### 15.3 Privileged Access

Privileged access is access to systems, data, or functions that can alter governance controls, modify governance records, or access sensitive governance information.

Privileged access requirements:

- All privileged sessions are logged in full in the Memory Layer before the session begins
- Privileged access grants are approved by an authority with standing to grant them at Identity Assurance Level 4
- Privileged access is granted for the minimum duration necessary
- Privileged access reviews occur at maximum 90-day intervals; privileged access that is not actively reviewed and reconfirmed is automatically revoked
- Emergency privileged access is documented, auditable, and reviewed after each use

### 15.4 Identity Lifecycle

- Identity provisioning follows a formally documented approval process
- Identity deprovisioning is automated upon termination of the relationship that justified the identity
- Dormant identities — those not used within the defined dormancy period — are detected and disabled automatically
- The complete identity register is reconciled against authoritative personnel records at defined intervals

---

## 16. Data Sovereignty

### 16.1 The Sovereignty Principle

All data generated or held by the Governing Entity is subject to the governance authority of the Governing Entity. Data Sovereignty is the default condition. Any sharing, transfer, or cross-boundary movement of governed data requires explicit authorisation from an authority with standing to grant it, and is subject to ongoing oversight.

### 16.2 Data Classification

All data held by the Governing Entity must be classified in accordance with a sensitivity framework. The following classification levels are the minimum required:

| Classification | Handling Requirements |
|---|---|
| Open | No access restrictions |
| Internal | Accessible to authorised internal actors only |
| Sensitive | Enhanced controls; encrypted at rest and in transit; all access logged |
| Restricted | Strict access controls; elevated audit requirements; cross-boundary movement requires specific authorisation |
| Sovereign | Highest controls; movement outside the Governing Entity's systems requires explicit authority from Strategic Authority level |

The Governing Entity defines the specific criteria for each classification level. The requirement to maintain a classification framework and enforce it automatically is universal.

### 16.3 Data Residency

Data classified at Internal level or above must be stored and processed within explicitly defined residency boundaries. The residency boundaries are documented and subject to Independent Observation for compliance.

Cross-residency-boundary data movement requires:

- A formal data transfer authorisation approved by an authority with standing
- End-to-end encryption meeting the Cryptography Standard of Section 11
- Logging in the Memory Layer including the authorising authority, the data classification, and the receiving entity
- A defined retention and deletion obligation for the receiving entity

### 16.4 Personal Information

Data that relates to identifiable individuals is subject to the following additional requirements:

- Collection is limited to what is necessary for the defined and authorised purpose
- Data collected for one purpose is not reused for a materially different purpose without fresh authorisation
- A register of all personal information processing activities is maintained
- Privacy risk assessments are conducted for all systems processing personal information at scale

---

## 17. Operational Disciplines

Each operational discipline delivers a class of technical capability within governance constraints. All disciplines operate under the three Constitutional Conditions, the authority structures of Section 14, the security requirements of Sections 8 through 12, and the Human and Machine Authority partition of Section 18.

### 17.1 Continuous Delivery Discipline

**Function:** Delivers software and infrastructure changes through automated pipelines with complete traceability.

**Requirements:**
- Every change from request through deployment is traceable with an immutable audit record in the Memory Layer
- All delivery pipeline configurations are stored in version-controlled repositories under change control
- Automated testing gates must pass before promotion to production — no bypass of testing gates is permitted
- No production deployment may be irreversible — Rollback Capability is required for all deployments
- All build artefacts are cryptographically signed as part of the Software Bill of Provenance requirement
- Delivery performance metrics — frequency, lead time, failure rate, recovery time — are measured and reported to the Centre's Risk Engine
- No deployment to production occurs without satisfying current authorisation conditions
- Decision Contracts are required for all deployments that affect governance-critical systems

### 17.2 Security Operations Discipline

**Function:** Continuously monitors for, detects, responds to, and recovers from threats across all governed systems.

**Requirements:**
- Continuous security monitoring proportional to the risk classification of each system — not periodic, continuous
- Security event management aggregates telemetry from all sources with defined retention periods meeting the Memory Layer requirements
- Incident response capability with documented procedures, defined severity levels, escalation paths, and notification obligations — tested at defined intervals
- Vulnerability remediation timelines governed by the Intelligence Function requirements of Section 10.3 for critical and high severity; standard governance process for medium and low
- Penetration testing and adversarial simulation at defined intervals, in addition to continuous Intelligence Function operation
- All security findings tracked in the governance register with assigned owners and target remediation dates
- The Security Operations Discipline feeds its findings directly to the Centre's Think Layer as a primary Governance Risk Level input

### 17.3 Infrastructure Configuration Discipline

**Function:** Manages all infrastructure and system configuration through version-controlled, declarative definitions, with automated reconciliation to maintain authorised state.

**Requirements:**
- All infrastructure and system configuration declared as code in version-controlled repositories
- The declared state in version control is the authoritative definition of what the operational state must be
- Automated reconciliation continuously detects deviations between declared and actual state — deviations are treated as potential security incidents until verified as authorised changes
- All production-affecting changes require review and approval before merge, with Decision Contracts for governance-critical systems
- Cryptographic signing of configuration change commits
- Credentials and sensitive configuration values are never stored in configuration repositories — dedicated secrets management is required
- The complete history of all infrastructure changes is preserved and non-repudiable in the Memory Layer

### 17.4 Financial Governance Discipline

**Function:** Ensures all technology and operational expenditure is transparent, accountable, efficient, and aligned with authorised allocations.

**Requirements:**
- All expenditure attributed to an authorised cost centre or funding authority
- Expenditure reporting available to budget authority holders at defined intervals
- Forecasting integrated with the Governing Entity's financial planning processes
- Anomalous expenditure detected automatically and escalated to the Centre's Think Layer
- No financial commitment that exceeds the authority of the approving party — financial authority limits are enforced in systems where technically feasible
- Unit economics — cost per service unit, cost per transaction — measured and reported for significant services
- Resource efficiency reviews at defined intervals

### 17.5 Integrated Security Delivery Discipline

**Function:** Integrates security requirements, testing, and accountability into every stage of the software delivery lifecycle.

**Requirements:**
- Static security analysis of source code in every delivery pipeline
- Dynamic security analysis of all externally accessible systems
- Composition analysis of all third-party components with vulnerability assessment
- Container and artefact scanning before promotion to any production environment
- Infrastructure configuration security analysis before deployment
- Complete Software Bill of Provenance for every production release
- Security gates in the delivery pipeline cause build failure for findings above the Governing Entity's risk threshold — exceptions require Decision Contracts
- All security exceptions are visible to the Oversight Body

### 17.6 Automated Intelligence Governance Discipline

**Function:** Governs the full lifecycle of automated reasoning systems from development through deployment, operation, monitoring, and retirement.

**Requirements:**
- All production automated reasoning systems registered in a model registry with full versioning and lineage
- Model performance monitored continuously with drift detection and alerting
- Training data lineage and provenance documented and retained as Governance Records
- Explainability documentation maintained for all models whose outputs influence decisions affecting Stakeholder rights
- Bias and fairness assessments conducted before deployment in any context where model outputs affect Stakeholders
- Human oversight maintained for all automated decisions that materially affect individual Stakeholders — Human Authority defines what constitutes material effect
- All automated reasoning systems operate within the Human and Machine Authority partition of Section 18
- No automated reasoning system holds Sovereign Decision authority — Constitutional Condition II applies to all systems governed by this discipline
- Model retirement procedures ensure decommissioned systems do not persist in production environments
- Governance risk assessments for all production automated reasoning systems

### 17.7 Data Operations Discipline

**Function:** Governs data pipelines, data quality, lineage, and access, ensuring data assets are reliable, traceable, and handled consistently with governance requirements.

**Requirements:**
- A data catalogue maintained for all significant data assets with full lineage tracking
- Data quality rules defined, automated, and monitored for all operational data assets
- Personal information detected, classified, and handled in accordance with Section 16.4
- Data retention and disposal enforced automatically — data is not retained beyond the authorised period without explicit renewal authorisation
- All data access logged in the Memory Layer with attribution to the accessing identity and the authority under which access was granted
- Data pipeline failures detected before they propagate to downstream consumers
- All data sharing governed by formal data sharing agreements that define classification, purpose, retention, and deletion obligations

### 17.8 Platform Operations Discipline

**Function:** Provides shared operational platforms that enable delivery teams to provision governed infrastructure through self-service mechanisms with embedded governance controls.

**Requirements:**
- Self-service capabilities provided within governance guardrails — teams operate within approved parameters without manual intervention from platform operators
- All platform components deployed from cryptographically signed, hardened, approved baseline configurations
- Service availability objectives defined, published, and reported for all platform services
- All provisioning requests automatically validated against governance policy before fulfilment
- Tenant isolation enforced — entities sharing a platform cannot access each other's data or operational state
- Recovery capability defined, documented, and tested at defined intervals
- Platform governance subject to oversight with representation from consuming entities

### 17.9 Network Governance Discipline

**Function:** Manages and governs network infrastructure, ensuring secure, reliable, and policy-compliant connectivity throughout the governed environment.

**Requirements:**
- Network segmentation enforced — environments of different classification levels are isolated at the network level
- All network traffic monitored with anomaly detection and alerting, feeding into the Centre's Sense Layer
- All data in transit across network boundaries encrypted using the Cryptography Standard of Section 11
- Network configuration managed as code under the Infrastructure Configuration Discipline
- Zero-Trust Architecture adopted as the target state with a defined implementation roadmap
- All network changes subject to the same governance controls as software changes — Decision Contracts required for governance-critical network changes

### 17.10 Infrastructure and Service Management Discipline

**Function:** Manages operational technology services, infrastructure, and support to deliver reliable, responsive, and accountable technology services.

**Requirements:**
- A service management function covering incident, problem, change, and asset management processes
- A configuration record system maintaining accurate records of all operational technology assets and their governance relationships
- Service availability commitments defined and published for all operational technology services
- Vulnerability and patch management at authorised patch levels within the timelines defined by Section 10.3
- Technology asset lifecycle management from procurement through verified, secure disposal
- Operational continuity plans defined, documented, and tested for all governance-critical services
- All user-facing services meet accessibility standards defined by the Governing Entity

---

## 18. Human and Machine Authority

### 18.1 The Authority Partition

The following authority partition applies universally across all operational disciplines and all Centre layers. It cannot be modified by operational configuration, Delegation, or any authority within the governed system.

| Operational Function | Machine Role | Human Role |
|---|---|---|
| Sensing and data collection | Primary — continuous collection and anomaly detection | Audit — validate machine outputs and calibrate sensing parameters |
| Observation verification | Supporting — cross-validation and consistency checking | Validate — confirm verified reality findings; approve contested observations |
| Scenario analysis and simulation | Primary — model consequences of alternative decisions | Review — assess, challenge, and approve analytical outputs |
| Governance decisions | Propose only — generate Decision Contracts with analysis | Approve — the only valid source of governance decision authority |
| Execution | Bounded and Controlled — execute within approved scope | Sovereign — halt, modify, or reverse at any point |

### 18.2 Machine Capability Boundaries

The formal boundary of machine authority:

```
Machine operational scope  is a strict subset of  Capacity to Act

Machine operational scope  has no intersection with  Sovereign Decision authority
```

In plain terms: machines operate as bounded tools within the governance system. They amplify Human Authority's capacity to sense, analyse, and execute. They do not constitute governance authority. The machine that executes a governance decision and the human authority that approved it are not equivalent actors — they have fundamentally different governance status, and all accountability rests with the human authority.

### 18.3 Machine System Adversarial Defence

All machine systems operating within the Centre are subject to continuous adversarial testing:

- Output cross-validation — machine system outputs are independently assessed by separate machine systems and human reviewers
- Drift detection — the Centre continuously monitors machine system outputs for systematic change in behaviour, accuracy, or bias that was not present during the system's validated operation
- Adversarial input testing — machine systems are periodically subjected to inputs designed to elicit incorrect outputs, to verify their resistance to manipulation
- A machine system that cannot be validated by Independent Observation does not qualify as a valid Verify Layer input and does not contribute to Independently Observed governance measurements

### 18.4 Machine Independence Requirement

Every Centre implementation must maintain the capability to govern without any machine system:

- Manual operation procedures for all governance-critical functions
- Documented and tested manual execution pathways for all Sovereign Decision categories
- Human-operable fallback for the Sense Layer, Verify Layer, Think Layer, and Act Layer
- A tested machine isolation procedure that removes all machine systems from governance functions without disrupting governance continuity

This requirement is not a backup condition. It is a design requirement. A Centre that cannot operate without machine systems has transferred Sovereign Decision authority to those systems by design — a violation of Constitutional Condition II.

---

## 19. Observability

### 19.1 Technical Observability Pillars

Three technical dimensions of observability are required for all governed systems:

**Measures:** Quantitative measurements of system state and performance over time — counters, gauges, and histograms aggregated over defined intervals.

**Records:** Structured, timestamped records of discrete operational events — actions taken, decisions made, access granted, changes executed.

**Traces:** End-to-end records of the path taken by requests or processes through the governed system — identifying each component the request passed through and the latency at each step.

All three observability dimensions must be maintained for all production systems. A system that cannot be observed across all three dimensions is treated as a governance gap.

### 19.2 Governance Observability Domains

Beyond technical observability, five governance observability domains must be continuously monitored:

**Governance telemetry:** Policy compliance state, authority utilisation, exception register status, Decision Contract completeness rate.

**Financial telemetry:** Expenditure against authorised allocations in real time, anomaly detections, commitment utilisation.

**Security telemetry:** Continuously observed security posture, active threat status, Intelligence Function finding queue, vulnerability remediation progress.

**Identity telemetry:** Access pattern analysis, privilege utilisation, anomalous identity events, dormant account status.

**Stakeholder telemetry:** Independently observed signals of stakeholder welfare — the primary operational expression of the Fidelity component. Stakeholder telemetry is not a secondary input; it is a primary governance signal. A Sense Layer that treats stakeholder feedback as lower priority than system metrics has inverted the governance priority order.

### 19.3 The Three-Observer Rule

All governance-critical observations must be produced simultaneously by three structurally independent observer types. The three types are:

**Internal Observer:** Operates within the Governing Entity's own infrastructure. Necessary but insufficient alone — subject to capture, manipulation, and the Reality Fabrication threat.

**External Observer:** Operates independently of the Governing Entity's infrastructure, is not funded or directed by the Governing Entity, and whose observations the Governing Entity cannot suppress or modify. The External Observer provides the primary check on Internal Observer integrity.

**Adversarial Observer:** Actively attempts to find discrepancies in the observations made by the Internal and External Observers. The Adversarial Observer does not assume observations are correct — it attempts to disprove them. The Adversarial Observer is the primary check on both internal and external observation integrity, and the primary defence against Coordinated Multi-Node Deception.

**The Disagreement Rule:**

```
When any two observers produce materially different assessments
of the same governance reality:

    Governance Risk Level  INCREASES
    Decision based on contested observation  IS SUSPENDED
    Investigation of disagreement source  BEGINS IMMEDIATELY
```

Disagreement is not resolved by averaging. Disagreement is not resolved by deferring to the Internal Observer. Disagreement is a governance signal: it indicates that the governance system's knowledge of its own state is unreliable. That unreliability must be investigated and resolved before governance decisions that depend on the contested observation are made.

### 19.4 Audit Record Integrity

All governance records required by this specification must be:

- Stored in tamper-resistant structures with Certification Hashes enabling verification of non-alteration
- Retained for a period defined by the Governing Entity based on its accountability obligations — minimum retention periods reflect the longest potential investigation or review timeline
- Accessible to the Oversight Body without modification by operational personnel
- Independently verifiable for integrity — the verification process must be available to the Oversight Body without requiring the cooperation of operational personnel

### 19.5 Governance Capacity Computation

The Governance Capacity calculation must be computable from Independently Observed component values at any time. The following requirements apply:

- Self-Declared component values are not valid inputs
- The computation is auditable — the inputs, the computation method, and the result are all logged in the Memory Layer
- The computation is reproducible — given the same inputs, the same result is always produced
- The computation is transparent — the Oversight Body can access the inputs, the method, and the result at any time

---

## 20. Federation

### 20.1 Federation Principles

When multiple Governing Entities operate through a shared governance arrangement — a Federation — the following principles apply:

- Each member entity retains full governance authority within its own boundary
- The Federation Agreement defines precisely what authority, data, and operational capability is shared
- The Federation does not create a superior governance authority unless explicitly established by the Federation Agreement
- Each entity's participation in the Federation is voluntary and revocable
- The withdrawal of a member entity from the Federation does not extinguish its governance obligations under this specification

### 20.2 Federation Governance Capacity

For federated systems, the governance capacity of the overall federated system is a function of the individual governance capacities of all member nodes, subject to a minimum floor established by the Federation Agreement:

```
Federated Governance Capacity  =  a function of all member Governance Capacities
                                    that is always at or above the Federation Floor

Federation Floor  =  the minimum system-level Governance Capacity
                     established by the Federation Agreement
```

The product structure means that distributed observation provides higher total Adaptive Transparency than any single entity could achieve alone — each member's Sense Layer covers a different part of the federated environment, and the combination provides coverage that exceeds any individual component.

The Federation Floor prevents the strict product form from collapsing the Federation when any single member's Governance Capacity approaches zero through partial participation. The Federation Agreement must define the floor and the response when any member falls below it.

### 20.3 Federation Requirements

- A formal Federation Agreement defining scope, obligations, governance mechanisms, and the Federation Floor
- A Federation Governance Body with representation from all member entities and the authority to assess compliance with the Federation Agreement
- Defined escalation and dispute resolution mechanisms for cross-entity governance conflicts
- A Federation Oversight Function providing each member entity with visibility over cross-entity interactions that affect it
- Regular review of the Federation Agreement — at maximum five-year intervals

### 20.4 Federated Data Governance

Data shared across Federation boundaries is governed by:

- The Data Sovereignty requirements of Section 16 of each involved entity
- The specific data sharing terms of the Federation Agreement
- The most restrictive applicable requirement from any involved entity governs where requirements conflict
- Audit records maintained by both sending and receiving entity for all cross-boundary data movements

### 20.5 Cross-Federation Security

The Cross-Federation Manipulation threat (Section 8.2) requires specific countermeasures in federated environments:

- Each member entity validates all observations and data received from other Federation members through its own Reality Integrity Protocol
- Trust is not implicit between Federation members — all cross-member communications are authenticated and verified
- A compromise of any single Federation member does not automatically create trust access to other members
- Cross-member Governance Capacity assessments are conducted independently by each member, not accepted as reported by the assessed member

---

## 21. Compliance Mapping

This specification does not mandate any specific external regulatory framework, national standard, or international certification scheme. It defines the governance requirements that must be met. The Governing Entity is responsible for identifying all external obligations applicable to its context and mapping them against the requirements of this specification.

### 21.1 Mapping Requirement

The Governing Entity must maintain a Compliance Map that:

- Identifies all applicable external regulatory obligations, legal frameworks, and contractual requirements
- Maps each external obligation to the requirement within this specification that satisfies it, partially satisfies it, or is supplemented by it
- Documents any external obligations that exceed the requirements of this specification and specifies how those additional requirements are implemented
- Is maintained as a live document, updated when external obligations or this specification change

### 21.2 Gap Management

Where the Governing Entity cannot fully satisfy an applicable external obligation through this specification's requirements:

- The gap is documented in the governance register as a finding
- A remediation plan is approved by an authority with standing to accept the interim risk
- The finding and remediation plan are visible to the Oversight Body
- Progress against the remediation plan is tracked and reported

---

## 22. Stakeholder Enforcement Capacity

### 22.1 The Enforcement Problem

The Governing Entity with the most resources and the greatest motivation to resist governance accountability proceedings is exactly the entity that has failed to govern. The Stakeholders with the most need to assert that failure are exactly those with the fewest resources, least coordination capacity, and least protection to do so.

This is the structural challenge of governance enforcement. It cannot be resolved by legal standing provisions alone. Standing to assert a governance failure is meaningless if the Stakeholders with standing have no practical ability to exercise it. This specification therefore treats Stakeholder enforcement capacity as a first-class governance requirement — not an aspirational condition, but a structural obligation.

A governance system that cannot be enforced by those it is designed to protect has zero Fidelity by its own definition. Zero Fidelity produces zero Governance Capacity. A Governing Entity that fails to maintain Stakeholder enforcement capacity is therefore directly reducing its own Governance Capacity.

### 22.2 Mandatory Stakeholder Capacity Conditions

The Governing Entity must maintain and independently observe the following conditions that enable Stakeholders to exercise governance accountability:

**Freedom of Assembly:** Stakeholders must be able to organise, coordinate, and act collectively on governance matters without interference from the Governing Entity.

**Information Access:** Stakeholders must have access to the Independently Observed Governance Capacity measurements for the Governing Entity — sufficient information to assess whether governance obligations are being met.

**Independent Representation:** Stakeholders must have access to representation that is capable of asserting governance failures on their behalf and that is independent of the Governing Entity.

**Non-Retaliation:** Stakeholders who assert or support governance accountability proceedings must be protected from any form of retaliation by the Governing Entity, including through indirect means.

**Suppression of any of these conditions by the Governing Entity is itself a governance failure.** It is a failure of the Adaptive Transparency component — the governance system is actively suppressing the feedback signals that would detect its own failures. The Cascade Property (Section 2.6) predicts the consequences.

### 22.3 The Inverse Capacity Principle

The enforcement resources available to Stakeholders must scale inversely with the independently observed Governance Capacity of the Governing Entity against whom they are asserting:

| Observed Governance Capacity condition | Stakeholder support level |
|---|---|
| Governance Capacity substantially above Governance Risk Level | Standard information access and representation access |
| Governance Capacity approaching Governance Risk Level — Stress State | Enhanced information disclosure; independently funded representation support activates automatically |
| Governance Capacity below Governance Risk Level — Crisis State | Mandatory public resourcing of Stakeholder representation activates; funded from a source the Governing Entity cannot reduce or control |

The Inverse Capacity Principle ensures that enforcement support scales to enforcement need without requiring the Governing Entity's cooperation. This is the structural substitute for the natural selection mechanism — governance systems, unlike biological systems, do not automatically remove themselves when they fail.

### 22.4 The Independent Stakeholder Advocacy Function

Every Governing Entity at Tier 2 and above must maintain, or participate in, an Independent Stakeholder Advocacy Function that:

- Has standing to assert governance failures on behalf of any Stakeholder group
- Has guaranteed access to Independently Observed Governance Capacity measurements without requiring formal proceedings to obtain them
- Is funded independently of the Governing Entity whose conduct it may challenge
- Is staffed independently of the Governing Entity
- Cannot be suspended, defunded, interfered with, or directed by the Governing Entity
- Reports to the Oversight Body, not to the Governing Entity

The Independent Stakeholder Advocacy Function is not the Oversight Body. The Oversight Body assesses whether governance requirements are being met. The Independent Stakeholder Advocacy Function represents those who bear the cost when they are not. These are different functions requiring different structural independence.

### 22.5 The External Escalation Pathway

Every Governing Entity at Tier 3 and above must establish a functioning External Escalation Pathway through which Stakeholders can:

- Submit evidence of governance failures to an entity outside the Governing Entity's jurisdiction or authority
- Receive acknowledgment, assessment, and escalation of that evidence
- Access interim protection while proceedings are underway

A Tier 3 Governing Entity without a functioning External Escalation Pathway does not satisfy the enforcement architecture requirements of this specification.

---

## 23. Scalability and Maturity

### 23.1 Operational Tiers

Four operational tiers define the scale context for implementation. The tier determines which disciplines must be operated independently versus consumed as shared services, and the Centre's performance requirements.

| Tier | Context | Scale | Centre Requirement |
|---|---|---|---|
| Tier 1 | Small team or project | 5–50 people | Logical Centre function |
| Tier 2 | Department or programme | 50–500 people | Operational Centre |
| Tier 3 | Enterprise or national scale | 500–10,000+ | Full Centre, continuously staffed |
| Tier 4 | Federated multi-entity | Multiple organisations | Full Centre plus Federation Centre coordination |

### 23.2 Governance Maturity Levels

Five maturity levels define the depth of governance embedding. Scale and maturity are independent — a small team can achieve high maturity; a large organisation can operate at low maturity.

| Level | Label | Governance and Centre Condition |
|---|---|---|
| Level 1 | Initial | Governance exists as policy documents. Enforcement is manual and inconsistent. No Centre. Governance Capacity not computed. Three Constitutional Conditions not continuously monitored. |
| Level 2 | Defined | Governance processes documented and followed. Logical Centre function operational. Governance Capacity computable on demand. Basic identity and access controls. |
| Level 3 | Managed | Centre operational with Independent Observation infrastructure. Governance Capacity monitored continuously. Stress State detectable. Reality Integrity Protocol deployed. Three-Observer Rule operational. THIS IS THE KEY TRANSITION. |
| Level 4 | Integrated | All Constitutional Conditions continuously verified. All three operating modes functional and automatically triggered. Full machine adversarial defence operational. Formal Correctness applied to governance-critical software. |
| Level 5 | Self-Sustaining | Centre self-aware and self-monitoring. Crisis State triggers automatic Response Cascade initiation. Continuous Adversarial Intelligence operating at full capacity. Post-Quantum Cryptography migration complete. All formal correctness requirements met. |

**The Level 3 transition is the most structurally significant event in the implementation of this specification.** Below Level 3, all Governance Capacity component values are Self-Declared — they are not independently observed. Under the Observation Condition (Section 2.5), Self-Declared values are not valid inputs to the Governance Capacity formula. Below Level 3, a Governing Entity's Governance Capacity is formally zero — not because the components are necessarily absent, but because their values cannot be independently verified.

Level 3 is the threshold at which governance becomes real rather than documented.

### 23.3 Minimum Requirements by Tier

| Tier | Minimum Maturity | Centre Form | Key Disciplines | Security Requirements |
|---|---|---|---|---|
| Tier 1 | Level 2 | Logical Centre function | Continuous Delivery, Security Operations, Infrastructure Configuration, Financial Governance | Basic Cryptographic Provenance; Intelligence Function on demand |
| Tier 2 | Level 3 | Operational Centre | All ten disciplines | Reality Integrity Protocol; Three-Observer Rule; Intelligence Function operational; basic Formal Correctness |
| Tier 3 | Level 4 | Full Centre, 24/7 | All disciplines plus full security architecture | Full adversarial defence; Post-Quantum Cryptography; Formal Verification of governance-critical software |
| Tier 4 | Level 4 | Full Centre plus Federation | All disciplines plus Federation governance | All Tier 3 requirements plus cross-federation security measures |

---

## 24. Implementation Roadmap

### Phase 1 — Governance Foundation (Months 1–6)

**Objective:** Establish the governance structure and core infrastructure before expanding capability coverage.

Activities:
- Document the authority structure, establish the Oversight Body, and define the Independent Stakeholder Advocacy Function
- Deploy identity and access governance infrastructure at Levels 1 through 3
- Establish centralised logging and security monitoring feeding the Centre's Sense Layer
- Deploy continuous delivery pipelines with security gates
- Implement data classification and data residency controls
- Establish the governance register for findings, exceptions, and Decision Contracts
- Implement version control for all infrastructure
- Establish financial tracking and cost attribution
- Deploy logical Centre function and initiate Governance Capacity computation capability

**Governance milestone:** Governance Capacity is computable. All privileged access is attributed. Delivery pipeline gates are operational. Governance register is active.

### Phase 2 — Operational Integration (Months 7–18)

**Objective:** All ten disciplines operational; Centre running; Stress State detectable.

Activities:
- Deploy integrated security delivery controls across all delivery pipelines
- Activate Centre with all six layers functioning
- Implement Reality Integrity Protocol in the Sense Layer
- Deploy Three-Observer Rule in the Verify Layer
- Initiate data operations with full data catalogue and lineage tracking
- Deploy advanced security operations with tested incident response
- Implement automated financial governance controls
- Initiate automated intelligence governance for any production machine reasoning systems
- Establish Independent Stakeholder Advocacy Function
- Activate Intelligence Function in basic mode

**Governance milestone:** All disciplines operational. Centre functioning with Independent Observation. Stress State detectable. Independent Stakeholder Advocacy Function established.

### Phase 3 — Continuous Governance (Months 19–36)

**Objective:** Continuous assurance; all Constitutional Conditions continuously verified; full security architecture operational.

Activities:
- Activate full Continuous Governance Assurance replacing periodic compliance checks
- Deploy policy-as-executable-code across all governance domains
- Activate all three operating modes with automatic transitions
- Complete Zero-Trust Architecture implementation
- Deploy full machine adversarial defence including Continuous Adversarial Intelligence at full capacity
- Begin Post-Quantum Cryptography migration
- Apply Formal Verification to governance-critical software components
- Establish External Escalation Pathway
- Activate Inverse Capacity Principle provisions

**Governance milestone:** All three Constitutional Conditions continuously independently verified. All operating modes functional. External Escalation Pathway operational.

### Phase 4 — Federated and Self-Sustaining (Month 36+)

**Objective:** Federation operational; Level 5 maturity achieved.

Activities:
- Establish Federation identity trust framework with partner entities
- Negotiate and implement Federation Agreements
- Extend Centre to Federation Centre coordination
- Deploy cross-entity Governance Capacity monitoring with sovereignty enforcement
- Complete Post-Quantum Cryptography migration
- Complete Formal Verification of all governance-critical software
- Achieve Level 5 maturity — self-sustaining governance

**Governance milestone:** All Constitutional Conditions hold across all Federation boundaries. Stakeholder enforcement capacity functioning in all member entities. Level 5 maturity achieved and independently verified.

---

## 25. Glossary

This glossary is a summary reference. All definitions in this section are governed by and consistent with the full definitions provided in Section 1.

| Term | Summary Definition |
|---|---|
| Accountability | Obligation to answer for use of authority. Cannot be transferred. |
| Adaptive Transparency | Independently observed capacity to detect, understand, and respond to changes. One of four Governance Capacity components. |
| Adversarial Observer | Observer that actively attempts to disprove existing observations. Third of three required observer types. |
| Authority Partition | Division of functions between machine systems (bounded tools) and human authorities (decision-makers). Cannot be modified by configuration. |
| Bounded Capability | The defined operational scope within which a machine system may act autonomously. |
| Cascade Property | The causal mechanism by which Adaptive Transparency degradation initiates sequential degradation of all other Governance Capacity components. |
| Centre | Governance Operations Centre — the mandatory operational brain of this specification. |
| Certification Hash | Cryptographic digest enabling verification that a record has not been altered. |
| Constitutional Condition | One of three requirements (Existence, Human Sovereignty, Verified Reality) that must hold at all times. |
| Continuous Adversarial Intelligence | Continuously operating adversarial analysis of the Governing Entity's own infrastructure. |
| Controlled Execution | Machine system execution: bounded, logged before completion, reversible, with human override authority. |
| Crisis State | Operating condition when Governance Capacity falls below Governance Risk Level. |
| Cryptographic Provenance | Chain of signatures establishing origin and integrity of a governance record or signal. |
| Data Sovereignty | Default governance authority of the Governing Entity over its data. |
| Decision Contract | Minimum information record required with every governance decision. |
| Disagreement Condition | State when independent observers produce materially different assessments. Increases Governance Risk Level. |
| Entropic Risk Property | Governance Risk Level always tends to increase without active governance effort. |
| External Escalation Pathway | Pathway enabling Stakeholders to assert governance failures outside the Governing Entity's jurisdiction. |
| External Observer | Observer independent of the Governing Entity's infrastructure. |
| Fidelity | Independently observed degree to which the governance system acts in Stakeholder interests. One of four Governance Capacity components. |
| Formal Verification | Mathematical proof that software satisfies its specification under all conditions. Required for governance-critical software. |
| Governance Capacity | Product of four independently observed components: Fidelity × Capacity to Act × Institutional Integrity × Adaptive Transparency. |
| Governance Capacity Law | The formal statement that Governance Capacity is the product of the four independently observed components, which must exceed Governance Risk Level to sustain governance. |
| Governance Failure | Condition when any Constitutional Condition is violated. |
| Governance Risk Level | Aggregate time-varying measure of all forces threatening the governed system. Always tends to increase without active governance. |
| Human Authority | The right of a designated human to make final governance decisions and override machine systems. |
| Identity Assurance Level | Four-level scale of confidence in identity verification, from self-asserted to hardware-bound. |
| Immutable Ledger | Record store where written records cannot be modified or deleted. |
| Independent Observation | Measurement by a process structurally separate from the measured actors, with independently verifiable independence. |
| Independent Stakeholder Advocacy Function | Independently funded body with standing to assert governance failures on behalf of Stakeholders. |
| Institutional Integrity | Independently observed degree to which structures genuinely constrain governance actors. One of four Governance Capacity components. |
| Internal Observer | Observer within the Governing Entity's own infrastructure. Necessary but insufficient alone. |
| Inverse Capacity Principle | Stakeholder enforcement resources scale inversely with independently observed Governance Capacity. |
| Memory Layer | Centre layer maintaining the Immutable Ledger, audit trails, and succession data. |
| Minimum Viability Floor | Lowest component value below which the component is treated as absent and Governance Capacity is zero. |
| Multi-Observer Verification | Simultaneous observation by Internal, External, and Adversarial observers with comparison. |
| Normal State | Operating condition when Governance Capacity substantially exceeds Governance Risk Level. |
| Observation Condition | All Governance Capacity components must be Independently Observed; Self-Declared values are invalid. |
| Post-Quantum Cryptography | Cryptographic algorithms resistant to attacks by advanced automated reasoning systems. |
| Reality Integrity Protocol | Sub-system validating authenticity and integrity of all observations entering the Centre. |
| Response Cascade | Four-phase recovery process (Declaration, Correction, Containment, Reconstruction) in Crisis State. |
| Scale Limit Property | Maximum sustainable governance scope is proportional to Independently Observed Adaptive Transparency. |
| Self-Declared Value | Measurement produced by the entity being measured. Not a valid Governance Capacity input. |
| Software Bill of Provenance | Cryptographically signed inventory of all components in a software artefact. |
| Sovereign Decision | Any governance decision materially affecting Stakeholder rights, resources, or welfare. Requires Human Authority. |
| Stakeholder | Any person, entity, or group whose rights, interests, or welfare are materially affected by the Governing Entity. |
| Stress State | Operating condition when Governance Capacity approaches Governance Risk Level. |
| Sustainability Condition | Governance Capacity must exceed Governance Risk Level continuously for governance to exist. |
| Three-Observer Rule | Requirement that governance-critical observations be produced by Internal, External, and Adversarial observers simultaneously. |
| Verified Reality | State of governance knowledge confirmed through Multi-Observer Verification with no Disagreement Condition. |
| Weakest-Link Property | The product of the four components is dominated by the smallest component. Investment priority: fix the weakest first. |
| Zero-Trust Architecture | Security design requiring independent verification of every access request regardless of origin. |

---

*Governance Operations Specification | Final v0.9 | April 2026 | Public Release*

*This specification is self-contained. It defines its own terms, its own authority, and its own requirements. It references no external document, standard, framework, or publication. It is intended to be adopted, implemented, and governed as a standalone instrument by any entity that exercises governance authority over digital systems, human organisations, or critical infrastructure.*

*Version 1.0 will be issued following ratification review of this v0.9 draft. Adopters may use v1.0 immediately if their GovOps initiative is based from this specification.*
