# FR-073: Mark Examples Clearly

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Update rule | Update when this requirement changes materially |

## Summary

Example artefacts must be clearly marked to prevent them from being treated as live project content.

## Details

ForgePilot includes example completed artefacts alongside templates. To avoid confusion, each example file must include clear labels—both in the filename and within the document itself—that identify it as an example. AGENTS.md and relevant skills should instruct Codex to ignore example files when generating or updating project artefacts. Index files should not list example documents as part of the active project documentation.

## Acceptance Criteria

- Example files have names or folder locations that indicate they are examples.
- Each example document includes a notice near the top stating that it is an example and not part of the live project.
- Index files for business analysis artefacts do not include example documents.
- Skills or agent instructions explicitly warn Codex to avoid treating example content as project truth.

## Notes

This requirement complements FR-072 and ensures clarity between sample and live artefacts.
