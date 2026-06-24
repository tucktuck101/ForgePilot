# FR-001: Provide required repository structure

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-001 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall include the required directory and file structure as defined in the project brief.

## Details

The template must create a consistent directory structure, including `AGENTS.md`, `.codex/`, `.agents/`, `docs/`, `templates/`, `examples/`, `scripts/`, `.github/`, `README.md`, `CHANGELOG.md`, and `VERSION`. This structure ensures that Codex and users have the necessary context and scaffolding to operate effectively.

## Acceptance Criteria

- The repository includes all required directories and files after applying the template.
- Directories are created even if initially empty.
- The structure matches the specification in the project brief.

## Notes

This requirement sets the foundation for all subsequent functionality.
