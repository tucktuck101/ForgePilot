# FR-047: Include factory validation

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-047 |
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

The system shall include validation mechanisms for the ForgePilot template itself, ensuring that the template contains all required files, directories, and metadata, and that examples are properly marked and no secrets are committed.

## Details

ForgePilot must provide tools or scripts to validate the integrity of the template repository. The factory validation should check that all required files and directories exist; that `AGENTS.md`, `.agents/skills`, `.codex`, `docs`, `templates`, `examples`, `scripts`, `.github`, `README.md`, `CHANGELOG.md`, and `VERSION` are present; that templates and examples follow doc-object style; that no secrets appear; and that examples are clearly marked. This validation can be executed via a script or CI job to ensure the template remains consistent over time.

## Acceptance Criteria

- A factory validation script or workflow exists.
- Validation checks required files and directories.
- Validation checks that skills, templates, and examples are present and well-formed.
- Validation checks for doc-object metadata in docs.
- Validation checks that examples are clearly marked and not used as live artefacts.
- Validation checks that no secrets are committed.

## Notes

Factory validation helps maintain the quality and consistency of the ForgePilot template as it evolves.
