# Opportunity Assessment Template

Use with the [Opportunity Assessment Workflow](../workflows/OPPORTUNITY_ASSESSMENT_WORKFLOW.md). Narrative evidence takes priority over an aggregate score.

## Record metadata

| Field | Entry |
|---|---|
| Assessment ID | `[ASSESSMENT-ID]` |
| Opportunity ID and version | `[OPPORTUNITY-ID]` |
| Profile ID and version | `[PROFILE-ID]` |
| Goal ID and version | `[GOAL-ID]` |
| Assessment date | `[YYYY-MM-DD]` |
| Reviewer | `[Agent or human role]` |
| Evidence freshness | `[Current as of date / Recheck required]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded / Not applicable]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must also record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). An `ASSUMPTION` may affect a recommendation but cannot be presented as candidate or employer fact.

## Requirement-to-evidence matrix

| Opportunity requirement | Importance | Candidate evidence | Mapping | Information type and governed states | Notes |
|---|---|---|---|---|---|
| `[Requirement]` | `[Essential / Preferred / Context]` | `[SOURCE-ID or None]` | `[SUPPORTED / PARTIAL / GAP / UNKNOWN]` | `[FACT / ASSUMPTION]` | `[Reason]` |

## Fit dimensions

| Dimension | Evidence | Rating | Confidence | Material risk or gap |
|---|---|---|---|---|
| Role alignment | `[Evidence]` | `[Strong / Moderate / Weak / Unknown]` | `[High / Medium / Low]` | `[Issue]` |
| Transferable skills | `[Evidence]` | `[Rating]` | `[Confidence]` | `[Issue]` |
| Essential requirements | `[Evidence]` | `[Rating]` | `[Confidence]` | `[Issue]` |
| Work model and location | `[Evidence]` | `[Rating]` | `[Confidence]` | `[Issue]` |
| Eligibility and timing | `[Evidence]` | `[Rating]` | `[Confidence]` | `[Issue]` |
| Career-goal alignment | `[Evidence]` | `[Rating]` | `[Confidence]` | `[Issue]` |
| Application effort | `[Evidence]` | `[Low / Medium / High]` | `[Confidence]` | `[Issue]` |

## Critical factors

### Potential strengths

- `[FACT-backed strength]`

### Material gaps

- `[Gap and its impact]`

### Unknowns and assumptions

| Item | Why it matters | Current state | Validation action | Owner |
|---|---|---|---|---|
| `[Unknown]` | `[Impact]` | `[ASSUMPTION / Unknown]` | `[Action]` | `[Owner]` |

### Possible disqualifiers

- `[Condition, evidence, and confidence]`

## Optional scoring

If a score is useful, define weights before scoring.

| Criterion | Weight | Score (1-5) | Evidence | Weighted result |
|---|---:|---:|---|---:|
| `[Criterion]` | `[0-100%]` | `[1-5]` | `[Evidence]` | `[Value]` |

Critical-gap override: `[None / Describe]`

## Recommendation

- Recommended disposition: `[APPLY / HOLD / INVESTIGATE / DECLINE]`
- State: `RECOMMENDATION`
- Confidence: `[High / Medium / Low]`
- Reasons: `[Concise evidence-backed explanation]`
- Smallest useful next action: `[Action]`

## Human decision

| Decision | Rationale | Next action within scope | Date | Decision state |
|---|---|---|---|---|
| `[APPLY / HOLD / INVESTIGATE / DECLINE]` | `[Human rationale]` | `[Action or None]` | `[YYYY-MM-DD]` | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |

Approval to proceed does not authorize submission or employer contact.
