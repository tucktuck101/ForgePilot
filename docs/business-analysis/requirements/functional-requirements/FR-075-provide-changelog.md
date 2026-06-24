# FR-075: Provide Changelog

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-075 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Could |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Related objects | [Functional Requirements Index](index.md), [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The template must include a `CHANGELOG.md` file documenting version changes.

## Details

To help users understand what has changed between versions of ForgePilot, a `CHANGELOG.md` file should be maintained at the repository root. Each entry in the changelog should correspond to a version in the `VERSION` file and summarise the changes introduced in that version. The changelog should follow established conventions (e.g., `### Added`, `### Changed`, `### Removed`, etc.) and highlight breaking changes when present.

## Acceptance Criteria

- A `CHANGELOG.md` file exists at the repository root.
- Each version bump in `VERSION` corresponds to a new entry in the changelog.
- Entries summarise added, changed, deprecated, removed, fixed, and security changes where applicable.

## Notes

Maintaining a changelog increases transparency for maintainers and users.
