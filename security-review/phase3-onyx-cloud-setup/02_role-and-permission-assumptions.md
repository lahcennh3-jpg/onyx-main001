# Role And Permission Assumptions

| ID | Account Label | Assumption | Validation Method | Status |
|---|---|---|---|---|
| RPA-001 | ONYX-ADMIN-001 | Admin can configure tenant settings, document areas, connectors, logging, and API/service settings. | Redacted tenant settings screenshots and settings export where available | Pending |
| RPA-002 | ONYX-BASIC-001 | Basic account can access only allowed synthetic document areas. | Retrieval tests with synthetic documents | Pending |
| RPA-003 | ONYX-RESTRICTED-001 | Restricted account cannot retrieve restricted synthetic documents. | Negative retrieval tests with synthetic documents | Pending |
| RPA-004 | ONYX-SERVICE-001 | API/service account has only the minimum required API permissions. | API settings review and key scope review | Pending |

## Permission Assumption Rules

- Treat all role capabilities as assumptions until validated.
- Record validation evidence privately first.
- Publish only redacted-safe summaries.
- If actual permissions differ from assumptions, update this register and the not-tested register.
