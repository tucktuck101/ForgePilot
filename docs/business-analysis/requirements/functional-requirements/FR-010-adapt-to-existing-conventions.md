# FR-010: Adapt to existing conventions

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-010 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall guide Codex to adapt to existing repository conventions rather than imposing new ones. When a project already has its own scripts, tests, documentation structure, or CI/CD configurations, Codex should integrate with them.

## Details

- If the repository already contains scripts for setup, validation, testing, linting, or formatting, Codex should use or wrap those scripts instead of creating duplicates.
- If the repository uses a particular documentation structure (e.g., `docs/guide` vs. `docs/reference`), Codex should place new documents in appropriate places.
- If CI/CD workflows are present, Codex should amend or extend them rather than replacing them wholesale.
- When adding new files, Codex must check for existing file names and directories to avoid conflicts.
- Integration should be done cautiously to respect existing project maintainers’ decisions.

## Acceptance Criteria

- Existing scripts and workflows are leveraged rather than duplicated.
- New files or directories introduced by ForgePilot do not conflict with existing ones.
- Codex records how it adapted to existing conventions in project notes.

## Notes

This requirement ensures that ForgePilot can be used on mature projects without disrupting the established workflow.
