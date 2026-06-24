# FR-031: Use one sprint per pull request by default

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-031 |
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

ForgePilot shall structure delivery so that each scoped sprint corresponds to a single GitHub pull request (PR) by default. This improves traceability and simplifies review.

## Details

- When a sprint is planned, Codex should create a new branch and a draft PR to implement that sprint’s work.
- The PR title should reflect the sprint goal or issue title.
- Once the sprint is complete and all checks pass, the PR can be reviewed and merged (with approval).
- If the sprint grows or requires splitting, additional issues and PRs may be created, but one-PR-per-sprint is the standard.

## Acceptance Criteria

- Each sprint results in one draft PR opened at the start of the sprint.
- The PR links to the corresponding issue.
- Work is confined to the PR and branch until the sprint’s Definition of Done is met.
- PR merges only after approval.

## Notes

Keeping PRs aligned to sprints helps maintain clear boundaries between tasks, facilitates code review, and allows for easier rollback if necessary.
