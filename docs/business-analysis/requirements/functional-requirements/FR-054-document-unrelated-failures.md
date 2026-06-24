# FR-054: Document unrelated failures

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-054 |
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

The system shall document test failures or issues that are unrelated to changes introduced in the current sprint without attempting to fix them.

## Details

When tests or quality checks fail due to pre-existing issues or external factors outside the scope of the current sprint, Codex should record these failures in sprint notes and test reports with context and reasons. Codex should not attempt to fix these unrelated failures unless they impede progress or are explicitly included in the sprint scope.

## Acceptance Criteria

- The system distinguishes between failures caused by current changes and failures that are unrelated or pre-existing.
- Unrelated failures are recorded with context in `docs/delivery/current-sprint.md` and `docs/delivery/test-reports.md`.
- Codex does not attempt to fix unrelated failures unless they block progress or are explicitly added to the sprint.
- Sprint notes clearly communicate any unrelated failures to the user and maintainers.

## Notes

Documenting unrelated failures helps maintain transparency about the project's current health without over-scoping sprints.
