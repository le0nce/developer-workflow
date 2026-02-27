## AI Step 2: Architecture & Design for AI Systems

**Description**  
Extend the system architecture and design phase with AI-specific considerations mandated by the EU AI Act, DORA, and BaFin. This includes designing for failover when AI models are unavailable, strict environment separation, explainability mechanisms, human-in-the-loop intervention points, and full data lineage traceability.

> This step introduces a new design gate between [Step 0: Planning](../extended-steps/planning_requirements_review.md) and [Step 1: Tasks](../steps/task.md) for AI-enabled software.

---

### Inputs
- **AI Risk Classification** (from AI Step 1)
- **System Architecture Documents**
- **AI-Specific Requirements** (logging, explainability, human oversight, resilience)
- **DORA ICT Risk Framework**

---

### Output
- Failover and fallback design for AI model/service unavailability *(DORA)*
- Environment separation plan (training / testing / production) *(BaFin, DORA)*
- Explainability design (model metadata, feature traceability) *(AI Act)*
- Human-in-the-loop intervention point design *(AI Act, BaFin)*
- Data lineage architecture (source → model → output) *(AI Act, BaFin)*

---

### Governance
- Failover and fallback mechanisms are designed so that financial services remain operational even if AI fails
- Training, testing, and production environments are strictly separated to prevent data leakage and uncontrolled model changes
- Explainability mechanisms (model metadata, feature traceability) are designed into the system for transparency and auditability in high-risk AI
- Human-in-the-loop intervention points are designed so humans can oversee and override automated decisions
- Full data lineage from source → model → output is architecturally ensured for traceability of AI decisions

---

### Regulatory Justification

| Practice | Why It Matters | Source |
|----------|---------------|--------|
| Design failover/fallback if AI model is unavailable | Financial services must remain operational even if AI fails | DORA |
| Separate training, testing, and production environments | Prevents data leakage and uncontrolled model changes | BaFin, DORA |
| Implement explainability mechanisms | Required for transparency and auditability in high-risk AI | AI Act |
| Design human-in-the-loop intervention points | Humans must be able to oversee and override automated decisions | AI Act, BaFin |
| Ensure full data lineage (source → model → output) | Supervisors expect traceability of AI decisions | AI Act, BaFin |

---

### Requirements Traceability
Extends: REQ-02, REQ-04, REQ-07, CRT-03, GOV-01
