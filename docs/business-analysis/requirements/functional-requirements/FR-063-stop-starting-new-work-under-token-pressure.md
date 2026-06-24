# FR-063: Stop starting new work under token pressure

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index](index.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall stop starting new work when token pressure is detected.

## Details

Once token pressure is detected, Codex must not initiate new tasks or steps. It should focus on completing or safely pausing the current atomic task and then enter the context recovery workflow. This ensures that work is not interrupted mid-task when the context window is about to be exhausted.

## Acceptance Criteria

- Codex stops beginning new tasks when token pressure is present.
- Codex finishes or safely pauses the current atomic task.
- Codex proceeds to write a resume brief and update project memory as part of the context recovery workflow.

## Notes

Stopping new work under token pressure helps maintain continuity and prevents partial implementations.
