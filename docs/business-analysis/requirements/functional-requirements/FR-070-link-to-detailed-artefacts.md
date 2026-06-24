# FR-070: Link to Detailed Artefacts

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

Project memory and other summaries should link to detailed artefacts rather than duplicating their content.

## Details

To maximise token efficiency and avoid duplication, the system must place detailed information in dedicated documents under `docs/` and link to them from summary files such as project memory, sprint notes, and resume briefs. This ensures that long descriptions or decisions are stored in the appropriate artefact (for example, solution design files, ADRs, or sprint notes) while summary documents reference them by relative link. Codex should avoid copying large sections of text into multiple places.

## Acceptance Criteria

- Project memory entries link to relevant discovery, design, delivery, and decision artefacts rather than duplicating their content.
- Sprint notes summarise decisions and reference the full details by link.
- Resume briefs contain links to relevant files instead of repeating their content.

## Notes

This requirement supports token efficiency and maintainability across long-running sessions.