## Step: Run Pre-Commit Steps (Git Hook)

**Description**  
Execute pre-commit hooks that validate the commit before it is accepted. This includes linting, format checks, build verification, and running existing and new test cases automatically.

---

### Inputs
- **Commit Message** (markdown format)
- **Commit** (staged changes)

---

### Output
- Commit accepted or denied
- Validation results:
  - Lint and format check *(REQ-06)*
  - Build success *(REQ-10)*
  - Existing and new test cases automatically tested *(REQ-08)*
  - Static analysis report *(DEV-02)*
  - Secret scanning result *(DEV-03)*

---

### Governance
- Static code analysis (linting) is mandatory *(REQ-06)*
- Unit tests written for new and changed code *(REQ-08)*
- Automated build pipeline configured *(REQ-10)*
- Build fails on linting or unit test errors *(REQ-11)*
- Static code analysis executed on every commit *(DEV-02)*
- Secrets and credentials must not be stored in source code *(DEV-03)*

---

### Requirements Traceability
REQ-06, REQ-08, REQ-10, REQ-11, DEV-02, DEV-03
