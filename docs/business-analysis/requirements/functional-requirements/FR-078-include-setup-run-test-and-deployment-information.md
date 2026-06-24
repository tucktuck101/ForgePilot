# FR-078: Include Setup, Run, Test, and Deployment Information

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-078 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-009](../../discovery/stakeholder-needs/SN-009-complete-prototype-handoff.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Related objects | [Functional Requirements Index](index.md), [SN-009](../../discovery/stakeholder-needs/SN-009-complete-prototype-handoff.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The final handoff document must include setup, run, test, and deployment instructions.

## Details

A handoff is not complete without clear instructions for using the delivered prototype. The final handoff document must provide:

- Setup instructions (dependencies, environment variables, local setup commands)
- Run instructions (how to start the application locally and any recommended environment settings)
- Test instructions (commands to run tests and interpret results)
- Deployment instructions or the staging URL if deployment has been approved, including required environment variables, secrets, and smoke tests

These sections ensure that future users can evaluate and operate the prototype without guesswork.

## Acceptance Criteria

- The final handoff includes clearly labelled sections for setup, run, test, and deployment instructions or staging URL.
- Required environment variables and secrets are referenced and documented (but not included) appropriately.
- Commands are presented in a format suitable for copy-pasting into a terminal.

## Notes

This requirement ensures that prototypes are usable and deployable by reviewers and future maintainers.
