# Scope Document

## In Scope

| Area | Status | Conditions |
|---|---|---|
| Evidence repository setup | In scope | Redacted-safe artifacts only |
| Authorization and scope documentation | In scope | Templates and placeholders only |
| Static source review preparation | In scope | No secrets or source archives committed |
| RAG access-control readiness checks | Conditional | Requires written authorization and allowed accounts |
| Enterprise search connector permission review | Conditional | Requires written authorization and connector scope |
| Prompt-injection and retrieved-document injection testing | Conditional | Requires written authorization and synthetic document permission |
| Retrieval leakage testing | Conditional | Requires written authorization and approved synthetic dataset |
| Agent action and tool-use safety testing | Conditional | Requires written authorization and tool/action allowlist |

## Out Of Scope By Default

- Credential attacks
- Brute force
- Destructive testing
- Infrastructure scanning
- Testing other tenants
- Touching unauthorized connectors
- Uploading real sensitive data
- Real external tool actions
- Claiming full enterprise audit without full enterprise scope, remediation, and retest proof

## Scope Change Rule

Any scope change must be approved in writing and recorded in the communication log before testing.
