# FR-059: Never commit secrets

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-059 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall ensure that real secrets, API keys, tokens, and credentials are never committed to version control.

## Details

ForgePilot must prevent secrets from being added to the repository by using `.gitignore` to exclude `.env` and other secret files, scanning commits for high-entropy strings and known credential patterns, and using placeholder values in examples and templates. Codex must never print or log secrets in outputs or documentation. This requirement complements validation but emphasises proactive prevention.

## Acceptance Criteria

- `.gitignore` lists secret files such as `.env` and other environment-specific files containing secrets.
- The system or developer workflow includes commit-time scanning to prevent secrets from being committed.
- Examples and templates use placeholder values instead of real secrets.
- Codex does not emit secrets in logs or documentation.

## Notes

Preventing secrets from entering version control reduces security risks and simplifies repository compliance.
