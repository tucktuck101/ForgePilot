# US-013: Approve Credential Use

## Document Metadata

| Field | Value |
|---|---|
| Document type | User Story |
| Status | Draft |
| Owner/audience | Client, Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [User Stories Index](index.md) |
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
