## AI Step 5: AI-Specific Deployment

**Description**  
Extend the standard release and deployment steps with AI-specific controls. AI model changes are considered controlled ICT changes requiring formal approval workflows. Rollback capability to previous model versions must be maintained. Segregation of duties between development and production release must be enforced.

> This step augments [Step 14: Release](../extended-steps/release.md) for AI model deployments.

---

### Inputs
- **AI Test Results** (from AI Step 4)
- **Versioned Model Artifacts** (from AI Step 3)
- **Release Approval Workflow** (from Step 14 / REL-01)
- **Rollback Strategy** (from Step 14 / REL-03)
- **RACI Matrix** (from Step B1 / GOV-03)

---

### Output
- Formal model promotion approval record *(DORA)*
- Rollback capability verified for previous model versions *(DORA)*
- Segregation of duties evidence (development vs. production release) *(BaFin, DORA)*

---

### Governance
- Formal approval workflows are used before promoting AI models to production — AI model changes are considered controlled ICT changes
- Rollback capability to previous model versions is maintained and tested for operational resilience and incident recovery
- Segregation of duties between development and production release is enforced to reduce risk of unauthorized or unsafe changes

---

### Regulatory Justification

| Practice | Why It Matters | Source |
|----------|---------------|--------|
| Use formal approval workflows before promoting models to production | AI model changes are considered controlled ICT changes | DORA |
| Maintain rollback capability to previous model versions | Required for operational resilience and incident recovery | DORA |
| Ensure segregation of duties between development and production release | Reduces risk of unauthorized or unsafe changes | BaFin, DORA |

---

### Requirements Traceability
Extends: REQ-24, REQ-25, REQ-26, REQ-27, REL-01, REL-03, REL-04, GOV-03, DEP-01
