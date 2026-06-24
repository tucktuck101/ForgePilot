# FR-074: Provide Version File

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-074 |
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

Include a `VERSION` file at the root of the template to track the current version of ForgePilot.

## Details

ForgePilot is a maintained product and must include its own version number. A text file named `VERSION` should reside at the repository root containing a single version string, following semantic versioning (e.g., `v1.0.0`). This version number should increment when the template is updated in meaningful ways. Codex and humans can use this version to determine compatibility and understand changes.

## Acceptance Criteria

- The repository root contains a `VERSION` file with the current version string.
- The version number is updated when significant changes are made to the template.
- The version file is referenced in the changelog (FR-075).

## Notes

Versioning helps track template evolution and supports reproducibility.
