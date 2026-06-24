# FR-044: Keep pull requests draft until ready

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | ../../index.md |
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
