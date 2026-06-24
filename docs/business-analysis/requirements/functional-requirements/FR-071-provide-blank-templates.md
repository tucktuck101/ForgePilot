# FR-071: Provide Blank Templates

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-071 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Related objects | [Functional Requirements Index](index.md), [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The repository must include blank templates for each type of business analysis artefact.

## Details

ForgePilot should provide Markdown templates that describe the expected structure for each artefact type, including business requirements, functional requirements, nonfunctional requirements, personas, user stories, ADRs, sprints, and final handoff. These template files act as guides for both Codex and human contributors, ensuring consistent documentation. The templates must not contain actual project content; instead, they include placeholders and brief descriptions of what to include.

## Acceptance Criteria

- Each requirements folder contains a `template.md` file with the doc-object structure and placeholder content.
- The personas and user-stories folders include their own `template.md` files.
- Template files clearly indicate that they are templates and should not be treated as live artefacts.

## Notes

Templates help maintain consistency and encourage adherence to the doc-object style used throughout ForgePilot.
