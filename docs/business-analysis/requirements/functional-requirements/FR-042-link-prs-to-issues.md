# FR-042: Link pull requests to issues

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-042 |
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

Each pull request (PR) created by ForgePilot should be linked to the GitHub issue that describes the sprint. This ensures traceability between tasks and code changes.

## Details

- The PR description should include a reference to the issue using the `#<issue_number>` syntax, which automatically links the PR to the issue.
- The issue should also be updated with a link to the PR.
- Linking ensures that closing the PR can automatically close the issue if desired.

## Acceptance Criteria

- Every PR references its corresponding issue number in the description.
- Issues are updated with a link to the PR.
- Stakeholders can navigate between issues and PRs easily.

## Notes

This requirement supports transparency and helps maintain a clear chain of ownership from requirements to implementation.
