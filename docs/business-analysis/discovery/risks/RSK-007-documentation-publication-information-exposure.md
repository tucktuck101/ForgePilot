# RSK-007: Documentation publication information exposure

## Document Metadata

| Field | Value |
|---|---|
| Object ID | RSK-007 |
| Document type | Risk |
| Status | Open |
| Priority | Must |
| Owner/audience | Product Owner, Approval Authority, Codex, maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-007](../stakeholder-needs/SN-007-secrets-and-security-safety.md), [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [OPT-006](../options/OPT-006-generated-documentation-portal.md), [FR-056](../../requirements/functional-requirements/FR-056-require-pre-deployment-approval.md), [NFR-022](../../requirements/nonfunctional-requirements/NFR-022-documentation-publication-safety.md) |
| Update rule | Update when the publication audience, content classification, or safety controls change materially |

## Assessment

- Likelihood/impact: Medium likelihood, High impact.
- Owner: Product Owner and Approval Authority.
- Primary exposure: sensitive, private, client-confidential, credential-bearing, production-only, or otherwise restricted information becoming available to an unintended audience.
- Distinction: static documentation publication does not create the same runtime risk as prototype or application deployment, but it can create material information exposure.
- Mitigation: keep repository Markdown authoritative; classify intended publication content; validate links and generated output; require explicit approval whenever publication may expose restricted information; and defer tooling and workflow design to approved solution work.

## Closure Condition

Close only when an approved publication design demonstrates content-boundary controls, review and approval rules, and evidence that restricted information is excluded from the published output.
