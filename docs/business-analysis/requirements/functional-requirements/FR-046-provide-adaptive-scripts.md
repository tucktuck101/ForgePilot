# FR-046: Provide adaptive scripts

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-046 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall include adaptive scripts for setup, validation, testing, linting, formatting, and smoke testing that detect the project's stack and delegate to existing commands when available.

## Details

ForgePilot must provide a set of scripts under `scripts/` that can adapt to the detected stack of the repository. The scripts should handle setup, validation, unit tests, integration tests, linting, formatting, and smoke testing. They should detect common package managers and existing scripts, and fall back to sensible defaults. Scripts must fail safely with helpful messages if the expected tools are not available.

## Acceptance Criteria

- A `scripts` directory exists in the template.
- Scripts detect common package managers and project types (e.g., npm/yarn/pip/go modules).
- Scripts delegate to existing repository commands when available.
- Scripts provide setup, validate, test, lint, format, and smoke-test functions.
- Scripts fail safely with clear error messages when a required tool is unavailable.

## Notes

This requirement ensures that ForgePilot projects have a consistent and adaptable build and validation toolchain across multiple stacks.
