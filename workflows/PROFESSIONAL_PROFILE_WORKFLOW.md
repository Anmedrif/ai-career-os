# Professional Profile Workflow

## Purpose

Build a single, evidence-backed professional profile that downstream CV, interview, LinkedIn, portfolio, and application workflows can use without factual drift.

## Inputs

- Completed [professional profile template](../templates/PROFESSIONAL_PROFILE_TEMPLATE.md)
- Evidence supplied or confirmed by the professional
- Existing public-safe career documents, where authorized
- Target-role context, if already decided
- Rules in [Source Governance](../SOURCE_GOVERNANCE.md) and [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md)

## Participating agents

- **Professional Profile Agent:** structures facts and identifies evidence gaps.
- **Evidence Checking Agent:** tests each claim against the stated source.
- **Privacy Review Agent:** removes or generalizes data that is unnecessary for the intended use.
- **Quality Review Agent:** checks completeness, consistency, and language.
- **Orchestrator Agent:** controls handoffs and prevents unresolved fields from becoming facts.

## State model

Use an optional information-type tag (`FACT`, `DECISION`, `ASSUMPTION`, or `RECOMMENDATION`) only to describe the field's content. Record the applicable governed dimensions separately:

- **Evidence state:** directly evidenced, user-confirmed, source-supported, inference, contradictory, unresolved, or historical.
- **Decision state:** proposed, pending human decision, approved within stated scope, rejected, withdrawn, or superseded.
- **Document state:** draft, unapproved, approved exact version, current, historical predecessor, review required, or approved decision pending integration.
- **Execution state:** prepared, content approved, externally authorized, attempted, completed, or outcome recorded.

See [Source Governance](../SOURCE_GOVERNANCE.md). Never use a bare `APPROVED` state.

## Procedure

1. Define the profile's intended uses and privacy boundary.
2. Inventory claims by category: experience, education, languages, skills, certifications, projects, and career direction.
3. Attach a source reference and the applicable governed state fields to every material claim.
4. Separate direct facts from interpretations such as "strong communicator" or "AI specialist."
5. Flag missing dates, unclear proficiency levels, unsupported metrics, and inconsistent role descriptions.
6. Resolve conflicts using the source-priority rules; do not select the most favorable version merely because it reads better.
7. Draft a concise professional summary using only fact claims with an adequate evidence state and decisions approved within stated scope. Keep the new wording at document state `Draft`.
8. Run factual-grounding, privacy, internal-consistency, and unsupported-claim checks using the [Evaluation Framework](../EVALUATION_FRAMEWORK.md).
9. Present unresolved items and the sanitized draft for human review.
10. After approval, record scope, date, and version. Approval for one use does not automatically authorize public publication.

## Human approval gate

Human approval is required before the profile becomes the authoritative profile, before public use, and before adding achievements, metrics, dates, identity details, or sensitive work information. See [Human in the Loop](../HUMAN_IN_THE_LOOP.md).

## Outputs

- Versioned authoritative professional profile
- Claim-to-source register
- Unresolved-facts queue
- Public-safe summary, if separately approved
- Change log recording approved corrections

## Stop and escalation conditions

Stop and escalate when sources conflict, evidence is unavailable, public status is unclear, a claim concerns confidential work, a requested metric is unsupported, or the professional disputes the proposed wording. Never fill a gap from model memory or general knowledge.
