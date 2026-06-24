# FR-050: Validate doc-object metadata

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index](index.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall validate that major documentation files include the required doc-object metadata fields.

## Details

For each document in `docs/`—including briefs, requirements, indexes, templates, personas, and user stories—the validation should check for a **Document Metadata** section that contains required fields such as **Document type**, **Status**, **Owner/audience**, **Source**, **Linked artefacts**, and **Update rule**. Missing or incomplete metadata should cause validation to fail with an explanatory message.

## Acceptance Criteria

- Validation scans documentation files for a `Document Metadata` section.
- The metadata section contains all required fields with non-empty values.
- Validation fails when any required metadata field is missing or empty.
- Validation output clearly identifies which document is missing metadata and which field is missing.

## Notes

This requirement ensures that all ForgePilot documentation remains self-describing and easy to maintain.
