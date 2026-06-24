# FR-043: Include pull request summaries

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-043 |
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

Pull requests created by ForgePilot shall include a summary section in their description outlining the work done, tests run, risks identified, and any required approvals.

## Details

- At the end of a sprint, before requesting review, Codex should update the PR description with:
  - A brief summary of the work completed.
  - A list of tests run and their results.
  - Notable decisions or trade-offs made during the sprint.
  - Identified risks or blockers.
  - Approval gates that need to be cleared (e.g., deployment approval).
- This summary helps reviewers understand the context and scope of the changes without reading all commits.

## Acceptance Criteria

- PRs have a structured summary section when ready for review.
- The summary covers work done, tests, decisions, risks, and approval gates.
- Reviewers can quickly assess the state of the sprint from the summary.

## Notes

Including thorough summaries in PRs improves transparency, communication, and the quality of code reviews.
