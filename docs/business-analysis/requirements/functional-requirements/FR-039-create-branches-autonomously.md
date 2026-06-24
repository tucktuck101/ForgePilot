# FR-039: Create branches autonomously

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-039 |
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

During sprint execution, Codex may autonomously create branches in the repository to isolate changes and support the one-PR-per-sprint workflow.

## Details

- When a sprint begins, Codex should create a new branch derived from the default (e.g., `main`) or from the most recent commit on the default branch.
- Branch names should include the sprint or issue identifier (e.g., `sprint-001`, `feature/US-003-login-flow`).
- The branch remains open until the sprint’s work is complete and merged via a PR.
- Branch creation should not occur if a conflicting branch already exists; in that case, Codex should notify the user or choose a different name.

## Acceptance Criteria

- New branches are created at the start of each sprint.
- Branch names follow a consistent naming convention.
- Branch creation does not override or conflict with existing branches.
- Branches serve as the basis for draft PRs.

## Notes

Autonomous branch creation streamlines the development process and keeps work isolated until it is ready for integration.
