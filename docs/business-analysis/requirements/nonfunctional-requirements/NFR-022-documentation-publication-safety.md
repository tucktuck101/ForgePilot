# NFR-022: Documentation Publication Safety

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-022 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Approval Authority, Codex, maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [RSK-007](../../discovery/risks/RSK-007-documentation-publication-information-exposure.md), [FR-056](../functional-requirements/FR-056-require-pre-deployment-approval.md), [SC-011](../../discovery/success-criteria/SC-011-documentation-publication-readiness.md) |
| Update rule | Update when publication audiences, information classifications, or approval controls change materially |

## Summary

Any future documentation publication shall prevent unintended exposure of restricted information.

## Details

Static documentation publication is a documentation-publication activity rather than prototype or application deployment. Its primary risk is information exposure. Before publication, the intended content and audience must be reviewed for sensitive, private, client-confidential, credential-bearing, production-only, or otherwise restricted information. Explicit approval is required whenever publication would expose, or may reasonably expose, such information.

## Acceptance Criteria

- A later publication design defines the intended audience and publishable content boundary.
- Restricted information is excluded from generated and published output.
- Publication that may expose restricted information remains blocked until explicit approval is recorded.
- Publication safety checks cover generated output as well as source Markdown.
- No publication workflow or external exposure is authorised by this requirement alone.
