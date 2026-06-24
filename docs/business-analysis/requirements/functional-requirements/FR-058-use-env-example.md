# FR-058: Use .env.example

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

The system shall provide a `.env.example` file containing placeholder values for all required environment variables.

## Details

ForgePilot projects should include a `.env.example` file that lists all environment variables needed to run the project locally or in CI. Each variable should have a placeholder value and explanatory comments as needed. The real `.env` file with actual secrets should be excluded via `.gitignore` and never committed to version control. The `.env.example` file serves as documentation for required configuration.

## Acceptance Criteria

- A `.env.example` file exists in the repository.
- `.env.example` lists all required environment variables with placeholder values and, where helpful, comments.
- The real `.env` file is not present in version control and is listed in `.gitignore`.
- Documentation references `.env.example` for setup and deployment instructions.

## Notes

Including a `.env.example` file helps users and Codex understand required configuration without exposing secrets.
