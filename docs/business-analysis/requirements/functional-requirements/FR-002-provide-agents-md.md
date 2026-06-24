# FR-002: Provide `AGENTS.md`

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

ForgePilot shall include an `AGENTS.md` file containing concise, durable repository-level instructions for Codex. This file provides high-level guidance for how Codex should operate within the repository.

## Details

The `AGENTS.md` file serves as the canonical place for durable, project-wide operating instructions. It should:

- Explain at a high level how Codex should behave in the repository.
- Point to relevant skills and documentation in the `.agents/skills/` and `docs/` directories.
- Avoid storing transient project state or long instructions that belong in reusable skills or project documentation.
- Remain concise and be updated only when the operating model or approval-gate policy changes.

This requirement supports the broader goal of separating stable operating rules from changing project knowledge.

## Acceptance Criteria

- A file named `AGENTS.md` exists at the repository root.
- It contains clear, concise instructions for Codex on how to operate within the repo.
- It links to relevant skills and documents without duplicating their content.
- It does not include temporary project state or lengthy guidelines better suited for skills or documentation.

## Notes

This requirement works alongside FR-003 (provide reusable skills) and FR-005 (separate agent rules from project artefacts) to ensure that operating instructions are easy to find and maintain.
