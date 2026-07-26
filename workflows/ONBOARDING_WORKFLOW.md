# Onboarding Workflow

## Purpose

Convert an accepted offer into a privacy-aware, human-controlled onboarding plan that tracks confirmed obligations, questions, readiness, and early learning without storing employer secrets.

## Inputs

- User-confirmed acceptance state
- Authorized onboarding instructions
- Confirmed start conditions
- Approved career goal and learning priorities
- User-selected tracking boundaries

## Participating agents

- **Career Strategy Agent:** aligns early goals with longer-term development.
- **Professional Profile Agent:** identifies transferable strengths and development needs.
- **Evidence Checking Agent:** distinguishes confirmed instructions from assumptions.
- **Privacy Review Agent:** prevents sensitive employer or identity data from entering the system.
- **Orchestrator Agent:** tracks dependencies, approvals, and completion evidence.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every onboarding record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). A plan may be `Approved exact version`; each external form, message, or commitment still requires `Externally authorized` and separate completion evidence.

## Procedure

1. Confirm that acceptance has actually occurred; do not infer it from an offer evaluation.
2. Record only minimum necessary onboarding facts and keep sensitive identity documents outside the repository.
3. Separate employer-required tasks from optional preparation.
4. Map dependencies, deadlines, owners, evidence of completion, and unresolved questions.
5. Identify tools or access needs without storing credentials, tokens, or private URLs.
6. Create a role-learning plan based on confirmed responsibilities and approved goals.
7. Define human-owned first-week, first-month, and first-quarter checkpoints.
8. Review the plan for privacy, unauthorized employer content, stale instructions, and unsupported assumptions.
9. Obtain user approval for the plan and any communication drafts.
10. Record completion only from observed evidence or user confirmation.

## Human approval gate

Human approval is required before sending forms or messages, sharing identity or banking data, accepting policies, changing start arrangements, or recording employer information. The system never signs or accepts terms.

## Outputs

- Minimal onboarding checklist
- Dependency and question register
- Access-readiness list without credentials
- Early learning and review plan
- Confirmed completion record

## Stop and escalation conditions

Stop when a task requests secrets or unnecessary sensitive data, instructions conflict, acceptance is not confirmed, an official system must be used, or legal or policy interpretation is required. Escalate to the professional or authorized employer contact.

## Related controls

Follow [Security](../SECURITY.md), [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md), and [Human in the Loop](../HUMAN_IN_THE_LOOP.md).
