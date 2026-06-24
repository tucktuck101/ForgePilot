# FR-060: Require credential approval

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index](index.md) |
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
