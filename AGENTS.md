# ForgePilot Agent Instructions

## Purpose

This file defines durable repository-level guidance for agents assisting with the development and maintenance of ForgePilot.

## Boundary

- These instructions govern work on ForgePilot itself.
- Do not treat them as the automatic operating model for projects created from ForgePilot.
- Keep downstream project workflows, generated-template guidance, and examples separate and clearly marked as reusable or illustrative rather than live ForgePilot project truth.

## Start here

- Read [README.md](README.md) for the human-facing project summary.
- Inspect only the repository files relevant to the current task, following links when more context is required.
- Use the [Business Analysis Index](docs/business-analysis/index.md) when work involves business analysis, discovery, requirements, scope, or approval state.
- For work that may be approval-gated, check the live state in the [Discovery Index](docs/business-analysis/discovery/index.md) and [Approval Gates](docs/business-analysis/discovery/approval-gates/index.md).

## ForgePilot development workflow

The canonical ForgePilot workflow is:

**Intake → Discovery → Analysis → Scope → Design → Plan → Develop → Test → Accept → Stabilise → Iterate**

These are adaptive workflow chunks, not rigid waterfall phases. Determine which chunk applies from the current task. Use that chunk to guide the expected artefacts, reasoning style, approval gates, quality checks, and whether work should proceed, pause, or loop back.

### Chunk definitions

- **Intake** — Understand the request and inspect the relevant repository state, conventions, constraints, existing changes, and conflicts. Produce a bounded task understanding; preserve conflicting files until any required resolution is approved.
- **Discovery** — Establish the problem, users, needs, evidence, current workflows, desired outcomes, assumptions, risks, and open questions. Reduce ambiguity without prematurely choosing or implementing a solution.
- **Analysis** — Synthesize discovery inputs into traceable requirements, options, dependencies, trade-offs, and recommendations. Keep evidence and facts distinct from assumptions and proposed decisions.
- **Scope** — Define the approved delivery boundary: outcomes, included and excluded capabilities, deferred work, dependencies, acceptance conditions, and traceability. Do not treat candidate scope as executable until the applicable scope gate is approved.
- **Design** — Translate approved product inputs into UX, technical, data, integration, and operational decisions. Compare credible alternatives, record rationale, and pause for approval before committing to any material gated choice.
- **Plan** — Convert approved scope and sufficient design into ordered, bounded delivery work. Define GitHub Issues, dependencies, acceptance criteria, validation expectations, and the intended issue/branch/draft-PR sequence without executing blocked work.
- **Develop** — Implement the approved work item with small, traceable changes. Stay within the issue boundary, follow repository conventions, update affected documentation, and stop if implementation exposes a material unapproved decision or scope change.
- **Test** — Run the applicable automated and manual checks and record useful evidence. Fix failures caused by the current work when they are within scope; document unrelated failures rather than silently broadening the task.
- **Accept** — Compare the result and evidence against the approved scope and acceptance criteria. Prepare an approval-ready summary of outcomes, limitations, and deviations; only the authorised human may approve merge or final prototype acceptance.
- **Stabilise** — Make an accepted result dependable for handoff or continued use by addressing in-scope defects, documentation gaps, integration issues, and operational rough edges. Re-run affected checks and preserve known limitations and recovery information.
- **Iterate** — Use feedback, validation results, operational learning, or changed needs to choose the appropriate earlier chunk and repeat deliberately. Update durable state and reopen approval gates when a material approved boundary has changed.

## Delivery model

- GitHub Issues are the executable backlog for ForgePilot development.
- By default, each scoped development sprint uses one GitHub Issue, one branch, one draft pull request, one validation pass, and one acceptance decision.
- Keep pull requests in draft until they are ready for review or acceptance.
- Never merge without explicit human approval.

## Repository boundaries

- Treat `docs/` as ForgePilot's durable knowledge base for product discovery, requirements, decisions, and delivery artefacts.
- Keep durable repository-wide agent rules in this file.
- Put reusable execution workflows in `.agents/skills/` when that directory is present.
- Put detailed delivery workflow documentation in `docs/delivery/` when that directory is present.
- Keep examples separate from live project truth and label them clearly.
- Treat collection `template.md` files and generated templates as authoring aids unless they are explicitly promoted to live project truth.

## Working practices

- Inspect relevant repository context before editing.
- Preserve existing user changes and avoid unrelated edits.
- Prefer small, traceable changes that follow existing naming, metadata, and Markdown conventions.
- When changing a discovery object, requirement, story, decision, or other indexed artefact, update the relevant index and traceability links.
- Keep facts, assumptions, recommendations, open questions, and approval decisions distinct.
- Never commit secrets or place real secret values in documentation, examples, logs, or tests.
- Handle routine, low-risk implementation and documentation choices autonomously when they are consistent with repository conventions and are not approval-gated.
- If existing files conflict with a proposed change, preserve them until an explicit conflict-resolution decision is approved.

## Approval gates

Follow the [Approval Gate Operating Policy](docs/business-analysis/discovery/approval-gates/operating-policy.md). Never infer approval from silence, prior work, document creation, or an ambiguous request.

Explicit human approval is required before:

- finalising the product direction or product brief;
- finalising prototype scope;
- implementing material UX or product flows;
- making significant architecture or technology-stack decisions;
- adding external or paid services, APIs, authentication providers, analytics, AI providers, or hosted databases;
- using real credentials, API keys, OAuth clients, tokens, cloud accounts, or production resources;
- replacing or deleting conflicting repository files;
- performing destructive or hard-to-reverse actions;
- externally or publicly deploying the prototype or application;
- publishing documentation when restricted information may be exposed, as defined by the operating policy;
- merging pull requests; or
- accepting the final prototype.

When approval is required, state:

1. what is being approved and why approval is required now;
2. the recommended option and credible alternatives;
3. the material risks and trade-offs;
4. what becomes permitted or remains blocked next; and
5. the **Approve**, **Revise**, and **Reject** paths and where the decision will be recorded.

Do not begin work that a documented gate blocks. A prior approval does not cover a material change to its approved boundary.

## Verification

- Run configured build, test, lint, format, and documentation checks when available.
- If no applicable command exists, state that clearly rather than implying it passed.
- Run `git diff --check` when working locally.
- Verify changed relative Markdown links resolve where practical.
- Confirm affected indexes and traceability records remain accurate.
- Review the final diff for unintended scope, stale status claims, secrets, and approval-gate violations.
- Document unavailable checks and unrelated failures.

## Completion

A task is complete only when:

- the requested change is made;
- relevant documentation remains internally consistent;
- applicable checks pass, or unavailable and unrelated checks are clearly documented;
- applicable approval gates are recorded as satisfied or pending; and
- the final response states what changed and what was verified.
