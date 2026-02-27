## Step: Merge to Target

**Description**  
Merge the approved merge request into the target branch after all checks, reviews, and approvals are complete. This is the final gate before code enters the main codebase.

---

### Inputs
- **Approved Merge Request**
  - All pipeline checks green *(REQ-23)*
  - Code review approved (4-eye principle) *(REQ-21)*
  - QA approval granted (if applicable) *(REQ-22)*
  - All comments resolved
  - No merge conflicts

---

### Output
- Code merged into target branch
- Merge record created
- CI pipeline triggered on target branch (if configured)
- Artifacts: merge commit reference, pipeline logs

---

### Governance
- 4-Eye Principle enforced *(REQ-21)*
- All CI checks must pass before merge *(REQ-23)*
- QA approval verified (if applicable) *(REQ-22)*
- No unresolved conflicts or comments
- No self-approval permitted
- Defects logged and tracked if issues found *(REQ-19)*
- Protected branches prevent direct commits *(MR-03)*
- Automated quality checks must pass before merge *(MR-02)*

---

### Requirements Traceability
REQ-19, REQ-21, REQ-22, REQ-23, MR-02, MR-03
