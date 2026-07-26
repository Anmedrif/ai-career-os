# LinkedIn Profile Template

Use with the [LinkedIn Optimization Workflow](../workflows/LINKEDIN_OPTIMIZATION_WORKFLOW.md). Complete and approve one section at a time.

## Record metadata

| Field | Entry |
|---|---|
| Working-plan ID | `[LINKEDIN-ID]` |
| Profile source version | `[PROFILE-ID and version]` |
| Career goal version | `[GOAL-ID and version]` |
| Target audience | `[Recruiters / hiring managers / peers / other]` |
| Audit date | `[YYYY-MM-DD]` |
| Platform content supplied by | `[Human owner]` |
| Public exposure level | `[Public / Connections / Private setting]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must separately record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). A section remains document state `Draft` until its exact version is approved.

## Positioning decisions

| Decision | Selected value | Alternatives | Reason | Decision state |
|---|---|---|---|---|
| Target role family | `[Value]` | `[Alternatives]` | `[Reason]` | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Public professional identity | `[Value]` | `[Alternatives]` | `[Reason]` | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Visibility boundary | `[Value]` | `[Alternatives]` | `[Reason]` | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |

## Section worksheet

Repeat this block for each section in order.

### `[Headline / About / Experience / Skills / Certifications / Projects / Featured]`

Current content supplied by the professional:

> `[Paste or summarize the current section. Remove unnecessary contact data before storage.]`

Audit:

| Issue | Evidence | Impact | Information type and governed states |
|---|---|---|---|
| `[Accuracy / clarity / consistency / privacy / keyword / format issue]` | `[SOURCE-ID or reviewer observation]` | `[Impact]` | `[FACT / RECOMMENDATION]` |

Proposed English version:

> `[Draft section content using only verified public-safe facts.]`

Document state: `Draft`

Claim map:

| Proposed claim | Profile source | Public-use decision state | Information type and governed states |
|---|---|---|---|
| `[Claim]` | `[SOURCE-ID]` | `[Pending human decision / Approved within stated scope / Rejected]` | `[Type: FACT; Evidence state; Document state: Draft]` |

Section decision:

| Decision | Exact version | Date | Decision, document, and execution states |
|---|---|---|---|
| `[Approve / Revise / Keep current / Remove]` | `[Version ID]` | `[YYYY-MM-DD]` | `[Decision: Approved within stated scope; Document: Approved exact version; Execution: Content approved / Prepared]` |

## Profile consistency check

| Comparison | Result | Conflict or action |
|---|---|---|
| LinkedIn vs. authoritative profile | `[Pass / Review]` | `[Issue]` |
| LinkedIn vs. current CV | `[Pass / Review]` | `[Issue]` |
| LinkedIn vs. portfolio | `[Pass / Review]` | `[Issue]` |
| LinkedIn vs. interview positioning | `[Pass / Review]` | `[Issue]` |

## Platform-action register

| Action | Exact content or setting | Performed by | Observed result | Governed states |
|---|---|---|---|---|
| `[Action]` | `[Version or setting]` | `[Human / authorized tool]` | `[Changed / Not changed / Unknown]` | `[Decision state; Document state; Execution: Externally authorized / Attempted / Completed / Outcome recorded]` |

No template approval authorizes direct platform changes.
