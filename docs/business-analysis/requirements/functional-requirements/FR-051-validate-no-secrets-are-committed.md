# FR-051: Validate no secrets are committed

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-051 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall validate that no secrets, API keys, tokens, credentials, or real `.env` files are committed to the repository.

## Details

Validation should scan the repository for likely secrets or sensitive values, such as high-entropy strings, known credential patterns, or `.env` files with values other than placeholders. It should ensure that `.env.example` exists with placeholder values, that `.env` is not committed, and that `.gitignore` includes `.env` and other secret-bearing files. If any secrets are detected, the validation must fail and alert the user.

## Acceptance Criteria

- Validation scans for common secret patterns and high-entropy tokens in the repository.
- `.env` or other environment files containing real values are not present in version control.
- `.env.example` exists and uses placeholder values.
- `.gitignore` includes `.env` and any other secret-bearing files.
- Validation fails with an informative message if secrets or real credentials are found.

## Notes

This requirement helps prevent accidental leakage of secrets and credentials in ForgePilot projects.
