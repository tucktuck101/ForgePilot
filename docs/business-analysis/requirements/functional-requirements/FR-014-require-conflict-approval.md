# FR-014: Require conflict approval

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-014 |
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
