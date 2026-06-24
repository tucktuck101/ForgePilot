# FR-006: Detect repository state

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-006 |
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

ForgePilot shall guide Codex to detect the state of the repository before performing any changes. Codex needs to understand whether the repo is empty, new, partially built, or mature.

## Details

Upon repository intake, Codex should perform an inspection to determine:

- If the repo contains no files (empty).
- If the repo only contains the ForgePilot template (new).
- If the repo has partial implementation (partially built).
- If the repo already contains a functioning project with its own tests, CI/CD, documentation, and scripts (mature).

This detection informs how ForgePilot adapts its actions, such as creating structure, respecting existing conventions, and avoiding destructive operations.

## Acceptance Criteria

- Codex examines the directory tree and identifies whether the repository is empty, new, partially built, or mature.
- The detected state is recorded in `docs/project-memory.md` or other intake artefacts.
- Subsequent actions (e.g., file creation, script adaptation) align with the detected state.

## Notes

Accurate detection ensures that ForgePilot does not overwrite existing work and that it appropriately bootstraps an empty or new repository.
