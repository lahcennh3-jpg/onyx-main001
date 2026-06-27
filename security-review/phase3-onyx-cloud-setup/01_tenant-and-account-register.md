# Tenant And Account Register

## Authorized Tenant

| Item | Value |
|---|---|
| Authorized tenant URL | Private only; not recorded in public repo |
| Tenant owner | Private only |
| Authorization evidence ID | Pending |
| Test window evidence ID | Pending |
| Emergency stop contact | Private only |

## Required Accounts

| Account Label | Role | Purpose | Status | Private Reference | Notes |
|---|---|---|---|---|---|
| ONYX-ADMIN-001 | Admin | Tenant configuration and evidence capture | Pending | Private account inventory | Use dedicated test/admin account where possible. |
| ONYX-BASIC-001 | Basic | Baseline normal-user retrieval behavior | Pending | Private account inventory | Use synthetic documents only. |
| ONYX-RESTRICTED-001 | Restricted | Access-control and denial-path validation | Pending | Private account inventory | Must not have access to restricted synthetic areas. |
| ONYX-SERVICE-001 | API/service account | API and integration settings review | Pending | Private key/account inventory | Least-privilege and revocable. |

## Account Handling Rules

- Do not publish email addresses, user IDs, service-account IDs, API keys, or screenshots containing account identifiers.
- Store all account identifiers privately.
- Use stable labels in public evidence.
- Revoke or rotate service-account credentials after testing.
