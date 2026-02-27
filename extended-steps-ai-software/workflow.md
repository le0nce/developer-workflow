# AI SDLC Workflow (AI Software Extension)

This workflow extends the standard SDLC with AI-specific steps required by the **EU AI Act**, **DORA**, and **BaFin** for software that uses AI. Each AI step augments a corresponding standard step and adds regulatory controls specific to AI systems in financial services.

```mermaid
flowchart TD
    B1["B1. Project Initiation &\nBusiness Alignment"] --> B2["B2. Scope, Planning &\nStakeholder Management"]
    B2 --> P["0. Planning /\nRequirements Review"]

    P --> AI1[" AI Step 1:\nRequirements &\nAI Risk Classification"]

    AI1 --> AI2[" AI Step 2:\nArchitecture & Design\nfor AI Systems"]

    AI2 --> A["1. Tasks\n(Approved Ticket)"]
    A --> B["2. Create New Branch\nin Repo"]

    B --> C["3. Coding"]
    C --> AI3[" AI Step 3:\nAI-Specific Development\nPractices"]

    AI3 --> D["4. Developer Testing"]
    D --> AI4a[" AI Step 4:\nAI-Specific Testing\n(Developer Level)"]
    AI4a --> E{"Quality Gates"}

    E --> F["5. Run Unit Tests /\nIntegration Testing\n(Coverage)"]
    E --> G["6. Run Quality Steps\n(Lint, Formatting)"]

    F --> H["7. Run Pre-Commit\nSteps (Git Hook)"]
    G --> H

    H -->|"Committed"| I["8. Run Commit\nPipeline"]
    H -->|"Denied"| C

    I --> J["9. Create MR"]

    J --> K["10. MR Pipeline"]

    K -->|"All checks pass"| L["11. Code Review\n(4-Eye Principle)"]
    K -->|"Checks fail"| C

    L -->|"Approved"| M["12. Merge to Target"]
    L -->|"Changes requested"| C

    M --> S["13. System Testing"]
    S --> AI4b[" AI Step 4:\nAI-Specific Testing\n(System Level)"]

    AI4b -->|"Passed"| R["14. Release"]
    AI4b -->|"Defects found"| C

    R --> AI5[" AI Step 5:\nAI-Specific Deployment"]

    AI5 --> PR["15. Post-Release"]
    PR --> AI6[" AI Step 6:\nAI Operations &\nMonitoring"]

    AI6 --> N(("Done"))

    style AI1 fill:#e1f5fe,stroke:#0288d1
    style AI2 fill:#e1f5fe,stroke:#0288d1
    style AI3 fill:#e1f5fe,stroke:#0288d1
    style AI4a fill:#e1f5fe,stroke:#0288d1
    style AI4b fill:#e1f5fe,stroke:#0288d1
    style AI5 fill:#e1f5fe,stroke:#0288d1
    style AI6 fill:#e1f5fe,stroke:#0288d1
```

---

## AI Steps Overview

| AI Step | Standard Step Augmented | Regulatory Source | Description |
|---------|------------------------|:-----------------:|-------------|
| [AI Step 1: Requirements & AI Risk Classification](ai_requirements_classification.md) | Step 0 (Planning) | AI Act, DORA, BaFin | Classify AI risk level, identify critical functions, define AI-specific requirements |
| [AI Step 2: Architecture & Design](ai_architecture_design.md) | Between Step 0 and Step 1 | AI Act, DORA, BaFin | Design failover, environment separation, explainability, human-in-the-loop, data lineage |
| [AI Step 3: AI Development Practices](ai_development.md) | Step 3 (Coding) | AI Act, DORA, BaFin | Version models/prompts, secure ML coding, controlled repositories |
| [AI Step 4: AI Testing](ai_testing.md) | Steps 4, 13 (Testing) | AI Act, DORA, BaFin | Bias/robustness testing, adversarial testing, explainability validation, fallback testing |
| [AI Step 5: AI Deployment](ai_deployment.md) | Step 14 (Release) | DORA, BaFin | Formal model promotion, rollback capability, segregation of duties |
| [AI Step 6: AI Operations & Monitoring](ai_operations_monitoring.md) | Step 15 (Post-Release) | AI Act, DORA, BaFin | Drift monitoring, AI decision logging, SIEM integration, incident classification |
