# US-011: Approve Risky Architecture or Tech Stack Decisions

## Document Metadata

| Field | Value |
|---|---|
| Object ID | US-011 |
| Document type | User Story |
| Status | Draft |
| Priority | Must |
| Owner/audience | Client, Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-002](../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [User Stories Index](index.md) |
| Related objects | [User Stories Index](index.md), [SN-002](../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Update rule | Update when this user story changes materially |

## Summary

Capture the Client need to approve risky architecture or tech-stack decisions.

## Story

As the Client, I want Codex to stop for architecture or stack decisions when meaningful trade-offs exist so that I can control cost, complexity, security, and maintainability.

## Acceptance Criteria

- Codex explains the recommendation and alternatives.
- Trade-offs are documented.
- An ADR is created where appropriate.
- Codex waits for approval when required.

## Notes

None.
