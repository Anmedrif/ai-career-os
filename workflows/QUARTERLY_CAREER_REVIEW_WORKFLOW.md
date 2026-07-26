# Quarterly Career Review Workflow

## Purpose

Run a periodic evidence-based review of goals, activities, outcomes, skills, materials, and next-quarter priorities without rewriting history or treating activity volume as success.

## Inputs

- Previous approved career goal and review
- [Quarterly review template](../templates/QUARTERLY_REVIEW_TEMPLATE.md)
- Application tracker and verified outcomes
- Current professional profile
- Skills-gap assessment and learning evidence
- Portfolio, LinkedIn, and interview-preparation records

## Participating agents

- **Career Strategy Agent:** analyzes progress and trade-offs.
- **Professional Profile Agent:** identifies verified profile changes.
- **Opportunity Assessment Agent:** reviews pipeline quality and fit.
- **Quality Review Agent:** tests conclusions and measurement quality.
- **Evidence Checking Agent:** validates outcomes and prevents selective reporting.
- **Orchestrator Agent:** prepares decisions for human approval.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every review record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). The review artifact may be `Approved exact version`; each adopted change requires a decision `Approved within stated scope` and integration in its owning source.

## Procedure

1. Freeze the review period, source set, and prior approved goals.
2. Reconcile activity records with observed outcomes; use evidence state `Unresolved` where outcome evidence is absent.
3. Compare planned and completed work without manufacturing success metrics.
4. Analyze opportunity quality, application conversion, material performance, interview signals, portfolio progress, learning evidence, and consistency issues.
5. Separate the information types `FACT`, `ASSUMPTION`, and `RECOMMENDATION`, and record the applicable governed states for each.
6. Identify what to continue, stop, start, or investigate.
7. Update the skills-gap view using demonstrated evidence, not course enrollment alone.
8. Propose at most a manageable set of next-quarter priorities, measures, and review dates.
9. Run completeness, factual-grounding, bias, privacy, and consistency checks.
10. Submit proposed goal, profile, and workflow changes for individual human decisions.

## Human approval gate

The professional approves the review narrative, goal changes, new priorities, profile updates, and any publication of results. A review recommendation never changes authoritative records automatically.

## Outputs

- Approved quarterly review
- Evidence and data-quality notes
- Continue/stop/start/investigate decisions
- Updated skills-gap recommendations
- Next-quarter plan and review date
- Separate change requests for authoritative records

## Stop and escalation conditions

Stop when records are materially incomplete, outcomes are inferred, definitions changed during the period, private employer information would be exposed, or a recommendation depends on an unresolved career decision. Escalate major goal trade-offs and source conflicts.

## Related controls

Use [Source Governance](../SOURCE_GOVERNANCE.md), the [Evaluation Framework](../EVALUATION_FRAMEWORK.md), and [Career Lifecycle](../CAREER_LIFECYCLE.md).
