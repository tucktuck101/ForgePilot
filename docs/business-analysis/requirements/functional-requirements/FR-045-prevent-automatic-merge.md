# FR-045: Prevent automatic merge

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-045 |
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

ForgePilot shall not merge pull requests without explicit human approval. Merging is a high-impact action that requires sign-off from the user or designated reviewer.

## Details

- Even if tests pass and all requirements are met, Codex should wait for a human to approve the PR before merging.
- The merge method (e.g., merge, squash, rebase) should follow repository conventions or user preference.
- This rule applies to all branches, including the default branch (e.g., `main`).

## Acceptance Criteria

- PRs are not merged automatically by Codex.
- Codex flags when a PR is ready for merge and requests approval.
- Only after approval does the merge occur (typically executed by the user or with explicit instruction).

## Notes

This requirement aligns with the general policy of requiring human approval for high-impact actions and ensures repository integrity.
