## Step: Run Quality Steps (Lint, Formatting)

**Description**  
Execute static code analysis, linting, and formatting checks to ensure the code meets the defined quality standards and coding conventions.

---

### Inputs
- **Quality Steps** (lint rules, formatting rules)
- **MCP / Command Line Access** for execution

---

### Output
- Quality check results: passed/failed
- Lint report *(REQ-06)*
- Static analysis report *(DEV-02)*
- Secret scanning report *(DEV-03)*

---

### Governance
- Coding standards defined and shared *(REQ-05)*
- Static code analysis (linting) is mandatory *(REQ-06)*
- Build fails on linting errors *(REQ-11)*
- Quality objectives defined and enforced through quality gates *(PM-21)*
- Static code analysis executed on every commit *(DEV-02)*
- All code must comply with coding standards *(DEV-01)*
- Secrets and credentials must not be stored in source code *(DEV-03)*

---

### Requirements Traceability
REQ-05, REQ-06, REQ-11, PM-21, DEV-01, DEV-02, DEV-03
