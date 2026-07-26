# Portfolio Development Workflow

## Purpose

Turn genuine work into a public-safe case study that demonstrates decisions, methods, evaluation, and limitations without exposing private data or overstating authorship.

## Inputs

- Approved career goal and public positioning
- Project source material the professional is authorized to use
- [Portfolio project template](../templates/PORTFOLIO_PROJECT_TEMPLATE.md)
- Contribution evidence and tool-use notes
- Publication constraints

## Participating agents

- **Portfolio Agent:** designs the case-study narrative and repository structure.
- **Evidence Checking Agent:** verifies contribution and outcome claims.
- **Privacy Review Agent:** classifies, rewrites, anonymizes, or excludes source material.
- **Quality Review Agent:** tests clarity, usefulness, and technical credibility.
- **Career Strategy Agent:** checks relevance to the target role.
- **Orchestrator Agent:** maintains the publication gate.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every portfolio record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). `Approved exact version` and `Content approved` do not mean `Externally authorized`; publication remains a separate execution transition.

## Procedure

1. Define audience, learning objective, and the capability the case study should evidence.
2. Inventory source material and classify each item for public use.
3. Exclude secrets, personal data, private correspondence, real application data, proprietary material, and unapproved employer or client information.
4. Separate the professional's contribution from model-generated, team-generated, or third-party work.
5. Reconstruct reusable concepts in generic language rather than copying private source files.
6. Use synthetic data for demonstrations and label it clearly.
7. Document the problem, constraints, architecture, workflow, evaluation method, results, limitations, and responsible-use controls.
8. Validate relative links, terminology, factual claims, privacy, and reproducibility.
9. Run secret and personal-data checks on the exact publication candidate.
10. Present the artifact, exclusions, unresolved facts, and checks for human approval.

## Human approval gate

Human approval is required before using personal identity, naming organizations, stating achievements, selecting a license, committing a release, publishing, or pushing to a public service. Content approval and publication authorization are distinct.

## Outputs

- Public-safe portfolio artifact
- Source classification and sanitization record
- Honest author-contribution statement
- Limitations and disclosure notes
- Publication checklist and approval status

## Stop and escalation conditions

Stop when ownership is unclear, content may be proprietary, a claim cannot be evidenced, anonymization may be reversible, a secret scan raises a finding, or the publication channel is not explicitly authorized. Escalate licensing and attribution questions.

## Related controls

Follow [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md), [Security](../SECURITY.md), [Source Governance](../SOURCE_GOVERNANCE.md), and [Publishing Checklist](../PUBLISHING_CHECKLIST.md).
