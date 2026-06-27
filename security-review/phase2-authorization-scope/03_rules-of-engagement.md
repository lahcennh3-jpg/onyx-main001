# Rules Of Engagement

## Required Before Testing

| Requirement | Status | Notes |
|---|---|---|
| Written authorization | Pending | Must identify the authorization owner. |
| Authorized tenant URL | Pending | Store privately only. |
| Test window | Pending | Include timezone and blackout periods. |
| Emergency stop contact | Pending | Store privately only. |
| Allowed accounts | Pending | Use dedicated test accounts. |
| Allowed API keys | Pending | Use least-privilege test keys only. |
| Allowed test profiles | Pending | Must be listed below. |
| Forbidden tests | Drafted | See forbidden tests section. |
| Cleanup duties | Drafted | See cleanup section. |
| Key-revocation duties | Drafted | See key-revocation section. |

## Request Limits

| Limit | Default |
|---|---|
| Maximum request rate | 1 request per 5 seconds unless written authorization allows more |
| Maximum concurrent sessions | 1 unless written authorization allows more |
| Maximum synthetic documents | 10 unless written authorization allows more |
| Maximum test duration | Within approved test window only |
| Stop condition | Any unexpected production impact, account lockout, security alert, or emergency stop request |

## Allowed Test Profiles

| Profile | Status | Conditions |
|---|---|---|
| Static documentation review | Allowed | Redacted-safe artifacts only |
| Synthetic RAG access-control tests | Pending | Requires written authorization |
| Synthetic prompt-injection tests | Pending | Requires written authorization |
| Retrieval leakage tests using synthetic data | Pending | Requires written authorization |
| Connector permission tests | Pending | Requires written authorization and connector allowlist |
| Agent/tool-use safety tests | Pending | Requires written authorization and tool allowlist |

## Forbidden Tests

- Credential attacks
- Brute force
- Destructive testing
- Infrastructure scanning
- Denial-of-service testing
- Phishing or social engineering
- Malware upload
- Testing other tenants
- Touching unauthorized connectors
- Uploading real sensitive data
- Real external tool actions
- Bypassing payment, tenant, or access controls outside the authorized test design

## Cleanup Duties

- Delete synthetic documents after testing.
- Delete test conversations and transcripts where supported.
- Remove temporary test users or service accounts.
- Remove temporary connector configurations.
- Archive redacted evidence only.
- Store raw evidence privately.
- Record cleanup completion in the command log.

## Key-Revocation Duties

- Revoke test API keys after testing.
- Rotate any exposed or suspected-exposed key immediately.
- Remove test secrets from local machines and cloud workspaces.
- Record revocation evidence privately.
- Publish only redacted-safe revocation confirmation.
