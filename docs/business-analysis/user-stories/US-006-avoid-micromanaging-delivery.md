# US-006: Avoid Micromanaging Delivery

## Document Metadata

| Field | Value |
|---|---|
| Object ID | US-006 |
| Document type | User Story |
| Status | Draft |
| Priority | Must |
| Owner/audience | Solo Builder, Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-002](../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [User Stories Index](index.md) |
| Related objects | [User Stories Index](index.md), [SN-002](../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Update rule | Update when this user story changes materially |

## Summary

Capture the Solo Builder need for Codex to handle routine delivery work autonomously.

## Story

As a Solo Builder, I want Codex to handle routine delivery work autonomously so that I only intervene at approval gates.

## Acceptance Criteria

- Codex autonomously creates issues, branches, commits, docs, and draft PRs where safe.
- Codex stops only for approval gates or serious risk.
- Routine implementation decisions are documented but not escalated unnecessarily.

## Notes

None.
