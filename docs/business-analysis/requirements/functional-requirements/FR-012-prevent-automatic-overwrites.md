# FR-012: Prevent automatic overwrites

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-012 |
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

ForgePilot shall ensure that Codex does not automatically overwrite existing files when a conflict is detected. Instead, it should stop and report the conflict.

## Details

When a file creation or update would overwrite an existing file:

- Codex should not perform the overwrite without explicit user confirmation.
- Codex should log the conflict details, including the path, file type, and why a conflict occurred.
- Codex should suggest that the user review the conflict and choose an appropriate resolution.

This behaviour prevents unintended loss of existing content when the template is applied to mature repositories.

## Acceptance Criteria

- No existing file is overwritten automatically by Codex.
- Conflicts are reported rather than acted upon without user input.
- The system waits for human approval or direction before resolving a conflict.

## Notes

This requirement reinforces the safety principle and works together with FR-011, FR-013, and FR-014 to handle conflicts responsibly.
