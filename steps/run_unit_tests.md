## Step: Run Unit Tests / Integration Testing (Coverage)

**Description**  
Execute all unit tests and integration tests to validate code correctness and ensure the minimum coverage threshold is met.

---

### Inputs
- **Tests** (unit tests and integration tests)
- **MCP / Command Line Access** for test execution

---

### Output
- Test results: passed/failed
- Code coverage report *(REQ-09)*
- Minimum coverage threshold enforced *(DEV-05)*

---

### Governance
- Unit tests written for new and changed code *(REQ-08)*
- Minimum unit test coverage threshold enforced *(REQ-09)*
- Integration tests executed *(REQ-16)*
- Build fails on unit test errors *(REQ-11)*
- Minimum unit test coverage enforced per DORA ICT resilience *(DEV-05)*
- All unit tests must pass before merge approval *(TEST-01)*

---

### Requirements Traceability
REQ-08, REQ-09, REQ-11, REQ-16, DEV-05, TEST-01
