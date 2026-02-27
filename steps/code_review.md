## Step: Code Review

**Description**  
Conduct a thorough code review following the 4-eye principle. An agent may assist by creating MR comments, but final approval must come from a human reviewer. No self-approval is permitted.

---

### Inputs
- **Merge Request** (with all pipeline checks passing)
- **MR Comments and Discussion**
- **Pipeline Results** (all green)

---

### Output
- Code review completed
- MR comments addressed and resolved
- Review approval granted *(REQ-21)*
- QA approval granted (if applicable) *(REQ-22)*

---

### Governance
- **4-Eye Principle** enforced — code review by at least one other developer *(REQ-21)*
- All checks green (pipeline, conflicts, approved, comments resolved) *(REQ-23)*
- MR Review by agent — agent creates MR comments for reviewer consideration
- **No self-approval** permitted *(REQ-21)*
- QA approval required before merge (if applicable) *(REQ-22)*
- **NO AI approval** — final approval must be human

---

### Requirements Traceability
REQ-21, REQ-22, REQ-23
