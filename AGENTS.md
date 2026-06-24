# ForgePilot Agent Instructions

## Start here

- Read [README.md](README.md) for the human-facing project summary.
- Use the [Business Analysis Index](docs/business-analysis/index.md) as the entry point for project knowledge.
- Before proposing design, backlog execution, or implementation, check the live approval state in the [Discovery Index](docs/business-analysis/discovery/index.md) and [Approval Gates](docs/business-analysis/discovery/approval-gates/index.md).
- Load only the documents directly relevant to the task; follow their links when more context is required.

## Repository boundaries

- Treat `docs/` as the source of truth for product discovery, requirements, decisions, and delivery artefacts.
- Treat collection `template.md` files as authoring aids, not as live project facts.
- Keep durable repository-wide Codex rules in this file. Put detailed reusable workflows in `.agents/skills/` when that directory exists.
- Do not start work that a documented approval gate blocks. Never infer approval from silence, prior work, or an ambiguous request.
- Do not use real credentials, production resources, paid or external services, destructive operations, deployments, or merges without the explicit approval required by the [Approval Gate Operating Policy](docs/business-analysis/discovery/approval-gates/operating-policy.md).

## Working practices

- Inspect the repository and relevant documentation before editing.
- Preserve existing user changes and avoid modifying unrelated files.
- Prefer small, traceable changes that follow existing naming, metadata, and Markdown conventions.
- When adding or changing a discovery object, requirement, story, or decision, update its relevant index and traceability links.
- Keep facts, assumptions, recommendations, open questions, and approval decisions distinct.
- Never commit secrets or place secret values in documentation, examples, logs, or tests.
- If existing files conflict with a proposed change, preserve them and present the options and consequences before replacing or deleting content.

## Verification

This repository is currently documentation-led and has no configured build or test command. For every change:

1. Run `git diff --check`.
2. Verify changed relative Markdown links resolve.
3. Confirm affected collection indexes and traceability records remain accurate.
4. Review the final diff for unintended scope, stale status claims, secrets, and approval-gate violations.

## Completion

A task is complete only when the requested change is made, relevant documentation remains internally consistent, applicable checks pass, and the final response states what changed and what was verified.
