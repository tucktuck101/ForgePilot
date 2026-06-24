# FR-049: Validate skills and templates

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-049 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [index](index.md) |
| Related objects | [index](index.md), [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall validate that all skills and templates are present and structurally valid.

## Details

ForgePilot must ensure that each skill in `.agents/skills/` contains a `SKILL.md` with clear instructions, triggers, and outputs, and that each template in `templates/` conforms to the doc-object style with placeholders and no sample project content. The validation should also ensure that examples in `examples/` are correctly separated and marked as examples.

## Acceptance Criteria

- Validation checks that each skill directory exists and contains a `SKILL.md` file.
- Validation verifies that each `SKILL.md` defines trigger conditions, process steps, outputs, stop conditions, and approval gates.
- Validation checks that each template file uses the doc-object style and contains placeholders rather than live project data.
- Validation ensures that example artefacts are clearly marked and stored separately from live project files.

## Notes

Proper validation of skills and templates helps maintain consistency and usability across different ForgePilot projects.
