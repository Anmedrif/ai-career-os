# Application Tracker Template

Use with the [Application Workflow](../workflows/APPLICATION_WORKFLOW.md). Preparation, material approval, submission authorization, submission evidence, and outcome are separate states.

## Tracker metadata

| Field | Entry |
|---|---|
| Tracker ID | `[TRACKER-ID]` |
| Owner | `[Human owner]` |
| Version | `[MAJOR.MINOR]` |
| Period covered | `[Start date to end date or Current]` |
| Last reconciled | `[YYYY-MM-DD]` |
| Privacy classification | `[Private / Internal]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must separately record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md).

## Application register

| Application ID | Opportunity ID | Document state | Execution state | Status evidence | Last verified | Next-action decision state |
|---|---|---|---|---|---|---|
| `[APPLICATION-ID]` | `[OPPORTUNITY-ID]` | `[Draft / Unapproved / Approved exact version / Current / Review required]` | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded]` | `[Evidence or None]` | `[YYYY-MM-DD]` | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |

## Per-application record

### `[APPLICATION-ID]`

| Field | Entry | Information state | Evidence |
|---|---|---|---|
| Opportunity version | `[ID and version]` | `FACT` | `[Source]` |
| Human disposition | `[Apply / Hold / Decline]` | `[Decision: Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` | `[Decision record]` |
| Deadline | `[Date / Unknown]` | `[FACT / ASSUMPTION]` | `[Source]` |
| Application channel | `[Verified channel / Unknown]` | `[FACT / ASSUMPTION]` | `[Source]` |
| Sensitive fields expected | `[Generic categories only]` | `[FACT / ASSUMPTION]` | `[Source]` |

## Material manifest

| Material | Exact version | Document state | Factual review | Privacy review | Execution state |
|---|---|---|---|---|---|
| `[CV / letter / form answers / other]` | `[Artifact ID]` | `[Draft / Unapproved / Approved exact version]` | `[Pass / Review]` | `[Pass / Review]` | `[Execution: Prepared / Content approved]` |

## External-action gate

| Check | Result |
|---|---|
| Exact destination verified | `[Yes / No]` |
| Exact materials displayed to human | `[Yes / No]` |
| Unresolved answers cleared | `[Yes / No]` |
| Legal declarations reviewed by human | `[Yes / No / Not applicable]` |
| Explicit submission authorization captured | `[Yes / No]` |
| Authorization scope and time | `[Record]` |

## Submission and outcome evidence

| Event | Observed evidence | Timestamp | Evidence and execution states | Notes |
|---|---|---|---|---|
| Submission attempt | `[Receipt, confirmation, error, or None]` | `[Timestamp]` | `[Evidence: Directly evidenced / User-confirmed / Unresolved; Execution: Attempted / Completed]` | |
| Employer response | `[Generic status; exclude private correspondent data]` | `[Timestamp]` | `[Evidence: Directly evidenced / User-confirmed / Unresolved; Execution: Outcome recorded when preserved]` | |
| Outcome | `[Advance / Reject / Withdraw / Offer / Unknown]` | `[Timestamp]` | `[Evidence: Directly evidenced / User-confirmed / Unresolved; Execution: Outcome recorded when preserved]` | |

## Follow-up

| Proposed action | Basis | Owner | Due date | Information type and decision state |
|---|---|---|---|---|
| `[Action]` | `[Evidence or policy]` | `[Human / agent]` | `[YYYY-MM-DD]` | `[Type: RECOMMENDATION / DECISION; Decision: Proposed / Pending human decision / Approved within stated scope / Rejected]` |

Never infer a successful submission or outcome from a prepared package.
