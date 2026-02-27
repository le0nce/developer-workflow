## AI Step 1: Requirements & AI Risk Classification

**Description**  
Extend the standard requirements phase with AI-specific classification and risk assessment. Before development begins, the AI use case must be classified by risk level (high-risk vs. low-risk AI), its role within critical financial functions must be determined, and AI-specific requirements for logging, explainability, human oversight, and resilience must be defined upfront — not retrofitted.

> This step augments [Step 0: Planning / Requirements Review](../extended-steps/planning_requirements_review.md) for projects that use AI.

---

### Inputs
- **Requirements Document** (from Step 0)
- **EU AI Act Risk Classification Framework**
- **DORA ICT Risk Management Framework** (from Step B1)
- **BaFin AI Governance Expectations**

---

### Output
- AI risk classification record (high-risk / low-risk / minimal-risk) *(AI Act)*
- Assessment of whether the AI system supports a critical or important financial function *(DORA)*
- AI-specific requirements defined:
  - Logging requirements *(AI Act, BaFin)*
  - Explainability requirements *(AI Act, BaFin)*
  - Human oversight requirements *(AI Act, BaFin)*
  - Resilience requirements *(DORA)*
- Initial AI risk assessment covering:
  - Bias risk *(AI Act)*
  - Drift risk *(AI Act, BaFin)*
  - Misuse risk *(DORA, BaFin)*
  - Third-party dependency risk *(DORA, BaFin)*

---

### Governance
- AI use case risk level is classified according to the EU AI Act before design begins
- Systems supporting critical or important financial functions are identified and flagged for stricter DORA controls
- Logging, explainability, human oversight, and resilience are defined as system requirements — not added later
- AI risk assessment (bias, drift, misuse, third-party dependency) is performed and integrated into the ICT risk framework

---

### Regulatory Justification

| Practice | Why It Matters | Source |
|----------|---------------|--------|
| Classify AI use case risk level | Determines level of controls, documentation, and oversight required | EU AI Act |
| Identify support of critical financial function | Such systems fall under stricter operational resilience requirements | DORA |
| Define logging, explainability, human oversight, resilience as requirements | Regulators expect these to be built-in, not added later | AI Act, BaFin |
| Perform initial AI risk assessment | AI risks must be part of the ICT risk framework | DORA, BaFin |

---

### Requirements Traceability
Extends: REQ-01, REQ-02, REQ-03, REQ-04, PM-13, PM-14, PM-15, CRT-01, CRT-02, CRT-04
