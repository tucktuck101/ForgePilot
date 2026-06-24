# BR-013: Treat the template as a maintained product

## Document Metadata

| Field | Value |
|---|---|
| Document type | Business Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index.md](index.md) |
| Update rule | Update when this artefact changes materially |

## Summary

ForgePilot shall treat the template itself as a maintained product with versioning and changelog practices.

## Details

The template is not a one-off deliverable; it evolves over time. ForgePilot must include a `VERSION` file indicating the current template version and a `CHANGELOG.md` that records changes to the structure, skills, scripts, docs, examples, workflows, and policies. Template updates should follow semantic versioning where practical. The changelog should clearly identify breaking changes and recommended migration steps.

## Acceptance Criteria

- A `VERSION` file exists in the template repository.
- A `CHANGELOG.md` exists and is updated whenever the template changes.
- The changelog entries describe changes in a clear and structured way.
- The template version is incremented appropriately.

## Notes

This requirement ensures that users of ForgePilot know when and how the template has changed and can upgrade accordingly.
