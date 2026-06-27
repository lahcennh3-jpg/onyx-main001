# Evidence Naming Convention

## Format

Use this format for evidence files:

`YYYYMMDD_phase-topic_evid-NNN_description_redacted.ext`

## Examples

- `20260627_phase1-scope_evid-001_repo-visibility_redacted.md`
- `20260627_phase1-scope_evid-002_command-log_redacted.md`
- `20260627_phase3-static-review_evid-010_semgrep-summary_redacted.json`

## Rules

- Use lowercase names.
- Use hyphens instead of spaces.
- Include `redacted` only after review.
- Never include tenant names, customer names, user emails, tokens, internal URLs, or hostnames in file names.
- Keep raw evidence in private storage and use a private evidence ID to reference it.
