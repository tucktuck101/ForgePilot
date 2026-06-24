# FR-076: Track Template Evolution

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Functional Requirements Index](../index.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The template must record its evolution across versions and maintainers.

## Details

ForgePilot should preserve the history of changes to its structure, skills, scripts, workflows, and documentation. This evolution is captured through a combination of versioning (FR-074), changelog entries (FR-075), and commit history. Maintainers should update version and changelog entries when introducing changes and ensure that the rationale for significant changes is documented in ADRs or commit messages.

## Acceptance Criteria

- Each update to the template incrementally increases the version and updates the changelog.
- Significant changes to design, delivery process, or file structure are captured in ADRs or commit messages.
- Users can trace when and why major template features were added or altered.

## Notes

Tracking evolution fosters long-term maintainability and helps future maintainers make informed decisions.