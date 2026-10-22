Markdown
# Contributing to Division 003 (Judicial Foundation)
**BEAST System 3.0**

---

## 1. Overview
Thank you for contributing to **Division 003** of **BEAST System 3.0**. Because this repository manages system-wide legal architecture, compliance standards, and cryptographic audit rails, all contributions must undergo strict automated verification and multi-signature governance review.

---

## 2. Contribution Workflow

1. **Branching Strategy:**
   * Create a feature or fix branch from `main` (e.g., `feat/update-schema` or `fix/validation-script`).
2. **Local Integrity Verification:**
   * Before committing, always run the repository validation script to ensure schema and file structure integrity:
     ```bash
     python3 scripts/verify_integrity.py
     ```
   * Run the test suite via `pytest` to confirm all validation checks pass:
     ```bash
     pytest tests/
     ```
3. **Pull Request Requirements:**
   * All pull requests must pass the GitHub Actions CI validation pipeline (`.github/workflows/validate.yml`).
   * Changes to core specifications (`DIVISION_003_JUDICIAL_FOUNDATION.md` or `governance/founding_rulings.md`) require multi-signature approval from core maintainers.

---

## 3. Code Quality Standards
* **Python Code:** Must be PEP 8 compliant, fully typed where possible, and include accompanying unit tests under `tests/`.
* **JSON Schemas:** Any modification to `schemas/case_schema.json` must be backward compatible and validated against current sample case records.

---
*Division 003 — Contributor Guidelines*
File Name: SECURITY.md
Markdown
# Security Policy & Incident Response
**Division 003 — Judicial Foundation**  
**BEAST System 3.0**

---

## 1. Reporting a Vulnerability
If you discover a security vulnerability, state consensus flaw, or cryptographic integrity bypass within Division 003 infrastructure, please report it directly through secure channels rather than public issues.

* **Security Contact:** `security@beast-system-3.0.internal` (Encrypted PGP Key available upon request)
* **Response Window:** Initial triage and SEV-1 assessment within 2 hours of receipt.

---

## 2. Emergency Halt Protocol (SEV-1)
In the event of a critical state corruption or unauthorized bypass of compliance verification:
1. The automated Compliance Engine will immediately emit a `SEV-1` alert.
2. System nodes will invoke the **Emergency Halt Protocol**, freezing cross-division transaction pipelines.
3. Division 003 judicial council will convene to review the incident, execute state rollbacks, and issue an emergency ruling update.

---
*Division 003 — System Security & Incident Governance*
