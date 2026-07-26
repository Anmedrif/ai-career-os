# Offer Evaluation Workflow

## Purpose

Support a structured comparison of an employment offer against the professional's goals, constraints, evidence, risks, and questions while preserving human judgment and the boundary around legal or financial advice.

## Inputs

- Written offer or user-confirmed offer terms
- Approved career goal and constraints
- Verified opportunity assessment
- User-defined evaluation criteria and priorities
- Public or authorized contextual evidence

## Participating agents

- **Career Strategy Agent:** structures criteria and trade-offs.
- **Opportunity Assessment Agent:** compares the offer with the assessed role.
- **Evidence Checking Agent:** separates written terms from verbal or inferred terms.
- **Privacy Review Agent:** limits exposure of compensation and personal information.
- **Orchestrator Agent:** records questions and routes the decision to the professional.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every offer record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). A choice may be `Approved within stated scope`; exact response wording may be `Approved exact version`; communication requires `Externally authorized`.

## Procedure

1. Define the decision deadline and ensure the evaluation uses the current offer version.
2. Extract terms into categories: role, duties, reporting, location, work model, start date, compensation, benefits, probation, notice, contingencies, and restrictions.
3. Mark absent or verbal terms as unresolved; do not convert them into facts.
4. Compare the offer with career goals, minimum constraints, and the original opportunity.
5. Identify material changes, ambiguities, downside risks, and clarification questions.
6. Apply user-defined weights only after recording narrative evidence.
7. Develop bounded options: accept, clarify, negotiate, decline, or seek qualified advice.
8. Run completeness, consistency, privacy, and missing-context review.
9. Prepare a neutral decision brief and any draft questions.
10. Submit all decisions and communications to the professional.

## Human approval gate

Only the professional may disclose terms, contact the employer, negotiate, accept, decline, or sign. Any legal, tax, immigration, or regulated-financial issue requires qualified professional advice.

## Outputs

- Term and evidence matrix
- Goal-and-constraint comparison
- Risk and ambiguity list
- Clarification or negotiation questions
- Human-owned decision record

## Stop and escalation conditions

Stop when the offer is incomplete, the source version is unclear, a high-impact term is ambiguous, a deadline is uncertain, or legal, tax, immigration, or financial interpretation is required. Escalate rather than presenting regulated advice as a conclusion.

## Related controls

See [Human in the Loop](../HUMAN_IN_THE_LOOP.md), [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md), and the [Onboarding Workflow](ONBOARDING_WORKFLOW.md).
