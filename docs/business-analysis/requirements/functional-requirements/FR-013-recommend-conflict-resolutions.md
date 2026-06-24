# FR-013: Recommend conflict resolutions

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

Upon detecting a file or directory conflict, ForgePilot shall provide the user with recommended resolution options instead of defaulting to an overwrite.

## Details

When conflicts are identified, Codex should suggest options such as:

- Keep the existing file and skip creating the template file.
- Merge relevant content manually into the existing file.
- Create a new file with a different name (e.g., append `.forgepilot` or a similar suffix).
- Back up the existing file (e.g., rename with `.bak`) before replacing it.

Codex should present these options with a brief explanation of the implications of each choice. This empowers the user to make an informed decision on how to integrate the template.

## Acceptance Criteria

- For each conflict, Codex proposes at least two resolution options.
- Proposed options include keeping, merging, renaming, or backing up existing files.
- The user is prompted to choose before any action is taken.

## Notes

The recommended options should be context-aware; for example, if the conflicting file is critical for an existing workflow, emphasise safer options like keeping or backing up rather than replacing it.
