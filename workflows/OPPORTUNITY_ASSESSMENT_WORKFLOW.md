# Opportunity Assessment Workflow

## Purpose

Evaluate a verified opportunity against the professional profile, goals, constraints, evidence strength, and application cost, producing a transparent recommendation rather than an automatic decision.

## Inputs

- Verified job-opportunity record
- Approved professional profile and career goal
- [Opportunity assessment template](../templates/OPPORTUNITY_ASSESSMENT_TEMPLATE.md)
- Current skills-gap analysis
- Any user-confirmed constraints

## Participating agents

- **Opportunity Assessment Agent:** performs criterion-by-criterion comparison.
- **Professional Profile Agent:** validates candidate evidence.
- **Evidence Checking Agent:** checks posting claims and traceability.
- **Career Strategy Agent:** interprets trade-offs.
- **Quality Review Agent:** challenges unsupported conclusions.
- **Orchestrator Agent:** routes the final recommendation to human review.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every assessment must separately record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states in [Source Governance](../SOURCE_GOVERNANCE.md). Pursuit disposition may be `Approved within stated scope`; the assessment artifact may be `Approved exact version`. Neither authorizes an application.

## Procedure

1. Confirm that the posting is current and the source record is complete enough to assess.
2. Separate essential requirements, preferred requirements, responsibilities, and practical constraints.
3. Map each requirement to `SUPPORTED`, `PARTIAL`, `GAP`, or `UNKNOWN`, citing the relevant profile evidence.
4. Assess role alignment, transferable skills, material gaps, eligibility, work model, location, language, timing, and application effort.
5. Identify possible disqualifiers and questions that require external clarification.
6. Score fit only after narrative evidence is recorded; never let a single aggregate score hide a critical gap.
7. Record confidence and data quality.
8. Produce a recommendation with reasons, risks, and the smallest useful next action.
9. Run contradiction, missing-context, factual-grounding, and bias checks under the [Evaluation Framework](../EVALUATION_FRAMEWORK.md).
10. Present the assessment for human disposition.

## Human approval gate

The professional chooses `APPLY`, `HOLD`, `INVESTIGATE`, or `DECLINE`. Approval to assess is not approval to tailor materials, contact an employer, or submit an application.

## Outputs

- Traceable fit matrix
- Gaps and clarification questions
- Confidence and evidence-quality statement
- Recommendation
- Human-approved disposition and next action

## Stop and escalation conditions

Stop when the posting is stale, a critical fact cannot be verified, requirements conflict across sources, eligibility is legally ambiguous, or an assessment would require sensitive data not needed at this stage. Escalate hard trade-offs and high-impact assumptions.

## Related controls

See [Source Governance](../SOURCE_GOVERNANCE.md), [Human in the Loop](../HUMAN_IN_THE_LOOP.md), and the next-step [CV Tailoring Workflow](CV_TAILORING_WORKFLOW.md).
