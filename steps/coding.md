## Step: Coding

**Description**  
Implement the approved task by writing production code and corresponding tests in the target repository, following coding conventions and secure coding practices defined in Agent.md.

---

### Inputs
- **Task (Ticket with Requirements, Definition of Done, Context)**
  - Functional requirements documented and approved *(REQ-01)*
  - Acceptance criteria / Definition of Done defined *(REQ-03)*
  - Risks and dependencies identified *(REQ-04)*
- **Agent.md**
  - Coding conventions and standards *(REQ-05)*
- **Access to Repo**
  - All required repositories accessible

---

### Output
- Production code for the task is created
- Tests written (following naming and reference conventions for tests) *(REQ-08)*
- Code follows secure coding practices *(REQ-07)*
- Code complies with coding standards *(DEV-01)*
- No secrets or credentials stored in source code *(DEV-03)*
- Unit tests written for all new or changed code *(DEV-04)*

---

### Governance
- Coding standards defined, shared, and enforced *(REQ-05)*
- Static code analysis (linting) is mandatory *(REQ-06)*
- Code follows secure coding practices *(REQ-07)*
- Unit tests written for new and changed code *(REQ-08)*
- All code must comply with coding standards *(DEV-01)*
- Secrets and credentials must not be stored in source code *(DEV-03)*
- Unit tests written for all new or changed code *(DEV-04)*
- **IF AI is used by Developer:**
  - Code must be reviewed and validated by the developer

---

### Requirements Traceability
REQ-01, REQ-03, REQ-04, REQ-05, REQ-06, REQ-07, REQ-08, DEV-01, DEV-03, DEV-04
