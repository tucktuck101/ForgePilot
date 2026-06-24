# FR-052: Run relevant project checks

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-052 |
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

The system shall run relevant tests, linting, formatting, type checks, build checks, and smoke tests during each sprint to verify work quality.

## Details

For each scoped sprint, ForgePilot must execute the appropriate validation commands for the project's stack. This includes running unit tests, integration tests, and end-to-end tests where applicable; running linters and formatters; performing type checks; ensuring the project builds correctly; and conducting smoke tests for deployment readiness. The system should interpret and report failures, fix those caused by current work, and document unrelated failures.

## Acceptance Criteria

- The system identifies and runs relevant validation commands for the project's stack during each sprint.
- Test and validation results are recorded in `docs/delivery/test-reports.md`.
- Failures caused by the current sprint are fixed before marking the sprint complete.
- Unrelated or pre-existing failures are documented with clear notes.

## Notes

This requirement ensures that ForgePilot delivers high-quality work by verifying code against tests and quality checks before considering a sprint done.
