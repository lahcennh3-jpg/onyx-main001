# Evidence Handling Policy

## Purpose

This policy defines how evidence is collected, stored, redacted, published, and retained for the Enterprise-style RAG Security Readiness Demo.

## Evidence Classes

| Class | Examples | Storage | Public Repo |
|---|---|---|---|
| Raw evidence | Raw screenshots, raw transcripts, HTTP logs, HAR files | Private only | No |
| Sensitive working notes | Tenant URLs, account names, connector details | Private only | No |
| Redacted artifacts | Sanitized reports, sanitized screenshots, evidence index | Public-safe folder after review | Yes |
| Templates and policies | Blank forms, procedures, checklists | Public repo | Yes |

## Handling Rules

- Store raw evidence outside the public repository.
- Redact sensitive identifiers before publishing.
- Keep command logs sanitized.
- Keep communication logs sanitized.
- Hash important evidence files when preserving chain of custody.
- Record who collected evidence, when it was collected, and where it is stored.
- Do not publish evidence until a secret scan has passed.

## Minimum Evidence Metadata

Each evidence item should include:

- Evidence ID
- Date and time collected
- Collector
- Source system or test area
- Sensitivity classification
- Storage location
- Hash, when applicable
- Redaction status
- Review status
