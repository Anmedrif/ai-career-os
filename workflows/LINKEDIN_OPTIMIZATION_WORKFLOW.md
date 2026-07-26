# LinkedIn Optimization Workflow

## Purpose

Improve one LinkedIn profile section at a time while maintaining consistency with the approved professional profile, CV, portfolio, and privacy decisions.

## Inputs

- User-provided current section content
- Approved professional profile and career goal
- Approved public projects and credentials
- [LinkedIn profile template](../templates/LINKEDIN_PROFILE_TEMPLATE.md)
- Current platform constraints and visibility settings

## Participating agents

- **LinkedIn Optimization Agent:** audits and drafts section-specific improvements.
- **Professional Profile Agent:** validates all career claims.
- **Career Strategy Agent:** checks positioning against the approved goal.
- **Quality Review Agent:** reviews clarity, keywords, tone, and consistency.
- **Privacy Review Agent:** checks public exposure and unnecessary personal data.
- **Orchestrator Agent:** enforces section order and approval gates.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every section record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). Exact section text may be `Approved exact version` and `Content approved`; a platform edit requires `Externally authorized`.

## Procedure

1. Confirm target role and public positioning before editing profile text.
2. Audit one section at a time in this order: headline, About, experience, skills, certifications, projects, and Featured content.
3. Compare the current section with the authoritative profile and target-role language.
4. Identify factual, consistency, privacy, clarity, and discoverability issues.
5. Draft a concise English revision using only verified public-safe information.
6. Explain material changes, tag optimization advice as `RECOMMENDATION`, and record its governed states separately.
7. Cross-check the draft against approved CV, portfolio, and interview positioning.
8. Run privacy, unsupported-claim, tone, and format checks.
9. Obtain approval for the exact section.
10. Update the working plan only after the user confirms what was actually changed on the platform.

## Human approval gate

Human approval is required before finalizing each section, publishing content, changing visibility, enabling job-search signals, adding contact details, or making direct platform changes. No approval is implied across sections.

## Outputs

- Section audit
- Approved section text
- Claim and keyword traceability notes
- Consistency checklist
- Pending platform-action list

## Stop and escalation conditions

Stop if the current section has not been provided, an improvement depends on an unverified claim, platform access is unavailable, privacy settings are unclear, or a requested direct change lacks authorization. Escalate conflicts between public positioning and approved career records.

## Related controls

See [Source Governance](../SOURCE_GOVERNANCE.md), [Human in the Loop](../HUMAN_IN_THE_LOOP.md), and [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md).
