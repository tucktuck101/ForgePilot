# FR-027: Keep Markdown as the knowledge source

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | ../../index.md |
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
