# FR-052: Run relevant project checks

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index](index.md) |
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
