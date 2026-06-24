# FR-007: Detect existing tooling

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | ../../index.md |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall guide Codex to detect existing languages, frameworks, package managers, scripts, tests, documentation, continuous integration, and deployment files in the repository.

## Details

During repository intake, Codex should identify:

- Programming languages and frameworks used (e.g., Node/TypeScript, Python, Go).
- Package managers (npm, yarn, pip, go modules, etc.).
- Existing scripts such as build, test, lint, and format scripts.
- Existing testing frameworks and test files.
- Existing documentation structure and conventions.
- Continuous integration configurations (e.g., GitHub Actions workflows) and deployment files.

Recognising these assets ensures ForgePilot respects and integrates with the current setup rather than duplicating or replacing it unnecessarily.

## Acceptance Criteria

- Codex scans the repository for key files and directories that indicate existing tooling.
- Identified tools and configurations are recorded in intake notes or project memory.
- Actions like script creation or modification account for the presence of existing tools.

## Notes

This requirement works with FR-010 (adapt to existing conventions) to ensure that ForgePilot acts cooperatively rather than disruptively.
