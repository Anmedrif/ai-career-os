# Interview Preparation Workflow

## Purpose

Prepare truthful, role-relevant interview material and practice prompts without inventing experience, memorizing deceptive scripts, or exposing confidential information.

## Inputs

- Current verified posting
- Approved professional profile
- Approved targeted CV and application materials
- Opportunity assessment and identified gaps
- Interview format or agenda, if known
- [Interview answer template](../templates/INTERVIEW_ANSWER_TEMPLATE.md)

## Participating agents

- **Interview Builder Agent:** develops themes, questions, and practice material.
- **Professional Profile Agent:** validates personal evidence.
- **Evidence Checking Agent:** checks factual grounding and source consistency.
- **Quality Review Agent:** reviews relevance, clarity, tone, and completeness.
- **Privacy Review Agent:** prevents disclosure of protected employer, client, or third-party information.
- **Orchestrator Agent:** routes unresolved questions and approval.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every preparation record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). An answer set may be `Approved exact version` and `Content approved`; sending or publishing it requires a separate execution state.

## Procedure

1. Reopen and understand the official posting before drafting preparation content.
2. Build a role-to-evidence map covering responsibilities, requirements, risks, and likely question themes.
3. Create an evidence bank of genuine examples, each with context, action, result, and confidentiality boundary.
4. Draft concise answer outlines rather than claims the professional cannot naturally defend.
5. Distinguish direct experience, transferable experience, learning, and future intent.
6. Prepare gap-handling answers that acknowledge limits and show credible next steps.
7. Create questions for the employer using public or interview-provided context only.
8. Run mock evaluation for instruction following, relevance, grounding, consistency, privacy, and tone.
9. Revise weak answers while preserving the underlying facts.
10. Present the final preparation set for human approval and practice.

## Human approval gate

The professional approves final answer substance, sensitive disclosures, career explanations, and questions to the employer. Approval of preparation content does not authorize recording, sending, or publishing it.

## Outputs

- Interview evidence bank
- Role-specific question set
- Approved answer outlines
- Gap and risk handling plan
- Employer-question list
- Practice feedback and unresolved issues

## Stop and escalation conditions

Stop when an answer requires invented experience, undisclosed private information, legal advice, confidential examples, or reconciliation of conflicting career facts. Escalate unclear dates, metrics, employment transitions, and disclosure decisions.

## Related controls

Apply [Source Governance](../SOURCE_GOVERNANCE.md), the [Evaluation Framework](../EVALUATION_FRAMEWORK.md), and [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md).
