# BR-002: Support new and existing repositories

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

ForgePilot shall support both new empty repositories and existing repositories that already contain code, documentation, scripts, tests, or continuous integration.

## Details

The system must detect whether the target repository is empty, newly created, partially built, or mature. It should adapt its installation accordingly and avoid overwriting existing content without explicit approval. For existing repositories, ForgePilot should integrate with existing structures, tooling, and conventions rather than imposing a single layout. Any potential conflicts must be reported and resolved with human approval.

## Acceptance Criteria

- The template can initialise an empty repository with the required structure and files.
- When applied to an existing repository, ForgePilot inspects the current contents and identifies existing languages, frameworks, scripts, tests, and CI configurations.
- Existing files are not overwritten automatically; conflicts are detected and presented for approval.
- The installation process respects existing conventions and integrates the template non-destructively.

## Notes

Supporting both new and existing repositories broadens the usefulness of ForgePilot and ensures it can be adopted by projects at any stage.
