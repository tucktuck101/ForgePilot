# FR-028: Link issues to documentation

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

GitHub Issues created by ForgePilot shall include links to relevant documentation. This ensures context is easily accessible to anyone reviewing or working on the issue.

## Details

- Each issue should reference the requirement, user story, or design document that defines the work.
- Links should be relative to the repository (e.g., `docs/business-analysis/...`) so they remain valid when cloned or viewed offline.
- If multiple artefacts apply, list them succinctly in the issue description.
- Do not duplicate the content of the documents in the issue body.

## Acceptance Criteria

- Issues contain relative links to the appropriate docs.
- The linked documents provide sufficient context for the task.
- Users and Codex can navigate from the issue to the documentation and back.

## Notes

Linking helps maintain a single source of truth and reduces confusion when tasks span multiple artefacts.
