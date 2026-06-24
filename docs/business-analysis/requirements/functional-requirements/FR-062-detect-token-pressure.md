# FR-062: Detect token pressure

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

The system shall detect when token/context pressure is likely to affect safe continuation.

## Details

Codex should monitor its context window usage and anticipate when the remaining tokens or context size may be insufficient to continue work. When token pressure is detected, Codex should prepare to pause and create a resume brief. Detection may involve estimating the size of current memory, pending tasks, and typical per-task token usage.

## Acceptance Criteria

- Codex detects approaching context or token limits based on the system’s context window size.
- Codex stops initiating new tasks when token pressure is detected.
- Codex triggers the context recovery workflow to safely pause work.

## Notes

Detecting token pressure early helps avoid abrupt terminations and ensures continuity across Codex sessions.
