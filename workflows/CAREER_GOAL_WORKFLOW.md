# Career Goal Workflow

## Purpose

Turn broad career preferences into a bounded, reviewable goal with target roles, constraints, evidence needs, success measures, and decision points.

## Inputs

- Approved professional profile
- [Career goals template](../templates/CAREER_GOALS_TEMPLATE.md)
- Current constraints and preferences
- Skills evidence and a current skills-gap assessment
- Relevant market evidence, with capture dates

## Participating agents

- **Career Strategy Agent:** frames options and trade-offs.
- **Professional Profile Agent:** checks feasibility against verified experience.
- **Job Research Agent:** supplies time-bounded market evidence.
- **Evidence Checking Agent:** distinguishes market facts from inference.
- **Orchestrator Agent:** keeps recommendations separate from decisions.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every record must also carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states defined in [Source Governance](../SOURCE_GOVERNANCE.md). A goal may be `Approved within stated scope`; its exact plan version may be `Approved exact version`. Neither state is external authorization.

## Procedure

1. Define the review horizon and the decision the workflow must support.
2. Record non-negotiable constraints separately from preferences.
3. Generate a small set of plausible target-role hypotheses grounded in the approved profile.
4. Compare each hypothesis across fit, evidence strength, entry barriers, learning needs, location or work-model constraints, and market uncertainty.
5. Identify transferable skills and material gaps without upgrading adjacent experience into direct experience.
6. Formulate one primary goal and, only when useful, one fallback goal.
7. Convert the goal into milestones, evidence-building activities, and review dates.
8. Tag projections and market interpretations as `ASSUMPTION` or `RECOMMENDATION`, then record their governed states separately.
9. Run consistency and feasibility review against the [Career Lifecycle](../CAREER_LIFECYCLE.md).
10. Submit the goal package for human selection and approval.

## Human approval gate

Only the professional may choose or change the target role, geography, work model, timeline, acceptable trade-offs, or learning commitments. Approval is also required before the goal changes downstream CV, LinkedIn, portfolio, or application positioning.

## Outputs

- Approved career-goal statement
- Constraints and preferences register
- Target-role comparison
- Skills-gap and evidence-building plan
- Milestones, review date, and decision log

## Stop and escalation conditions

Stop when a goal depends on an unverified qualification, conflicts with a stated constraint, requires regulated advice, or rests on stale or insufficient market evidence. Escalate material trade-offs to the professional instead of optimizing them silently.

## Related controls

Follow [Source Governance](../SOURCE_GOVERNANCE.md), [Human in the Loop](../HUMAN_IN_THE_LOOP.md), and [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md).
