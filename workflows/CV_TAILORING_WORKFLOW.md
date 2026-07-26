# CV Tailoring Workflow

## Purpose

Create a role-specific CV that improves relevance while preserving the verified career record, document lineage, and human control over every consequential claim.

## Inputs

- Approved professional profile
- Verified opportunity and approved assessment
- Approved base CV, if available
- [CV tailoring template](../templates/CV_TAILORING_TEMPLATE.md)
- Positioning and formatting standards

## Participating agents

- **CV Tailoring Agent:** selects and orders relevant evidence.
- **Professional Profile Agent:** checks every claim against the authoritative profile.
- **Evidence Checking Agent:** validates traceability and metrics.
- **Quality Review Agent:** reviews clarity, relevance, completeness, and format.
- **Privacy Review Agent:** removes unnecessary sensitive data.
- **Orchestrator Agent:** preserves version and approval boundaries.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every tailoring record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). A reviewed CV can be `Approved exact version` and `Content approved`; submission still requires `Externally authorized`.

## Procedure

1. Freeze the source versions: profile, posting, assessment, and base CV.
2. Build a requirement-to-evidence map and identify unsupported or weak areas.
3. Select relevant verified content; do not remove context in a way that changes meaning.
4. Draft headline, summary, skills, and experience bullets using faithful language and no invented metrics.
5. Preserve dates, employers, titles, education, certifications, and language levels unless the authoritative source is separately corrected.
6. Record every substantive change and its rationale in the tailoring template.
7. Check keyword coverage for natural relevance rather than repetition.
8. Run factual-grounding, consistency, privacy, format, and unsupported-claim checks.
9. Compare the tailored version with its predecessor and verify that unrelated claims did not change.
10. Submit the exact artifact and change summary for human review.

## Human approval gate

The professional must approve the exact CV version, its public or application use, all new wording about achievements, and any metric. Approval to tailor does not authorize submission or replacement of the base CV.

## Outputs

- Versioned targeted CV
- Requirement-to-evidence map
- Change and provenance record
- Unresolved issues list
- Human approval status

## Stop and escalation conditions

Stop when the role requires an unsupported claim, a source conflict affects employment history, a metric lacks evidence, the base version is unclear, or privacy risk cannot be resolved by omission. Escalate requests to overstate experience or conceal a material fact.

## Related controls

Follow [Source Governance](../SOURCE_GOVERNANCE.md), [Human in the Loop](../HUMAN_IN_THE_LOOP.md), and [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md). Continue through the [Application Workflow](APPLICATION_WORKFLOW.md) only after approval.
