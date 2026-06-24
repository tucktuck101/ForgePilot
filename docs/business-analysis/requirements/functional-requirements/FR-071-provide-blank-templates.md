# FR-071: Provide Blank Templates

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Functional Requirements Index](../index.md) |
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