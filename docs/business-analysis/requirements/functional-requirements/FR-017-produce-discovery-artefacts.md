# FR-017: Produce discovery artefacts

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

ForgePilot shall produce structured discovery artefacts after the interview phase, capturing essential information about the project in Markdown files under `docs/business-analysis/discovery/`.

## Details

Upon completion of discovery questions, Codex should create the following documents:

- `product-brief.md`: summarising the overall goal and purpose.
- `problem-statement.md`: detailing the problem to solve.
- `target-users.md`: describing intended users or personas.
- `prototype-hypothesis.md`: explaining what the prototype is meant to prove.
- `scope.md`: listing what is in scope and out of scope for the prototype.
- `success-criteria.md`: defining what constitutes a successful prototype.
- `risks-assumptions-open-questions.md`: capturing known risks, assumptions, and unresolved questions.
- `user-stories.md`: listing initial user stories or jobs-to-be-done.
- `definition-of-done.md`: stating high-level acceptance criteria for the project.

Each artefact should follow the doc-object style with metadata, summary, details, and update rules.

## Acceptance Criteria

- All specified discovery files are created in the repository under the appropriate folder.
- Documents follow the doc-object format.
- Information captured during discovery is correctly transcribed into these files.
- Files are organised under `docs/business-analysis/discovery/`.

## Notes

These artefacts serve as the foundation for solution design and subsequent phases. Keeping them clear and structured supports both Codex and human stakeholders.
