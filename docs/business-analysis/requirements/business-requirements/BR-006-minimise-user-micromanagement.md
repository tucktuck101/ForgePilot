# BR-006: Minimise user micromanagement

## Document Metadata

| Field | Value |
|---|---|
| Object ID | BR-006 |
| Document type | Business Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall allow Codex to autonomously perform routine implementation, testing, documentation, issue management, and pull request workflows without requiring constant user intervention.

## Details

To avoid micromanagement, the system should empower Codex to handle routine tasks such as creating issues, branches, commits, tests, linting, formatting, documentation updates, and draft pull requests. Codex should follow established guidelines and scripts without needing to ask the user for approval for each routine action. Only decisions that affect product direction, risk, or exposure should require approval.

## Acceptance Criteria

- Codex creates and updates GitHub Issues for scoped work autonomously.
- Codex opens branches, makes commits, and opens draft PRs during sprints without human prompts.
- Codex updates documentation and runs validations as needed.
- The user is not asked to approve routine low-risk changes.

## Notes

This requirement reduces friction and keeps the user focused on high-level decisions rather than day-to-day implementation details.
