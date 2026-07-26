# Career Goals Template

Use with the [Career Goal Workflow](../workflows/CAREER_GOAL_WORKFLOW.md). Recommendations generated here do not change career direction until the professional records a decision.

## Record metadata

| Field | Entry |
|---|---|
| Goal record ID | `[GOAL-ID]` |
| Version | `[MAJOR.MINOR]` |
| Planning horizon | `[Start date to review date]` |
| Profile version | `[PROFILE-ID and version]` |
| Market evidence date | `[YYYY-MM-DD]` |
| Owner | `[Human owner]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded / Not applicable]` |
| Approved by and date | `[Human approver; YYYY-MM-DD]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must also record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states defined in [Source Governance](../SOURCE_GOVERNANCE.md).

## Goal statement

| Component | Content | Information type and governed states | Evidence or decision record |
|---|---|---|---|
| Target role family | `[Role family]` | `[STATE]` | `[ID]` |
| Target environment | `[Sector, organization type, or work context]` | `[STATE]` | `[ID]` |
| Geography or work model | `[General boundary]` | `[STATE]` | `[ID]` |
| Time horizon | `[Date or bounded period]` | `[STATE]` | `[ID]` |
| Purpose | `[Why this goal matters]` | `[STATE]` | `[ID]` |

Proposed goal wording:

> `[One concise, measurable but non-inflated statement.]`

Wording document state: `[Draft / Unapproved / Approved exact version]`
Goal decision state: `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]`

## Constraints and preferences

| Item | Type | Priority | Governed states | Decision source | Review date |
|---|---|---|---|---|---|
| `[Constraint or preference]` | `[Non-negotiable / Strong / Flexible]` | `[High / Medium / Low]` | `[STATE]` | `[DECISION-ID]` | `[YYYY-MM-DD]` |

## Target-role hypotheses

| Option | Profile fit evidence | Material gaps | Market evidence | Assumptions | Recommendation |
|---|---|---|---|---|---|
| `[Option]` | `[SOURCE-IDs]` | `[Gap list]` | `[SOURCE-IDs and date]` | `[ASSUMPTION items]` | `[RECOMMENDATION]` |

## Transferable skills and gaps

| Capability | Current evidence | Required evidence | Gap type | Next validation action | Governed states |
|---|---|---|---|---|---|
| `[Capability]` | `[SOURCE-ID]` | `[What the target requires]` | `[Knowledge / Practice / Credential / Evidence]` | `[Action]` | `[STATE]` |

## Milestones

| Milestone | Evidence of completion | Target date | Dependencies | Owner | Status |
|---|---|---|---|---|---|
| `[Milestone]` | `[Observable result]` | `[YYYY-MM-DD]` | `[Dependency]` | `[Owner]` | `[Not started / Active / Complete / Blocked]` |

## Measures and guardrails

| Measure | Definition | Baseline | Target or direction | Data limitation |
|---|---|---|---|---|
| `[Measure]` | `[Stable definition]` | `[FACT or Unknown]` | `[DECISION]` | `[Missing or biased evidence]` |

## Decision log

| Date | Decision | Options considered | Reason | Decision state | Next review |
|---|---|---|---|---|---|
| `[YYYY-MM-DD]` | `[Decision]` | `[Options]` | `[Reason]` | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` | `[YYYY-MM-DD]` |

## Approval checklist

- [ ] Goal is feasible against verified profile evidence.
- [ ] Constraints and preferences are distinguished.
- [ ] Market assumptions are dated and labeled.
- [ ] Gaps are not disguised as existing skills.
- [ ] The professional approved the exact goal and review date.
