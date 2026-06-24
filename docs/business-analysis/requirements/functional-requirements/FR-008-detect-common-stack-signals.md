# FR-008: Detect common stack signals

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

ForgePilot v1 shall identify common signals indicating the technology stack and tools used in the repository. This helps Codex select appropriate scripts, tests, and deployment strategies.

## Details

Signals include but are not limited to:

- `package.json` or `tsconfig.json` for Node/TypeScript projects.
- `pyproject.toml`, `requirements.txt`, or `setup.py` for Python projects.
- `go.mod` for Go projects.
- `Dockerfile`, `docker-compose.yml`, or other container definitions.
- Static site generators or frameworks (e.g., `index.html`, `site.config`, `vite.config`).
- `.github/workflows/` directory for GitHub Actions workflows.
- Common test configuration files (e.g., Jest, pytest, go test files).

Detecting these signals allows the system to choose validation scripts, testing frameworks, and deployment methods that align with the project's existing tech stack.

## Acceptance Criteria

- Codex scans the repository for known files and patterns associated with common stacks.
- Detected stack signals are recorded in intake artefacts.
- The system selects or adapts scripts and validation processes based on the detected stack.

## Notes

Unknown stacks should fall back to targeted inspection and conservative assumptions as described in FR-009 (handle unknown stacks).
