# Assumptions Register

| ID | Assumption | Impact If False | Owner | Status |
|---|---|---|---|---|
| ASM-001 | The public repository must contain only redacted-safe artifacts. | Sensitive data could be exposed. | Tester/operator | Active |
| ASM-002 | Raw evidence will be stored privately outside the public repository. | Chain of custody and confidentiality could fail. | Tester/operator | Active |
| ASM-003 | Live testing is not authorized until written authorization is recorded. | Testing could exceed permission boundaries. | Authorization owner | Active |
| ASM-004 | Only synthetic or explicitly approved data will be used. | Real sensitive data could be mishandled. | Data owner | Active |
| ASM-005 | Test accounts and API keys will be least-privilege and revocable. | Test impact could exceed intended scope. | Tenant owner | Active |
