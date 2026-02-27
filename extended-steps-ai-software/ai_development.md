## AI Step 3: AI-Specific Development Practices

**Description**  
Extend the standard coding step with AI-specific development practices. Models, training data references, and prompts must be versioned like source code. Secure coding practices must cover ML components and APIs. Models and artifacts must be stored in access-controlled repositories. Prompts and model configurations must be treated as controlled configuration items.

> This step augments [Step 3: Coding](../steps/coding.md) for AI components.

---

### Inputs
- **AI Architecture Design** (from AI Step 2)
- **Coding Standards** (from Step B1 / GOV-02)
- **Access Control Policy** (from Step B1 / GOV-04)
- **Model Repository / Artifact Store**

---

### Output
- Models versioned in controlled repository *(AI Act, BaFin)*
- Training data references versioned alongside models *(AI Act, BaFin)*
- Prompts and prompt templates versioned *(BaFin)*
- Secure ML component and API code *(DORA)*
- Access-restricted model and artifact repositories *(DORA, BaFin)*
- Prompts and model configurations tracked as controlled configuration items *(BaFin)*

---

### Governance
- Models, training data references, and prompts are versioned like source code for reproducibility and traceability
- Secure coding practices are applied to ML components and APIs as part of the ICT attack surface
- Models and artifacts are stored in controlled repositories with access restrictions to prevent unauthorized modification or model poisoning
- Prompts and model configurations are treated as controlled configuration items — prompt changes can alter system behaviour and risk

---

### Regulatory Justification

| Practice | Why It Matters | Source |
|----------|---------------|--------|
| Version models, training data references, and prompts like source code | AI artefacts must be reproducible and traceable | AI Act, BaFin |
| Use secure coding practices for ML components and APIs | AI components are part of the ICT attack surface | DORA |
| Store models in controlled repositories with access restrictions | Prevents unauthorized modification or model poisoning | DORA, BaFin |
| Treat prompts and model configurations as controlled configuration items | Prompt changes can alter system behaviour and risk | BaFin |

---

### Requirements Traceability
Extends: REQ-05, REQ-07, REQ-08, REQ-12, REQ-13, DEV-01, DEV-03, GOV-04, CI-04
