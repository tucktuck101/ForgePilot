# FR-053: Fix failures caused by current work

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-053 |
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

The system shall fix test failures and quality issues caused by changes introduced in the current sprint before marking the sprint complete.

## Details

During a scoped sprint, ForgePilot may encounter failing tests or quality checks. When such failures are introduced by the changes of the current sprint, Codex must diagnose the cause and implement fixes as part of the sprint work. Codex should re-run the relevant checks to confirm that the fixes have resolved the issues.

## Acceptance Criteria

- The system identifies test failures and quality issues introduced by the current sprint.
- Codex fixes the root cause of the failures within the scope of the sprint.
- The relevant tests and checks are re-run to verify that the issues are resolved.
- A sprint is not marked complete until failures caused by the sprint are fixed or explicitly deferred with justification and approval.

## Notes

Fixing regressions introduced by new work is essential to maintain project stability and prevent accumulating technical debt.
