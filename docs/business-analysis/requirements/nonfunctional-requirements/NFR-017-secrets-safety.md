# NFR-017: Secrets Safety

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-017 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot must protect secrets.

## Details

The system must never invent, print, or commit secrets, API keys, tokens, private certificates, or any other sensitive credentials. It should use `.env.example` files with placeholder values and ensure `.env` and other sensitive files are listed in `.gitignore`. Real credentials must only be used after explicit approval from the user. When secrets are required, the system should document them in `docs/solution-design/secrets-and-config.md`, explaining their purpose and how they should be provided securely.

## Notes

This requirement reduces the risk of credential leaks and unauthorised access.
