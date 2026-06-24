# DISC-005: BA Pre-Solution Quality Gate Assessment

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-005 |
| Document type | BA Quality Assessment |
| Status | Passed; human approvals remain pending |
| Priority | Must |
| Owner/audience | Product Owner, Approval Authority, Codex, future maintainers |
| Source | Quality-gate rubric supplied on 2026-06-24 and repository evidence linked below |
| Source need(s) | [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md), [SN-006](stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [Discovery Index](index.md), [Requirements Index](../requirements/index.md), [User Stories Index](../user-stories/index.md) |
| Related objects | [Product Brief](product-brief.md), [Prototype Scope](scope.md), [Approval Gates](approval-gates/index.md) |
| Update rule | Re-run this assessment when pre-solution content, scope, traceability, or approval rules change materially |

## Review Basis

- Structural compliance was checked against the expected artefact pattern and live collection indexes.
- Content quality was assessed from populated project artefacts; `template.md` files were not counted as project truth.
- Traceability quality was checked through live metadata, the traceability matrix, scope trace, and link validation.
- Approval readiness was assessed independently from approval status. A complete pending gate can be ready even though it does not authorise dependent work.
- `docs/product/`, `docs/solution-design/`, `docs/delivery/`, `docs/decisions/`, `AGENTS.md`, and `.agents/skills/` do not yet exist. They are later-stage prototype outputs, not missing pre-solution truth; their dependent work remains blocked.

## BA Quality Gate Attempt 1

### Gate Decision

- Decision: **FAIL**
- Overall score: **21/33**
- Required categories at score 3: Problem framing only
- Categories below threshold: Scope discipline, Workflow and experience understanding, Backlog handoff readiness
- Can implementation proceed: **No**

### Artefacts Reviewed

| Artefact | Type | Live / Example / Template / Missing / Incomplete | Notes |
|---|---|---|---|
| `discovery/problem-statement.md` | Problem framing | Live | Clear problem, symptoms, causes, impact, outcome, owner/audience, and evidence limits |
| `discovery/current-state.md` | Current state | Live | Useful current flow and constraints; no complete target workflow or exception model |
| `discovery/product-brief.md` | Product brief | Live | Correctly pending approval; links the core discovery collections |
| `discovery/target-users/` and `personas/` | Users/personas | Live | Six project-specific roles; no consolidated accountability or conflict map |
| `discovery/value-hypotheses/` and `success-criteria/` | Value/outcomes | Live | Observable measures exist; major capabilities were not consolidated to recipients, value types, and learning goals |
| `discovery/risks/`, `assumptions/`, `open-questions/` | Unknowns | Live | Owners/actions are present; empirical evidence and baseline gaps remain explicit |
| `discovery/options/` | Options | Live | Manual, repository template, CLI, and hosted alternatives with rationale and risks |
| `discovery/scope-items/` | Scope | Incomplete | In/out/deferred items exist, but no bounded consolidated prototype, dependency model, or requirement inclusion boundary |
| `requirements/` | Requirements | Incomplete | Priorities, need links, evidence, and FR/BR acceptance criteria exist; 18 NFRs lacked explicit verification |
| `user-stories/` | User stories | Live | Prioritised actor goals with acceptance criteria and source needs |
| `discovery/traceability-matrix.md` | Traceability | Incomplete | Need-level coverage exists; prototype scope and backlog handoff trace were absent |
| `discovery/approval-gates/` | Approval process | Incomplete | Three pre-solution gates exist; later material gate triggers were not operationalised in one policy |
| `.github/ISSUE_TEMPLATE/` | Backlog handoff | Missing | FR-029 described an issue structure, but no executable process template existed |
| Collection `template.md` files | Authoring templates | Template | Correctly excluded from live project truth |
| `docs/solution-design/`, `docs/delivery/`, `docs/decisions/` | Later-stage artefacts | Missing | Intentionally not required before GATE-002/GATE-003; no implementation artefacts were introduced |

### Scorecard

| Category | Score | Gate status | Evidence | Gap | Required action |
|---|---:|---|---|---|---|
| Problem framing | 3 | Meets required score | `problem-statement.md`; `current-state.md` | None material | None |
| Stakeholder and user understanding | 2 | Meets minimum | Target-user and persona collections | Authority existed across files but no consolidated accountability/trade-off view | Add stakeholder map |
| Value and success definition | 2 | Below required score | Value hypotheses and success criteria collections | Capability-to-recipient/value/learning mapping not consolidated | Add value and success definition |
| Assumptions, risks, and open questions | 2 | Meets minimum | Risk, assumption, open-question, and evidence indexes | Category coverage and empirical evidence remain limited | Keep explicit; no invention |
| Solution neutrality and ideation quality | 3 | Meets | Four options and pending GATE-001 | None material | None |
| Requirement quality | 2 | Below required score | BR/FR/NFR and story collections | NFR verification incomplete; prototype inclusion not distinguished from product priority | Add verification and scope baseline |
| Scope discipline | 1 | Below minimum and required score | Atomic scope-item index | Scope was broad and lacked dependencies, constraints, bounded slices, and requirement boundary | Add consolidated pending prototype scope |
| Workflow and experience understanding | 1 | Below minimum | Current-state workflow and stories | No target flow, handoff table, exception paths, or maintainer operation flow | Add workflow analysis |
| Traceability and evidence | 2 | Meets minimum | Need-level traceability matrix | No explicit scope-to-story/requirement trace or gated delivery handoff rule | Extend traceability matrix |
| Approval gate readiness | 2 | Below required score | GATE-001–003 and NFR-018 | Later mandatory gates lacked operational trigger/record rules | Add operating policy |
| Backlog handoff readiness | 1 | Below minimum | FR-029 and US-022 | Requirement described fields but no process template existed | Add gated issue template |

### Gate Blockers

| Blocker | Category | Evidence | Why it blocks progress | Required fix |
|---|---|---|---|---|
| Major capabilities were not explicitly tied to value recipients, value types, and prototype learning | Value and success | Value-hypothesis and success-criteria indexes | Required category could not score 3 | Consolidated value model |
| NFRs were not all objectively verifiable | Requirement quality | 18 NFR files without local acceptance sections | Required category could not score 3 | Verification matrix and quality rules |
| Candidate prototype boundary was not approval-ready | Scope discipline | Scope-item index only | Required category was below minimum | Consolidated bounded scope |
| Target workflow and exceptions were absent | Workflow understanding | Current-state document | Category was below minimum | Current/target workflow and failure paths |
| Later human gates were not fully operationalised | Approval readiness | GATE-001–003 only | Required category could not score 3 | Gate register and recording policy |
| Delivery handoff was specification-only | Backlog handoff | FR-029; absent issue-template directory | Category was below minimum | Gated delivery issue template |

### Minimum Remediation Set

| ID | Priority | Category | Action | File/path | Required for PASS? |
|---|---|---|---|---|---|
| REM-01 | Must | Stakeholders | Consolidate roles, authority, accountability, and trade-offs | `discovery/stakeholder-map.md` | Yes |
| REM-02 | Must | Value | Map major capabilities to recipient, value type, success, and learning | `discovery/value-and-success-criteria.md` | Yes |
| REM-03 | Must | Scope | Define bounded slices, exclusions, dependencies, constraints, and acceptance boundary | `discovery/scope.md` | Yes |
| REM-04 | Must | Workflow | Add current/target stages, handoffs, exceptions, and maintainer flow | `discovery/workflows.md` | Yes |
| REM-05 | Must | Approval | Operationalise every required human gate and durable outcome | `discovery/approval-gates/operating-policy.md` | Yes |
| REM-06 | Must | Requirements/traceability | Add NFR verification, distinguish product priority from prototype inclusion, and trace scope | `requirements/quality-and-verification-baseline.md`; `discovery/traceability-matrix.md` | Yes |
| REM-07 | Must | Backlog handoff | Add a non-executable-until-approved issue template with all required fields | `.github/ISSUE_TEMPLATE/delivery-work.md` | Yes |

## Rectification Summary for Attempt 1

### Files Changed

| File | Change summary | Rubric category improved |
|---|---|---|
| `discovery/stakeholder-map.md` | Added roles, authority, RACI-style accountability, trade-offs, and evidence limit | Stakeholder understanding |
| `discovery/value-and-success-criteria.md` | Added capability-to-value and prototype-learning model | Value and success |
| `discovery/scope.md` | Added bounded pending scope, requirement slices, exclusions, dependencies, constraints, and acceptance boundary | Scope discipline |
| `discovery/workflows.md` | Added current/target workflows, handoffs, failures, and maintainer operation | Workflow understanding |
| `discovery/approval-gates/operating-policy.md` | Added all mandatory gate triggers, approve/revise/reject outcomes, records, and re-approval | Approval readiness |
| `requirements/quality-and-verification-baseline.md` | Added quality rules and observable verification for all 20 NFRs | Requirement quality |
| `.github/ISSUE_TEMPLATE/delivery-work.md` | Added goal, links, criteria, dependencies, risk, gates, tests, and DoD | Backlog handoff |
| `discovery/traceability-matrix.md` | Added prototype-scope trace and decision/delivery trace rules | Traceability |
| `discovery/product-brief.md` | Linked stakeholder, value, workflow, scope, and approval-policy artefacts | Value, scope, approval |
| `discovery/current-state.md` | Linked the full workflow analysis | Workflow |
| `discovery/index.md` | Indexed all new live singleton documents and approval policy | Structural compliance |
| `discovery/approval-gates/index.md` | Linked and explained the runtime gate policy | Approval readiness |
| `discovery/approval-gates/GATE-001-options-and-direction-approval.md` | Added value and operating-policy context | Approval readiness |
| `discovery/approval-gates/GATE-002-product-brief-approval.md` | Expanded approval inputs to the complete discovery package | Approval readiness |
| `discovery/approval-gates/GATE-003-prototype-scope-approval.md` | Pointed approval at the consolidated scope boundary | Scope and approval |
| `requirements/index.md` | Linked the requirement quality and verification baseline | Requirement quality |
| `business-analysis/index.md` | Clarified live gate report and template separation | Structural compliance |
| `discovery/ba-quality-assessment.md` | Replaced the prior rubric with this supplied-rubric review loop | Gate evidence |

### What Was Fixed

| Gap | Fix | Evidence |
|---|---|---|
| No consolidated stakeholder authority | Added explicit role and accountability map | `stakeholder-map.md` lines 18–47 |
| Value model not capability-complete | Added recipient, value type, success, and learning mapping | `value-and-success-criteria.md` lines 18–42 |
| Prototype scope too broad/implicit | Added five bounded slices and explicit exclusions/dependencies | `scope.md` lines 18–60 |
| Target workflow absent | Added target stages, handoffs, exception paths, and maintainer flow | `workflows.md` lines 29–58 |
| Mandatory later gates incomplete | Added complete gate register and durable recording rules | `approval-gates/operating-policy.md` lines 17–59 |
| NFR verification incomplete | Added one observable verification for every NFR | `requirements/quality-and-verification-baseline.md` lines 18–55 |
| Scope trace incomplete | Added scope-to-needs/users/stories/requirements/success trace | `traceability-matrix.md` lines 33–48 |
| Issue handoff absent | Added gated issue template with all rubric fields | `.github/ISSUE_TEMPLATE/delivery-work.md` lines 11–57 |

### What Remains

| Remaining gap | Reason not fixed yet | Next action |
|---|---|---|
| External user evidence is absent | Evidence cannot be invented | Identify pilot audience and record research/pilot evidence |
| Measurement baselines are absent | No completed comparable pilots exist | Record at least three comparable pilot cycles before improvement claims |
| Product direction, product brief, and scope are unapproved | Human approval was not provided in repository evidence | Approval Authority reviews GATE-001, GATE-002, and GATE-003 |
| Runtime approval record implementation is undecided | This is a later solution-design choice | Resolve OQ-003 after GATE-002 |

## BA Quality Gate Attempt 2

### Gate Decision

- Decision: **PASS**
- Overall score: **32/33**
- Required categories at score 3: Problem framing; Value and success definition; Requirement quality; Scope discipline; Approval gate readiness
- Categories below threshold: None
- Can implementation proceed: **No** — the BA gate passes, but GATE-002 and GATE-003 remain pending

### Artefacts Reviewed

| Artefact | Type | Live / Example / Template / Missing / Incomplete | Notes |
|---|---|---|---|
| Problem statement and current state | Problem/current state | Live | Approval-ready framing with explicit evidence limits |
| Stakeholder map, target users, personas, needs | Stakeholders/users | Live | Authority, roles, needs, and trade-offs are explicit |
| Product brief, value model, hypotheses, success criteria | Value/product | Live | Product brief remains pending; measures distinguish structural proof from value validation |
| Scope document and atomic scope items | Scope | Live | Consolidated boundary is pending approval and explicitly blocks implementation |
| Workflow analysis and stories | Experience/workflow | Live | Current, target, handoff, exception, resume, and maintainer paths are covered |
| Options, assumptions, risks, open questions, evidence | Discovery reasoning | Live | Facts, assumptions, recommendations, and unknowns remain distinct |
| Requirements and quality/verification baseline | Requirements | Live | Prioritised, traceable, accepted/verified, and separated from prototype inclusion |
| Traceability matrix | Traceability | Live | Need coverage, scope trace, decision rules, and gated delivery handoff are explicit |
| Approval gates and operating policy | Approval process | Live | Pre-solution gates are pending; all later mandatory triggers are operationalised |
| Delivery issue template | Backlog handoff | Template/process artefact | Complete handoff structure; explicitly non-executable before approvals |
| Collection `template.md` files | Authoring templates | Template | Clearly separate and not counted as live truth |
| Later-stage design/delivery/decision artefacts | Later-stage artefacts | Missing | Intentionally deferred; absence does not break a pre-solution trace path |

### Scorecard

| Category | Score | Gate status | Evidence | Gap | Required action |
|---|---:|---|---|---|---|
| Problem framing | 3 | Pass | `problem-statement.md` lines 18–49; `current-state.md` lines 18–47 | None material | None |
| Stakeholder and user understanding | 3 | Pass | `stakeholder-map.md` lines 18–51; target-user/persona indexes | External validation absent but roles and authority are approval-ready | Validate during pilots |
| Value and success definition | 3 | Pass | `value-and-success-criteria.md` lines 18–42; value/success indexes | Hypotheses remain unvalidated by design | Collect evidence after approval |
| Assumptions, risks, and open questions | 2 | Pass minimum | Risk, assumption, question, and evidence indexes | Business/data/privacy/cost evidence is still limited before a concrete pilot | Reassess for each pilot/design |
| Solution neutrality and ideation quality | 3 | Pass | Options index; GATE-001; `scope.md` exclusions | Direction remains provisional | Human GATE-001 decision |
| Requirement quality | 3 | Pass | BR/FR/story acceptance criteria; `quality-and-verification-baseline.md` lines 18–55 | None blocking | Maintain baseline on change |
| Scope discipline | 3 | Pass | `scope.md` lines 18–60 | Human approval pending, correctly marked | GATE-003 decision |
| Workflow and experience understanding | 3 | Pass | `workflows.md` lines 18–58 | Pilot validation pending | Test with representative users |
| Traceability and evidence | 3 | Pass | `traceability-matrix.md` lines 18–51; zero broken links | Delivery links are prospective because execution is blocked | Populate only after approvals |
| Approval gate readiness | 3 | Pass | `operating-policy.md` lines 17–59; GATE-001–003 | Approval decisions not yet granted | Human review |
| Backlog handoff readiness | 3 | Pass | `.github/ISSUE_TEMPLATE/delivery-work.md` lines 11–57; FR-029 | No live implementation issue, intentionally | Create from approved scope only |

### Gate Blockers

| Blocker | Category | Evidence | Why it blocks progress | Required fix |
|---|---|---|---|---|
| None for the BA quality gate | — | All categories meet their thresholds | The pre-solution package is ready for the next approved stage | — |

### Minimum Remediation Set

| ID | Priority | Category | Action | File/path | Required for PASS? |
|---|---|---|---|---|---|
| None | — | — | Stop the loop; do not add implementation work | — | — |

## Final BA Pre-Solution Quality Gate Result

### Final Decision

- **PASS**
- Attempts completed: **2**
- Whether implementation may proceed: **No**
- Reason: The pre-solution artefacts meet the supplied quality thresholds, but product-brief and prototype-scope approvals remain Pending and explicitly block solution design/implementation as recorded by GATE-002 and GATE-003.

### Final Scorecard

| Category | Final score | Required score | Status | Evidence |
|---|---:|---:|---|---|
| Problem framing | 3 | 3 | Pass | `problem-statement.md`; `current-state.md` |
| Stakeholder and user understanding | 3 | 2 | Pass | `stakeholder-map.md`; target users; personas |
| Value and success definition | 3 | 3 | Pass | `value-and-success-criteria.md`; value hypotheses; success criteria |
| Assumptions, risks, and open questions | 2 | 2 | Pass | Risks, assumptions, open questions, evidence gaps |
| Solution neutrality and ideation quality | 3 | 2 | Pass | Options, GATE-001, pending decisions |
| Requirement quality | 3 | 3 | Pass | Requirement objects and `quality-and-verification-baseline.md` |
| Scope discipline | 3 | 3 | Pass | `scope.md`; scope items; GATE-003 |
| Workflow and experience understanding | 3 | 2 | Pass | `workflows.md`; stories; personas |
| Traceability and evidence | 3 | 2 | Pass | `traceability-matrix.md`; validated relative links |
| Approval gate readiness | 3 | 3 | Pass | GATE-001–003 and `operating-policy.md` |
| Backlog handoff readiness | 3 | 2 | Pass | Gated delivery issue template and FR-029 |

### Final Artefact Status

| Artefact | Status | Notes |
|---|---|---|
| Problem statement/current state | Draft; gate-ready | Evidence limits are explicit |
| Stakeholder map/users/personas/needs | Draft; gate-ready | Authority and trade-offs are explicit |
| Product brief | Pending approval | Must not be marked final without GATE-002 |
| Value/success/hypotheses | Draft or Unvalidated | Suitable to test; not claimed as proven |
| Prototype scope | Pending approval | Consolidated, bounded, and traceable |
| Workflows | Draft; gate-ready | Includes current, target, exceptions, operations, and resume |
| Options | Pending direction approval | Recommendation remains provisional |
| Risks/assumptions/open questions/evidence | Live | Unknowns and validation actions remain visible |
| Requirements/stories | Draft; gate-ready | Prioritised, accepted/verified, and traceable |
| Traceability matrix | Draft; gate-ready | No broken relative links; delivery path is gated |
| Approval process | Pending decisions; operationally ready | All required triggers and outcomes are defined |
| Delivery issue template | Ready for approved handoff | Not authority to start work |
| Solution design/delivery/decision records | Not started | Correctly deferred until approval |

### Files Changed

| File | Summary |
|---|---|
| `docs/business-analysis/discovery/stakeholder-map.md` | Added stakeholder authority and accountability |
| `docs/business-analysis/discovery/value-and-success-criteria.md` | Added consolidated value/success model |
| `docs/business-analysis/discovery/scope.md` | Added bounded pending prototype scope |
| `docs/business-analysis/discovery/workflows.md` | Added workflow and exception analysis |
| `docs/business-analysis/discovery/approval-gates/operating-policy.md` | Added complete human-gate policy |
| `docs/business-analysis/requirements/quality-and-verification-baseline.md` | Added requirement quality and NFR verification |
| `.github/ISSUE_TEMPLATE/delivery-work.md` | Added gated backlog handoff template |
| `docs/business-analysis/discovery/traceability-matrix.md` | Added scope and delivery trace |
| `docs/business-analysis/discovery/product-brief.md` | Linked new approval inputs |
| `docs/business-analysis/discovery/current-state.md` | Linked detailed workflow analysis |
| `docs/business-analysis/discovery/index.md` | Indexed new live artefacts |
| `docs/business-analysis/discovery/approval-gates/index.md` | Indexed runtime gate policy |
| `docs/business-analysis/discovery/approval-gates/GATE-001-options-and-direction-approval.md` | Expanded direction-decision context |
| `docs/business-analysis/discovery/approval-gates/GATE-002-product-brief-approval.md` | Expanded brief approval condition |
| `docs/business-analysis/discovery/approval-gates/GATE-003-prototype-scope-approval.md` | Pointed to consolidated scope |
| `docs/business-analysis/requirements/index.md` | Linked quality baseline |
| `docs/business-analysis/index.md` | Clarified navigation and template separation |
| `docs/business-analysis/discovery/ba-quality-assessment.md` | Recorded both attempts, rectification, and final result |

### Remaining Risks or Open Questions

| Item | Type | Impact | Required human decision |
|---|---|---|---|
| No external user research | Evidence risk | Personas and value remain plausible but unvalidated | Select representative participants and acceptable evidence |
| No measurement baseline | Measurement risk | Efficiency improvement cannot be claimed | Approve pilot measurement approach |
| Minimum supported stack set | OQ-002 | Pilot fixtures and portability claim remain open | Choose bounded representative stacks at GATE-003 |
| Runtime approval record | OQ-003 | Later workflow state design remains open | Choose durable record mechanism during approved solution design |
| Mandatory automated factory checks | OQ-004 | Validation implementation boundary remains open | Confirm required automated checks at GATE-003 |
| First pilot audience | OQ-005 | Value hypotheses cannot be tested representatively | Identify pilot participants |

### Approval Status

| Approval gate | Status | Evidence | Next action |
|---|---|---|---|
| Options and direction | Pending | GATE-001 has no approver/date/reference | Approval Authority reviews options and records approve/revise/reject |
| Product brief | Pending | GATE-002 has no approver/date/reference | Review the complete discovery package and BA result |
| Prototype scope | Pending | GATE-003 has no approver/date/reference | Review DISC-008 boundaries and unresolved scope decisions |
| Material UX/product flow | Not triggered | Operating policy | Trigger before making or implementing a material flow choice |
| Significant architecture/stack | Not triggered | Operating policy | Trigger during solution design if material |
| External services/credentials/resources | Not triggered | Operating policy | Trigger before selection, access, or configuration |
| Conflict/destructive/deployment/merge | Not triggered | Operating policy | Trigger before the affected action |
| Final prototype acceptance | Not triggered | Operating policy | Trigger after verified handoff |

### Do Not Do Yet

- Finalise the product brief or prototype scope without recorded human approval.
- Start solution design while GATE-002 is Pending.
- Create executable implementation work or implement product functionality while GATE-002 or GATE-003 is Pending.
- Make material UX, architecture, stack, external-service, credential, conflict, or destructive decisions without their gate.
- Use real credentials or production resources.
- Deploy externally, merge pull requests, or accept a final prototype.

### Final Verdict

**BA quality gate passed. Pre-solution artefacts are ready for the next approved stage.**
