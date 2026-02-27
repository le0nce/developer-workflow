## Step: Run Commit Pipeline

**Description**  
Execute the automated CI pipeline triggered by a commit. The pipeline builds the project, runs all checks, and produces versioned artifacts. Infrastructure and architecture are validated according to DORA definitions.

---

### Inputs
- **Committed Code** (passing pre-commit checks)
- **CI Pipeline Configuration**

---

### Output
- Build result: success/failure
- Versioned build artifacts *(REQ-12)*
- CI build logs *(REQ-10)*

---

### Governance
- Automated build pipeline configured *(REQ-10)*
- Build fails on linting or unit test errors *(REQ-11)*
- Build artifacts are versioned *(REQ-12)*
- Dependencies are managed and locked *(REQ-13)*
- Infrastructure and architecture validated according to DORA definitions

---

### Requirements Traceability
REQ-10, REQ-11, REQ-12, REQ-13
