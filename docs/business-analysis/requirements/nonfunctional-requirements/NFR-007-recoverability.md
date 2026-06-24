# NFR-007: Recoverability

## Document Metadata

| Field | Value |
|---|---|
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

The system must support recovery across Codex sessions.

## Details

ForgePilot should persist enough project state across sessions to allow Codex to resume work without re-reading the entire repository. It should maintain a concise `docs/project-memory.md`, `docs/delivery/current-sprint.md`, and `docs/delivery/resume-brief.md` as continuity files. When token limits are reached, the system must pause safely, update these files, and provide clear next instructions. The next run should continue from these files without losing context.

## Notes

Recoverability is critical for long-running tasks that exceed a single session or context window.
