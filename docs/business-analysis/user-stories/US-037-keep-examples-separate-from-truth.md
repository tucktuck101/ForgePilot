# US-037: Keep Examples Separate from Truth

## Document Metadata

| Field | Value |
|---|---|
| Object ID | US-037 |
| Document type | User Story |
| Status | Draft |
| Priority | Must |
| Owner/audience | ForgePilot Maintainer, Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [User Stories Index](index.md) |
| Related objects | [User Stories Index](index.md), [SN-010](../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Update rule | Update when this user story changes materially |

## Summary

Capture the ForgePilot Maintainer need to distinguish examples from live project artefacts.

## Story

As a ForgePilot Maintainer, I want example artefacts clearly separated from live project artefacts so that Codex does not confuse examples with the project's actual state.

## Acceptance Criteria

- Examples live under `examples/`.
- Examples are clearly marked.
- AGENTS.md and skills warn not to treat examples as project truth.
- Factory validation checks example markings where practical.

## Notes

None.
