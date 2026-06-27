# GitHub And Evidence Repo Policy

## Repository Visibility

- Repository: `lahcennh3-jpg/onyx-main001`
- Confirmed visibility on 2026-06-27: public
- Public repository use: redacted-safe project artifacts only
- Raw evidence location: private storage outside this public repository

## Publish Rules

Publish only:

- Redacted reports
- Evidence indexes
- Templates
- Policies
- Sanitized command logs
- Sanitized communication logs
- Redacted screenshots or transcripts after review

Do not publish:

- `.env` files
- API keys
- Private keys
- Cookies
- Session tokens
- Raw screenshots
- Raw transcripts
- HTTP logs
- HAR files
- Tenant URLs
- Customer identifiers
- Source archives
- Unredacted connector outputs
- Unredacted prompts or responses containing sensitive data

## Branching Rule

All project evidence changes must be prepared on a project branch before merge into the default branch.

Project branch for this setup:

- `codex/evidence-repo-setup`

## Pre-Commit Rule

Before every commit or upload, run a secret scan on the files being published. If any finding appears, stop, redact, rescan, and only then publish.
