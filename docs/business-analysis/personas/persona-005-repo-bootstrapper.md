# persona-005: Repo Bootstrapper

## Document Metadata

| Field | Value |
|---|---|
| Document type | Persona |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Personas Index](./index.md) |
| Update rule | Update when this persona changes materially |

## Profile

The Repo Bootstrapper is the person or automated process responsible for installing the ForgePilot template into a new or existing repository. This may be the user manually copying files, Codex applying the template, or a future install script.

## Goals

- Install the template safely without overwriting valuable existing files.
- Detect existing repository structure, scripts, tests, and CI.
- Create missing folders and templates where appropriate.
- Preserve useful existing conventions.
- Leave the repository ready for the first Codex run.

## Pain Points

- Existing repos may already have documentation, scripts, CI, or agent instructions.
- Blindly copying template files can overwrite valuable work or create conflicts.
- Different stacks require different validation scripts and conventions.
- Empty repos need more bootstrapping than mature repos.

## Needs

- A safe bootstrap process that first inspects the repo.
- Conflict detection and recommended resolution options.
- Human approval before resolving conflicts.
- Adaptive stack detection to tailor scripts and tools.
- Clear first-run instructions for the user and Codex.

## Notes

Ensuring a careful install process makes ForgePilot usable on a wide variety of existing projects without damaging them.
