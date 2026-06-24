# BR-008: Prefer free and open-source tooling

## Document Metadata

| Field | Value |
|---|---|
| Object ID | BR-008 |
| Document type | Business Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index.md](index.md) |
| Related objects | [index.md](index.md), [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall prefer free, open-source, local, and GitHub-native tools unless a paid or external service is explicitly approved.

## Details

The system should prioritise widely accepted free and open-source tools for development, testing, deployment, and project management. When multiple toolchain options exist, Codex should choose the option that avoids costs and vendor lock-in, unless the user has approved a paid or external alternative. Documentation should highlight any use of paid services and require approval before integration.

## Acceptance Criteria

- Default stacks and scripts use free/open-source tools.
- Paid services or managed platforms are only integrated after approval.
- Toolchain choices and deviations are documented.

## Notes

This requirement supports cost-effective prototyping and reduces dependency on proprietary services.
