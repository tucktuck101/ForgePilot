# US-015: Approve Deployment

## Document Metadata

| Field | Value |
|---|---|
| Object ID | US-015 |
| Document type | User Story |
| Status | Draft |
| Priority | Must |
| Owner/audience | Client, Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-007](../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [User Stories Index](index.md) |
| Related objects | [User Stories Index](index.md), [SN-007](../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Update rule | Update when this user story changes materially |

## Summary

Capture the Client need to approve deployment before external exposure.

## Story

As the Client, I want to approve deployment before anything becomes externally accessible so that I control exposure.

## Acceptance Criteria

- Deployment readiness summary exists.
- Secrets/config requirements are documented.
- Smoke test plan exists where relevant.
- Codex waits for approval before deployment.

## Notes

None.
