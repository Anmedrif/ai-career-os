# Job Opportunity Template

Use with the [Job Discovery Workflow](../workflows/JOB_DISCOVERY_WORKFLOW.md). Record facts from the original source; never treat search snippets or model summaries as authoritative.

## Record metadata

| Field | Entry |
|---|---|
| Opportunity ID | `[OPPORTUNITY-ID]` |
| Captured | `[YYYY-MM-DD HH:MM timezone]` |
| Last verified | `[YYYY-MM-DD]` |
| Source type | `[Official posting / Authorized board / Other]` |
| Public source URL | `[URL or source reference]` |
| Freshness status | `[Current / Expired / Unclear]` |
| Record owner | `[Owner]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded / Not applicable]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must also record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md).

## Opportunity summary

| Field | Value | Information type and governed states | Source location | Confidence |
|---|---|---|---|---|
| Organization | `[Public organization or generic label]` | `[Type; Evidence state; Decision state; Document state]` | `[Source section]` | `[High / Medium / Low]` |
| Role title | `[Title]` | `[Type; Evidence state; Decision state; Document state]` | `[Source section]` | |
| Location | `[General location]` | `[Type; Evidence state; Decision state; Document state]` | `[Source section]` | |
| Work model | `[On-site / Hybrid / Remote / Unknown]` | `[Type; Evidence state; Decision state; Document state]` | `[Source section]` | |
| Employment type | `[Type / Unknown]` | `[Type; Evidence state; Decision state; Document state]` | `[Source section]` | |
| Posting or requisition reference | `[Public reference only]` | `[Type; Evidence state; Decision state; Document state]` | `[Source section]` | |
| Deadline | `[Date / Not stated]` | `[Type; Evidence state; Decision state; Document state]` | `[Source section]` | |

## Responsibilities

| Responsibility | Essential? | Source | Information type and governed states | Notes |
|---|---|---|---|---|
| `[Responsibility]` | `[Yes / No / Unclear]` | `[Source section]` | `[FACT / ASSUMPTION]` | |

## Requirements

| Requirement | Category | Required or preferred | Source | Information type and governed states |
|---|---|---|---|---|
| `[Requirement]` | `[Experience / Skill / Language / Education / Eligibility / Other]` | `[Required / Preferred / Unclear]` | `[Source section]` | `[FACT / ASSUMPTION]` |

## Practical conditions

| Condition | Source-backed value | Information type and governed states | Unresolved question |
|---|---|---|---|
| Schedule | `[Value / Not stated]` | `[STATE]` | `[Question]` |
| Travel or relocation | `[Value / Not stated]` | `[STATE]` | `[Question]` |
| Compensation | `[Record only if authorized and useful; otherwise Not collected]` | `[STATE]` | `[Question]` |
| Eligibility | `[Value / Not stated]` | `[STATE]` | `[Question]` |

## Verification and screening

- Original posting opened: `[Yes / No]`
- Source identity verified: `[Yes / No / Unclear]`
- Duplicate check result: `[Unique / Duplicate of ID / Unclear]`
- Obvious exclusion condition: `[None / Describe generically]`
- Sensitive third-party data omitted: `[Yes / No]`
- Recheck date: `[YYYY-MM-DD]`

## Discovery recommendation

Recommendation: `[ASSESS / HOLD / EXCLUDE / REVERIFY]`

State: `[RECOMMENDATION]`

Reason: `[Concise evidence-based explanation]`

Human disposition decision state: `[Pending human decision / Approved within stated scope for assessment / Rejected / Withdrawn / Superseded]`
