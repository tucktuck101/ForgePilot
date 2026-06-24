# FR-060: Require credential approval

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-060 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall require human approval before using real credentials, API keys, OAuth clients, tokens, cloud accounts, or production resources.

## Details

Codex must not request or use real credentials until the user has explicitly approved their use for specific actions. Until approval is granted, placeholder values in `.env.example` must be used. Any creation or modification of cloud resources or secrets must also be approved. Approval requests should clearly list the service involved, the credential names, and the reason for use.

## Acceptance Criteria

- Codex uses only placeholder values until explicit approval is granted for credential use.
- Codex requests approval before using real credentials for API calls, database connections, or deployment operations.
- Approval requests list the services, secret identifiers, and reasons for using the credentials.
- Codex does not proceed with actions requiring real credentials until approval is recorded.

## Notes

This requirement helps protect sensitive credentials and prevents unauthorised resource usage.
