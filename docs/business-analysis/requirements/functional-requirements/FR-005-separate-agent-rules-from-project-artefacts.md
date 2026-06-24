# FR-005: Separate agent rules from project artefacts

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

ForgePilot shall keep Codex operating rules separate from project artefacts. Operating rules belong in `AGENTS.md` and the `.agents/skills/` directory, while product briefs, solution designs, sprints, and other project knowledge belong in the `docs/` directory.

## Details

Separation of concerns helps maintain clarity and avoid conflating how Codex operates with what the project is about. To achieve this:

- Store high-level operating instructions in `AGENTS.md`.
- Store detailed workflows in `.agents/skills/`.
- Store product and delivery artefacts (briefs, requirements, personas, user stories, designs, sprints, ADRs) in `docs/`.
- Do not place transient project state or design details in `AGENTS.md` or skills.

This separation ensures that updating project requirements doesn’t alter core operating rules and vice versa.

## Acceptance Criteria

- `AGENTS.md` and `.agents/skills/` contain only operating instructions and workflows.
- `docs/` contains product discovery, solution design, delivery, decisions, personas, and user stories.
- There is no project-specific information in `AGENTS.md` or skills.
- Operating instructions and project knowledge can be maintained independently.

## Notes

This requirement underpins maintainability and reusability, enabling the same template to be applied across projects without mixing instructions and content.
