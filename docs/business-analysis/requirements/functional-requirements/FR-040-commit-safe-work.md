# FR-040: Commit safe work autonomously

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-040 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

Codex should commit changes to the branch during sprint execution when it is safe to do so. Commits should be meaningful and atomic, representing logically grouped changes.

## Details

- Codex should avoid committing half-finished work that would break tests or cause a non-functional state.
- Each commit message should describe the changes introduced.
- Commits can be made after implementing a feature slice, adding tests, or updating documentation.
- Frequent commits help track progress and facilitate code review.

## Acceptance Criteria

- Commits occur throughout the sprint to capture incremental progress.
- Commit messages are clear and descriptive.
- Commits maintain or improve the build and test state (i.e., no failing commits).

## Notes

This requirement ensures a clean and understandable commit history for the final PR and reduces the risk of losing work if context limits interrupt the session.
