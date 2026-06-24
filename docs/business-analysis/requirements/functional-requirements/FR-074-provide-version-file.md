# FR-074: Provide Version File

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

Include a `VERSION` file at the root of the template to track the current version of ForgePilot.

## Details

ForgePilot is a maintained product and must include its own version number. A text file named `VERSION` should reside at the repository root containing a single version string, following semantic versioning (e.g., `v1.0.0`). This version number should increment when the template is updated in meaningful ways. Codex and humans can use this version to determine compatibility and understand changes.

## Acceptance Criteria

- The repository root contains a `VERSION` file with the current version string.
- The version number is updated when significant changes are made to the template.
- The version file is referenced in the changelog (FR-075).

## Notes

Versioning helps track template evolution and supports reproducibility.