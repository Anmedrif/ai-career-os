# Application Workflow

## Purpose

Assemble, validate, and track an application package while keeping preparation, approval, submission, and outcome as separate states.

## Inputs

- Human-approved opportunity disposition
- Approved targeted CV
- Approved supporting materials, where required
- Verified posting instructions and closing information
- [Application tracker template](../templates/APPLICATION_TRACKER_TEMPLATE.md)
- [Cover letter template](../templates/COVER_LETTER_TEMPLATE.md), when appropriate

## Participating agents

- **Orchestrator Agent:** controls package state and external-action gate.
- **CV Tailoring Agent:** supplies the approved CV.
- **Career Strategy Agent:** advises on optional materials.
- **Evidence Checking Agent:** validates form answers and claims.
- **Privacy Review Agent:** checks requested data and destination.
- **Quality Review Agent:** checks completeness and instruction compliance.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every application record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). Keep `Content approved`, `Externally authorized`, `Attempted`, `Completed`, and `Outcome recorded` distinct.

## Procedure

1. Reverify the live posting, destination, deadline, and required fields.
2. Create an application record before assembling materials.
3. List required and optional items; identify sensitive fields and legal attestations.
4. Populate answers only from authoritative sources or current user confirmation.
5. Create optional materials only when they add specific value.
6. Verify filenames, versions, links, language, and consistency across the package.
7. Run instruction-following, completeness, privacy, and factual-grounding review.
8. Present the exact package, destination, and unresolved questions for human approval.
9. Perform submission only after a separate explicit action authorization and through an authorized channel.
10. Record an observed attempt as `Attempted`, a verified submission completion as `Completed`, and any response separately as `Outcome recorded`. If evidence is absent, leave the outcome unresolved; never infer receipt.

## Human approval gate

Human approval is mandatory before answering sensitive questions, accepting declarations, uploading files, contacting an employer, or submitting. Material approval and submission authorization are separate gates.

## Outputs

- Application package manifest
- Validated form-response set
- Privacy and completeness check
- Approval record
- Submission evidence or an explicit not-submitted state
- Follow-up and status record

## Stop and escalation conditions

Stop for unexpected sensitive-data requests, legal attestations, conflicting application answers, ambiguous destination, changed posting requirements, authentication barriers, or any absence of explicit submission authorization. Escalate rather than attempting workarounds.

## Related controls

See [Human in the Loop](../HUMAN_IN_THE_LOOP.md), [Security](../SECURITY.md), [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md), and the [Interview Preparation Workflow](INTERVIEW_PREPARATION_WORKFLOW.md).
