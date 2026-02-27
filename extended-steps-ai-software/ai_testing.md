## AI Step 4: AI-Specific Testing

**Description**  
Extend the standard testing steps with AI-specific validation. Beyond functional accuracy, AI systems must be tested for bias, robustness, and edge cases. Adversarial and misuse testing (e.g., prompt injection) must be performed. Explainability outputs and decision trace logs must be validated. Fallback procedures must be tested for scenarios where model confidence is low or the AI service fails.

> This step augments [Step 4: Developer Testing](../steps/developer_testing.md) and [Step 13: System Testing](../extended-steps/system_testing.md) for AI components.

---

### Inputs
- **AI Models and Components** (from AI Step 3)
- **Test Strategy** (from Step 0 / REQ-14)
- **AI Risk Classification** (from AI Step 1)
- **Explainability Design** (from AI Step 2)
- **Fallback Design** (from AI Step 2)

---

### Output
- Bias testing report *(AI Act)*
- Robustness testing report *(AI Act)*
- Edge case testing results *(AI Act)*
- Adversarial testing report (prompt injection, manipulation) *(DORA, BaFin)*
- Explainability output validation results *(AI Act)*
- Decision trace log validation results *(AI Act)*
- Fallback procedure test results (low confidence, service failure) *(DORA)*

---

### Governance
- AI systems are tested not only for accuracy, but also for bias, robustness, and edge cases — AI must be safe, reliable, and non-discriminatory
- Adversarial and misuse testing (prompt injection, manipulation) is performed — AI systems are new attack vectors
- Explainability outputs and decision trace logs are validated — decisions must be understandable and auditable
- Fallback procedures are tested when model confidence is low or service fails — ensures continuity of critical services

---

### Regulatory Justification

| Practice | Why It Matters | Source |
|----------|---------------|--------|
| Test for bias, robustness, and edge cases (not just accuracy) | AI must be safe, reliable, and non-discriminatory | AI Act |
| Perform adversarial and misuse testing (prompt injection, manipulation) | AI systems are new attack vectors | DORA, BaFin |
| Validate explainability outputs and decision trace logs | Decisions must be understandable and auditable | AI Act |
| Test fallback procedures when model confidence is low or service fails | Ensures continuity of critical services | DORA |

---

### Requirements Traceability
Extends: REQ-14, REQ-15, REQ-16, REQ-17, REQ-18, TEST-03, TEST-04, TEST-05
