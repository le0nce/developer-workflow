## AI Step 6: AI-Specific Operations & Monitoring

**Description**  
Extend the standard post-release step with AI-specific operational monitoring and incident management. AI behaviour changes over time and requires continuous monitoring for model drift and performance degradation. All AI inputs, outputs, decisions, and human overrides must be logged. AI systems must be integrated into security monitoring infrastructure. Major AI failures must be classified as ICT incidents with proper escalation and reporting.

> This step augments [Step 15: Post-Release](../extended-steps/post_release.md) for AI systems in production.

---

### Inputs
- **Production AI System** (deployed)
- **Monitoring Dashboards** (from Step 15 / REQ-28)
- **Incident Management Process** (from Step 15 / OPS-02)
- **SIEM / Anomaly Detection Infrastructure** *(DORA)*
- **AI Risk Classification** (from AI Step 1)

---

### Output
- Model drift monitoring dashboards and alerts *(AI Act, BaFin)*
- Performance degradation detection reports *(AI Act, BaFin)*
- AI decision logs (inputs, outputs, decisions, overrides) *(AI Act, DORA)*
- AI integration into SIEM / anomaly detection *(DORA)*
- AI incident classification and escalation records *(DORA)*

---

### Governance
- Continuous monitoring for model drift and performance degradation is active — AI behaviour changes over time and may create risk
- AI inputs, outputs, decisions, and overrides are logged for incident analysis and auditability
- AI systems are integrated into security monitoring (SIEM, anomaly detection) as part of the institution's ICT infrastructure
- Major AI failures are classified as ICT incidents and follow escalation/reporting procedures — some AI incidents may be reportable to supervisors

---

### Regulatory Justification

| Practice | Why It Matters | Source |
|----------|---------------|--------|
| Continuously monitor for model drift and performance degradation | AI behaviour changes over time and may create risk | AI Act, BaFin |
| Log AI inputs, outputs, decisions, and overrides | Required for incident analysis and auditability | AI Act, DORA |
| Integrate AI systems into security monitoring (SIEM, anomaly detection) | AI is part of the institution's ICT infrastructure | DORA |
| Classify major AI failures as ICT incidents and follow escalation/reporting | Some AI incidents may be reportable to supervisors | DORA |

---

### Requirements Traceability
Extends: REQ-28, REQ-29, REQ-30, DEP-03, OPS-01, OPS-02, OPS-03, AUD-01
