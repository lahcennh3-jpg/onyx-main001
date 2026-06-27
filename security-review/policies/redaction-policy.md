# Redaction Policy

## Redact Before Publishing

Redact:

- Names of tenants, customers, users, and organizations
- Email addresses
- Account IDs
- Tenant URLs
- Internal URLs
- IP addresses, unless already public and approved for publication
- API keys, tokens, cookies, passwords, and session values
- Source document contents that are not approved for publication
- Raw prompts and responses containing sensitive data
- Connector names or paths that expose private systems

## Redaction Method

Use stable placeholders:

| Sensitive Item | Placeholder |
|---|---|
| Tenant URL | `[REDACTED_TENANT_URL]` |
| User email | `[REDACTED_EMAIL]` |
| API token | `[REDACTED_TOKEN]` |
| Customer name | `[REDACTED_CUSTOMER]` |
| Internal path | `[REDACTED_INTERNAL_PATH]` |
| Source document | `[REDACTED_SOURCE_DOCUMENT]` |

## Review Checklist

- No secrets are visible.
- No session material is visible.
- No tenant URL is visible.
- No private customer or user data is visible.
- No raw logs are included.
- File names do not reveal sensitive target details.
- The artifact has passed a secret scan.
