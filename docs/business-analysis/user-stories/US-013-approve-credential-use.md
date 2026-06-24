# US-013: Approve Credential Use

## Document Metadata

| Field | Value |
|---|---|
| Object ID | US-013 |
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

Capture the Client need to approve use of credentials and secrets.

## Story

As the Client, I want to approve use of real credentials and secrets so that sensitive access is not mishandled.

## Acceptance Criteria

- `.env.example` uses placeholders.
- Required secrets are documented.
- Real secrets are not printed or committed.
- Codex waits for approval before using real credentials.

## Notes

None.
