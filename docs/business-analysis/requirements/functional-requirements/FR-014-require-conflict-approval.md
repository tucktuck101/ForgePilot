# FR-014: Require conflict approval

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

ForgePilot shall require human approval before applying any conflict resolution that alters existing files. This ensures user oversight when the template integration could modify pre-existing content.

## Details

After listing conflicts and providing recommended options (see FR-013), Codex must:

- Wait for the user to select a resolution option.
- Apply the chosen option only after receiving explicit approval.
- Record the decision in project notes and update `docs/project-memory.md` as needed.

This gate protects existing work from unintended changes and aligns with the overall approval policy.

## Acceptance Criteria

- No conflicting files are modified or replaced without user approval.
- User approval is explicitly captured for each conflict resolution.
- The chosen resolution is recorded in project notes.

## Notes

This requirement is consistent with the principle that only human decisions should determine project direction, risk management, and destructive actions.
