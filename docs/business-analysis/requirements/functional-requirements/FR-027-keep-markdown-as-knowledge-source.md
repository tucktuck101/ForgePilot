# FR-027: Keep Markdown as the knowledge source

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-027 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall use Markdown documentation as the canonical source of product, design, delivery, and decision knowledge. GitHub Issues are for work tracking, but they should reference the Markdown files for context.

## Details

- Product briefs, requirements, personas, user stories, solution designs, sprints, and ADRs are stored as Markdown files in the `docs/` directory.
- GitHub Issues should link to these documents rather than replicate their content.
- Updates to core information should happen in the Markdown files first, with issues or comments referencing the changes.

## Acceptance Criteria

- All key artefacts exist as Markdown files within `docs/business-analysis`.
- Issues and PRs reference these files via relative links.
- Duplicate or conflicting information in Issues is minimised.

## Notes

This separation ensures clarity between long-lived knowledge and transient work logs, and supports token-efficient operations.
