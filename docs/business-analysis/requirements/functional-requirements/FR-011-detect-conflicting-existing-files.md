# FR-011: Detect conflicting existing files

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-011 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

When installing ForgePilot into an existing repository, the system shall detect any files that would be overwritten or conflict with existing content before making changes.

## Details

During bootstrap or file creation:

- Codex should check whether the target file or directory already exists in the repository.
- For each potential conflict, Codex should not automatically overwrite the file.
- Conflicts include both file name collisions and directory structure collisions.
- Codex should list all conflicting paths and their types (file/directory) for the user to review.

This requirement prevents accidental loss of work when integrating ForgePilot into projects with existing content.

## Acceptance Criteria

- Before creating or modifying files, Codex checks for the existence of those files or directories.
- If a conflict is detected, Codex does not proceed to overwrite the file.
- Conflicts are recorded and presented to the user with recommended resolution options.

## Notes

This requirement is complemented by FR-012 (prevent automatic overwrites), FR-013 (recommend conflict resolutions), and FR-014 (require conflict approval).
