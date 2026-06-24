# FR-009: Handle unknown stacks

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-009 |
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

When ForgePilot cannot identify a common technology stack, Codex should fall back to targeted repository inspection, documented assumptions, conservative recommendations, and human approval for material trade-offs.

## Details

In cases where stack signals are absent or unfamiliar:

- Codex should inspect the repository structure and contents to infer as much context as possible.
- Where inference is uncertain, Codex should document assumptions and seek clarification from the user for critical decisions.
- Proposed tools or scripts should lean toward generic solutions (e.g., basic shell scripts, manual testing) until more information is available.
- For decisions with significant trade-offs (e.g., selecting a database or deployment platform), Codex should request human approval.

This approach ensures progress without imposing unsupported assumptions or risking misalignment with the project’s actual needs.

## Acceptance Criteria

- Unknown stacks do not break ForgePilot operations.
- Codex documents assumptions and clarifies uncertainties rather than guessing inappropriate defaults.
- Human approval is requested when material decisions are required.

## Notes

This requirement complements FR-008 (detect common stack signals) by ensuring the system remains robust when detection fails.
