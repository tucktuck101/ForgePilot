# ForgePilot — Detailed Project Brief

## Document Metadata

| Field | Value |
|---|---|
| Document type | Project brief |
| Product name | ForgePilot |
| Status | Draft |
| Primary audience | User / Product Owner, Codex, future maintainers |
| Purpose | Define the product intent, operating model, delivery process, safety boundaries, and expected artefacts for ForgePilot |
| Inputs | Discovery interview, requirements extraction, persona/user-story analysis |
| Outputs | Requirements, personas, user stories, solution design, implementation backlog |
| Update rule | Update when product direction, delivery model, approval gates, repo structure, or operating assumptions change |

## 1. Project Summary

ForgePilot is a reusable GitHub repository template that enables Codex to autonomously design, build, test, document, and prepare deployment for software prototypes. The template can be applied to new or existing repositories. Once installed, Codex reads the repository guidance, interviews the user about their idea, produces discovery artefacts, designs an appropriate solution, implements scoped sprints, manages GitHub Issues and pull requests, runs validations, and stops only when human approval is required. The goal is to delegate the heavy lifting of prototyping to Codex while preserving control over product direction, risk, cost, secrets, destructive actions, deployment, and acceptance.

## 2. Product Goal

Build a reusable Codex-oriented GitHub template repository that allows a user to move from a vague idea to a working prototype with minimal manual intervention while ensuring safe autonomy, clear approval gates, token efficiency, and maintainability.

## 3. Primary Deliverable

ForgePilot shall be delivered as a GitHub template repository. The template includes `AGENTS.md`, `.codex`, `.agents`, `docs`, `templates`, `examples`, `scripts`, `.github`, `README.md`, `CHANGELOG.md`, and `VERSION`.

## 4. Supported Use Cases

ForgePilot supports web apps, mobile apps, desktop apps, APIs, backend services, CLI tools, workflow automations, AI agents, data tools, integrations, internal tools, and scripts/utilities.

## 5. Operating Environment

The template is environment-agnostic. It avoids assumptions about OS, language, package manager, or deployment platform. It supports local development, Codespaces/devcontainers, GitHub, and CI-based validation. Codex interacts via chat.

## 6. Core Principles

- **Single Adaptive Delivery Process:** Use one adaptive process from repo intake to acceptance review, with depth determined by ambiguity and risk.
- **Agile, Task-Scoped:** Sprints are scoped by tasks, not time. Each sprint corresponds to a GitHub Issue and PR.
- **GitHub Issues as Delivery Backlog:** Issues track executable work; Markdown docs store knowledge.
- **One PR per Sprint:** Each sprint produces one draft pull request.
- **Autonomy with Guardrails:** Codex acts autonomously except at approval gates.
- **Human Approval When Necessary:** Only require approval at meaningful gates.
- **Token Efficiency:** Plan for context limits by summarising state in `project-memory.md`, `current-sprint.md`, and `resume-brief.md`.

## 7. Repository Structure

The repository separates agent operating rules from project artefacts:

```
AGENTS.md
.codex/
.agents/
docs/
templates/
examples/
scripts/
.github/
README.md
CHANGELOG.md
VERSION
```

Agent rules live in `AGENTS.md` and `.agents/skills`. Product, solution, delivery, and decision artefacts live in `docs/`. Templates and examples live in their respective folders. Scripts provide validation and tooling.

## 8. Documentation Style

Use a polished doc-object style. Each major document includes document type, status, audience, purpose, inputs, outputs, linked artefacts, and update rule. Avoid mixing agent rules with project artefacts.

## 9. Examples and Templates

Provide blank templates and example completed artefacts in `templates` and `examples`. Mark examples clearly to avoid confusion with live project files.

## 10. Stack Detection

The template detects common stacks (Node/TypeScript, Python, Go, Docker, static sites, GitHub Actions) and adapts scripts accordingly. Unknown stacks default to conservative assumptions with human approval when needed.

## 11. Toolchain Philosophy

Prefer free, open-source, local, and GitHub-native tools. Use simple, maintainable technology. Document significant deviations.

## 12. Factory Validation

Include validation scripts and CI to check that the template itself is complete, examples are marked, docs use doc-object metadata, and no secrets are committed.

## 13. Approval Gates

Require approval for:
1. Product brief and scope.
2. Material UX/product flows.
3. Significant architecture/stack choices.
4. External or paid services.
5. Credential use.
6. Resolving conflicts in existing repos.
7. Destructive/high-risk actions.
8. Deployment.
9. Pull request merges.
10. Final acceptance.

## 14. Existing Repo Conflict Behaviour

Do not overwrite conflicting files automatically. Detect conflicts, provide recommendations, and request approval before resolution.

## 15. Secrets and Credentials

Never invent, expose, or commit secrets. Use `.env.example` with placeholders. Prefer mock/local services. Document required secrets in `docs/solution-design/secrets-and-config.md`.

## 16. Context and Token-Limit Recovery

Treat token limits as a planned continuity mechanism. When context is low, stop starting new work, summarise state in `project-memory.md`, update `current-sprint.md` and `resume-brief.md`, commit safe work, and provide clear resume instructions.

## 17. Versioning and Changelog

Treat the template as a product. Include a `VERSION` file and `CHANGELOG.md` for tracking changes to structure, skills, scripts, docs, examples, workflows, and policies.

## 18. Final Handoff Package

When a prototype is complete, produce `docs/delivery/final-handoff.md` with the working prototype status, setup/run instructions, test instructions and results, deployment instructions, product brief, scope, architecture summary, key ADRs, known limitations, security/privacy notes, future backlog, and acceptance checklist.

## 19. Definition of Success

ForgePilot succeeds when a user can install the template, run Codex to perform discovery, approve the brief and scope, have Codex design and build in scoped sprints with GitHub Issues and draft PRs, resume safely after context limits, approve deployment and merges, and receive a final handoff package for review or continuation.
