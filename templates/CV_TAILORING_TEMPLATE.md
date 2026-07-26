# CV Tailoring Template

Use with the [CV Tailoring Workflow](../workflows/CV_TAILORING_WORKFLOW.md). This record documents a new targeted version; it does not authorize overwriting a base CV or submitting the result.

## Record metadata

| Field | Entry |
|---|---|
| Tailoring record ID | `[TAILOR-ID]` |
| Opportunity ID | `[OPPORTUNITY-ID]` |
| Assessment ID | `[ASSESSMENT-ID]` |
| Profile version | `[PROFILE-ID and version]` |
| Base CV version | `[CV-ID and version]` |
| Target CV version | `[CV-ID and new version]` |
| Created | `[YYYY-MM-DD]` |
| Intended use | `[Named opportunity only / Other bounded use]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded]` |
| Approved exact artifact | `[Artifact ID or Not yet approved]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must also record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). `Approved exact version`, `Content approved`, and `Externally authorized` remain separate.

## Requirement-to-evidence plan

| Requirement or keyword | Importance | Verified evidence | Proposed CV location | Information type and governed states | Include? |
|---|---|---|---|---|---|
| `[Requirement]` | `[Essential / Preferred / Context]` | `[SOURCE-ID or None]` | `[Summary / Skills / Role entry / Education / Omit]` | `[FACT / ASSUMPTION]` | `[DECISION pending / Yes / No]` |

## Proposed positioning

| Element | Proposed wording or approach | Supporting facts | Document and evidence states | Reviewer note |
|---|---|---|---|---|
| Headline | `[Concise role-relevant wording]` | `[SOURCE-IDs]` | `[Evidence state; Document state: Draft / Unapproved / Approved exact version]` | |
| Summary | `[Two to four evidence-backed lines]` | `[SOURCE-IDs]` | `[Evidence state; Document state: Draft / Unapproved / Approved exact version]` | |
| Core skills | `[Selected verified skills]` | `[SOURCE-IDs]` | `[Evidence state; Document state: Draft / Unapproved / Approved exact version]` | |

## Experience edits

| Entry and element | Current wording | Proposed wording | Evidence | Reason | Information type and governed states |
|---|---|---|---|---|---|
| `[Role ID; bullet or field]` | `[Current text]` | `[Proposed text]` | `[SOURCE-ID]` | `[Relevance / clarity / order]` | `[Type: RECOMMENDATION; Evidence state; Decision state; Document state: Draft]` |

## Content controls

| Check | Result | Evidence or note |
|---|---|---|
| Employment titles and dates unchanged unless separately corrected | `[Pass / Fail / Review]` | `[Note]` |
| No unsupported metric or achievement | `[Pass / Fail / Review]` | `[Note]` |
| Direct and transferable experience are distinguished | `[Pass / Fail / Review]` | `[Note]` |
| Required context preserved | `[Pass / Fail / Review]` | `[Note]` |
| Personal data minimized | `[Pass / Fail / Review]` | `[Note]` |
| Keywords read naturally | `[Pass / Fail / Review]` | `[Note]` |

## Exclusions and unresolved items

| Item | Reason excluded or unresolved | Required evidence or decision | Impact |
|---|---|---|---|
| `[Claim or requirement]` | `[Reason]` | `[Need]` | `[Impact on CV or fit]` |

## Version review

- Predecessor preserved: `[Yes / No]`
- Changed sections listed: `[Yes / No]`
- Unrelated claims unchanged: `[Pass / Fail / Review]`
- Factual-grounding review: `[Pass / Fail / Review]`
- Privacy review: `[Pass / Fail / Review]`
- Format and link review: `[Pass / Fail / Review]`

## Human approval

| Decision | Exact version | Permitted use | Date | Decision, document, and execution states |
|---|---|---|---|---|
| `[Approve / Revise / Reject]` | `[Artifact ID and version]` | `[Named use]` | `[YYYY-MM-DD]` | `[Decision: Approved within stated scope; Document: Approved exact version; Execution: Content approved / Prepared]` |
