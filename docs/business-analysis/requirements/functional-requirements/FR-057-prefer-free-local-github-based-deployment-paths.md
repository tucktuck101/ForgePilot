# FR-057: Prefer free/local/GitHub-based deployment paths

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-057 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-007](../../discovery/stakeholder-needs/SN-007-secrets-and-security-safety.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall prefer free, local, Docker-based, and GitHub-native deployment options before paid managed services.

## Details

When selecting deployment strategies for prototypes, Codex should prioritise options that incur no or minimal cost and provide ease of use. This includes local environments, Docker containers, GitHub Actions workflows, GitHub Pages for static sites, or other free-tier services. Managed platforms or paid services should only be considered after approval.

## Acceptance Criteria

- Deployment recommendations prioritise cost-free and open-source solutions.
- Codex suggests local or GitHub-based deployment as the default approach when appropriate.
- Proposals to use paid or managed services are clearly identified and require human approval.
- Deployment instructions align with the selected cost-efficient option.

## Notes

Preferring free and local deployment options helps manage costs and reduce reliance on external vendors during prototyping.
