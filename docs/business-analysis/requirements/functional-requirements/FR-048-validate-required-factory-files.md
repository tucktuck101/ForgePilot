# FR-048: Validate required factory files

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-048 |
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

The system shall validate that all required factory files and directories are present in the ForgePilot template.

## Details

ForgePilot must include a validation step that ensures the presence of all mandatory files and directories needed for proper operation. These include `AGENTS.md`, the `.agents/skills` directory with skill files, `.codex` configuration, the `docs/` hierarchy with required subfolders, templates, examples, scripts, `.github` workflows, and versioning files. Missing or misnamed files should cause validation to fail with clear error messages.

## Acceptance Criteria

- Validation checks for the existence of all mandatory files and directories in the template.
- Validation fails if any required file or folder is missing or renamed.
- Validation output clearly lists missing or misnamed items.

## Notes

This requirement ensures the completeness of the ForgePilot template structure before it is used.
