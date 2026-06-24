# FR-044: Keep pull requests draft until ready

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-044 |
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

ForgePilot shall keep pull requests in draft state until the sprint’s Definition of Done is satisfied. Only after tests pass and required documentation is updated should the PR be marked ready for review.

## Details

- Draft PRs allow Codex to push commits and update the PR description without notifying reviewers prematurely.
- When the sprint is complete (tests pass, acceptance criteria met, documentation updated), Codex marks the PR ready for review.
- Reviewers are then invited to review and provide feedback or approval.

## Acceptance Criteria

- PRs remain draft until all tasks and tests for the sprint are complete.
- Codex does not request reviews or approvals prematurely.
- The transition from draft to ready is documented and visible.

## Notes

This ensures that reviewers are only engaged when there is a complete, coherent set of changes to review, preventing review fatigue and confusion.
