# ForgePilot

ForgePilot is a proposed reusable GitHub repository template for running software prototype delivery with Codex. Its goal is to take a vague idea through structured discovery, human-approved scope, design, implementation, validation, and final handoff without requiring the user to micromanage routine work.

The operating model combines agent autonomy with explicit human control. Codex should be able to perform routine analysis and delivery work independently, while material decisions—such as product direction, architecture, credentials, destructive changes, deployment, and merge—remain approval-gated.

## Intended capabilities

- Bootstrap ForgePilot into new or existing repositories without silently overwriting project files.
- Conduct chat-driven product discovery and record the results as version-controlled Markdown.
- Link evidence, stakeholder needs, requirements, scope, decisions, GitHub issues, and delivery outcomes.
- Convert approved scope into bounded delivery work, with verification and one draft pull request per sprint by default.
- Preserve compact project state so work can resume safely across Codex sessions and context limits.
- Prefer portable, free, open-source, local, and GitHub-native tooling for core operation.

The primary users are solo builders and product owners who want help moving quickly from an idea to a tested prototype. The model also accounts for client approval authorities, Codex delivery agents, repository bootstrappers, technical reviewers, and future maintainers.

## Current status

As of June 25, 2026, ForgePilot still does not contain an installable or runnable implementation; it remains a repository skeleton. The business-analysis foundation (problem, users, workflows, options, requirements, risks, proposed scope, traceability, and approval process) has been documented and the pre‑solution quality assessment has passed.

The Product Owner has now approved the three pre‑solution gates recorded in this repository:

1. **Product direction** — GATE‑001 approved the recommended reusable GitHub template approach.
2. **Product brief** — GATE‑002 approved the consolidated product intent and operating model.
3. **Prototype scope** — GATE‑003 approved the bounded capability slices for the first implementation.

With these approvals, solution design may begin. Implementation, backlog execution, and prototype construction may proceed once sufficient solution design is recorded, but remain subject to later gates governing architecture, material UX/product flows, external services, credentials, deployment, destructive actions, merge, and final acceptance. The product assumptions and value hypotheses also remain unvalidated. The initial pilot audience, measurement approach, proposed stack fixtures, runtime approval‑recording model, and proposed automated‑check boundary were answered on June 25, 2026, but measurement and pilot evidence are not yet available.

## Proposed first prototype

The current candidate scope is intended to test five areas:

1. A safe, durable repository operating skeleton.
2. Chat-led, approval-ready pre-solution discovery.
3. Controlled handoff from approved scope to design and GitHub issues.
4. Repeatable validation of structure, metadata, links, traceability, and secret safety.
5. Reliable session resumption and final prototype handoff.

A hosted orchestration platform, mandatory paid services, production guarantees, automatic merging, production credentials, and broad compatibility claims are explicitly outside the proposed first prototype.

## Documentation

Start with the [Business Analysis Index](docs/business-analysis/index.md). It links to the current discovery package, personas, user stories, and requirements.

The most useful project-level documents are:

- [Product brief](docs/business-analysis/discovery/product-brief.md)
- [Problem statement](docs/business-analysis/discovery/problem-statement.md)
- [Current state](docs/business-analysis/discovery/current-state.md)
- [Proposed prototype scope](docs/business-analysis/discovery/scope.md)
- [Current and target workflows](docs/business-analysis/discovery/workflows.md)
- [Approval gates](docs/business-analysis/discovery/approval-gates/index.md)
- [Pre-solution quality assessment](docs/business-analysis/discovery/ba-quality-assessment.md)
