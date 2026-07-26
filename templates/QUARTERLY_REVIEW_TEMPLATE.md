# Quarterly Review Template

Use with the [Quarterly Career Review Workflow](../workflows/QUARTERLY_CAREER_REVIEW_WORKFLOW.md). Preserve unknown outcomes and data limitations rather than converting incomplete records into favorable conclusions.

## Record metadata

| Field | Entry |
|---|---|
| Review ID | `[REVIEW-ID]` |
| Period | `[YYYY-Q# or date range]` |
| Prior goal version | `[GOAL-ID and version]` |
| Profile version | `[PROFILE-ID and version]` |
| Data cutoff | `[YYYY-MM-DD]` |
| Reviewer | `[Human and agent roles]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded / Not applicable]` |
| Approved by and date | `[Human approver; YYYY-MM-DD]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must separately record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). Explanations of why a result occurred remain information type `ASSUMPTION` with evidence state `Inference` until supported.

## Executive review

| Prompt | Response | Information type and governed states | Evidence |
|---|---|---|---|
| What materially changed? | `[Summary]` | `[Type: FACT; Evidence state; Document state: Draft]` | `[SOURCE-IDs]` |
| What did not change? | `[Summary]` | `[Type: FACT; Evidence state; Document state: Draft]` | `[SOURCE-IDs]` |
| What decision is now required? | `[Decision question]` | `[Type: DECISION; Decision state: Pending human decision; Document state: Draft]` | `[Context]` |

## Goal progress

| Goal or milestone | Planned evidence | Observed evidence | Operational result | Data quality | Information type and governed states |
|---|---|---|---|---|---|
| `[Item]` | `[Expected result]` | `[Observed result or None]` | `[Complete / Partial / Not complete / Unknown]` | `[High / Medium / Low]` | `[FACT]` |

## Activity and outcomes

| Area | Activity | Observed outcome | Interpretation | Interpretation state |
|---|---|---|---|---|
| Opportunity discovery | `[Count or qualitative summary with stable definition]` | `[Outcome]` | `[Possible explanation]` | `[ASSUMPTION]` |
| Applications | `[Activity]` | `[Outcome]` | `[Possible explanation]` | `[ASSUMPTION]` |
| Interviews | `[Activity]` | `[Outcome]` | `[Possible explanation]` | `[ASSUMPTION]` |
| Learning | `[Activity]` | `[Demonstrated evidence]` | `[Possible explanation]` | `[ASSUMPTION]` |
| Portfolio and LinkedIn | `[Activity]` | `[Observed change]` | `[Possible explanation]` | `[ASSUMPTION]` |

## Quality and consistency findings

| Finding | Affected artifact or workflow | Evidence | Severity | Proposed action | Information type and governed states |
|---|---|---|---|---|---|
| `[Finding]` | `[Record ID]` | `[Evidence]` | `[Critical / Material / Minor]` | `[Action]` | `[FACT / RECOMMENDATION]` |

## Continue, stop, start, investigate

| Category | Item | Reason | Evidence | Information type and governed states |
|---|---|---|---|---|
| Continue | `[Item]` | `[Reason]` | `[Evidence]` | `[RECOMMENDATION]` |
| Stop | `[Item]` | `[Reason]` | `[Evidence]` | `[RECOMMENDATION]` |
| Start | `[Item]` | `[Reason]` | `[Evidence]` | `[RECOMMENDATION]` |
| Investigate | `[Item]` | `[Reason]` | `[Evidence gap]` | `[RECOMMENDATION]` |

## Next-quarter proposal

| Priority | Action | Success evidence | Guardrail | Owner | Review date | Decision state |
|---:|---|---|---|---|---|---|
| `[1]` | `[Action]` | `[Observable result]` | `[Limit or stop condition]` | `[Owner]` | `[YYYY-MM-DD]` | `[RECOMMENDATION / DECISION]` |

## Separate change decisions

| Authoritative record | Proposed change | Evidence | Human decision | Decision state |
|---|---|---|---|---|
| `[Profile / goal / workflow / material]` | `[Change]` | `[SOURCE-ID]` | `[Approve / Reject / Defer]` | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |

## Approval checklist

- [ ] Period and source set are fixed.
- [ ] Activity and outcome are distinguished.
- [ ] Unknown outcomes remain unknown.
- [ ] Interpretations are labeled assumptions.
- [ ] Private employer and third-party information is excluded.
- [ ] Each authoritative-record change received a separate decision.
- [ ] The next review date is approved.
