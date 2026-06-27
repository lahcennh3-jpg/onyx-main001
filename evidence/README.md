# Evidence Folder Structure

This folder is for public-safe evidence artifacts only.

## Public-Safe Structure

| Path | Purpose | Public Repo |
|---|---|---|
| `evidence/public-redacted/` | Redacted-safe evidence artifacts | Yes |
| `evidence/templates/` | Evidence templates and empty forms | Yes |
| `security-review/logs/` | Sanitized command and communication logs | Yes |
| `security-review/policies/` | Evidence handling and redaction policies | Yes |
| `security-review/templates/` | Chain-of-custody and index templates | Yes |

## Private-Only Structure

These paths are intentionally ignored by `.gitignore` and must not be committed:

| Path | Purpose | Public Repo |
|---|---|---|
| `raw-evidence/` | Raw collected evidence | No |
| `evidence/raw/` | Raw screenshots, transcripts, and captures | No |
| `evidence/private/` | Sensitive working evidence | No |
| `evidence/http-logs/` | HTTP logs and HAR files | No |
| `security-review-evidence/raw/` | Raw review evidence | No |

## Publication Rule

Only publish an artifact after redaction review and secret scan pass.
