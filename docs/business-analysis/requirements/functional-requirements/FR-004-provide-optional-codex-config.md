# FR-004: Provide optional Codex configuration

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

ForgePilot should support an optional project-specific Codex configuration file stored under the `.codex/` directory. This configuration may override default behaviors or provide project-level settings when needed.

## Details

While ForgePilot aims to work out-of-the-box for most projects, certain repositories may require custom settings for Codex. To facilitate this, the template should include:

- A `.codex/` directory at the repository root.
- A `config.toml` or similar configuration file that Codex can read to adjust its behaviour.

This configuration should be optional. When absent, Codex falls back to default settings and the guidance defined in `AGENTS.md` and skills.

## Acceptance Criteria

- The template contains a `.codex/` directory.
- The directory includes a sample or optional `config.toml` file that can be customised per project.
- Codex reads and applies settings from `config.toml` if present.
- Absence of this file does not break default behaviour.

## Notes

This requirement allows advanced users to fine-tune Codex without modifying the core template or instructions. It should be used sparingly and documented in the template’s README.
