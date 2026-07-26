# Professional Profile Template

Use this template with the [Professional Profile Workflow](../workflows/PROFESSIONAL_PROFILE_WORKFLOW.md). Keep sensitive contact, identity, immigration, financial, and account data outside this record.

## Record metadata

| Field | Entry |
|---|---|
| Record ID | `[PROFILE-ID]` |
| Version | `[MAJOR.MINOR]` |
| Owner | `[Professional or authorized owner]` |
| Created | `[YYYY-MM-DD]` |
| Last reviewed | `[YYYY-MM-DD]` |
| Intended uses | `[CV / interview / LinkedIn / portfolio / other]` |
| Source snapshot | `[List source IDs and versions, not private local paths]` |
| Privacy classification | `[Private / Internal / Public-safe candidate]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded / Not applicable]` |
| Approved by and date | `[Human approver; YYYY-MM-DD]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. For every material entry, also record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). Never use a bare `APPROVED` value.

## Professional direction

| Field | Content | Information type and governed states | Source or decision record | Notes |
|---|---|---|---|---|
| General professional identity | `[Neutral, evidence-backed description]` | `[Type; Evidence state; Decision state; Document state]` | `[SOURCE-ID]` | |
| Target role family | `[Role family]` | `[Type; Evidence state; Decision state; Document state]` | `[DECISION-ID]` | |
| Preferred work context | `[General context]` | `[Type; Evidence state; Decision state; Document state]` | `[DECISION-ID]` | |
| Career direction | `[One or two sentences]` | `[Type; Evidence state; Decision state; Document state]` | `[SOURCE/DECISION-ID]` | |

## Professional summary

`[Draft a concise summary using adequately evidenced fact claims and decisions approved within stated scope.]`

Summary document state: `[Draft / Unapproved / Approved exact version]`
Summary execution state: `[Prepared / Content approved]`

## Experience register

Repeat for each relevant role. Do not include confidential duties or third-party personal data.

### `[Role record ID]`

| Field | Content | Information type and governed states | Source | Public-safe? |
|---|---|---|---|---|
| Organization description | `[Public name if approved within stated scope, otherwise generic sector]` | `[Type; Evidence state; Decision state; Document state]` | `[SOURCE-ID]` | `[Yes / No / Review]` |
| Role title | `[Verified title]` | `[Type; Evidence state; Decision state; Document state]` | `[SOURCE-ID]` | |
| Dates | `[Verified month/year range or approved granularity]` | `[Type; Evidence state; Decision state; Document state]` | `[SOURCE-ID]` | |
| Responsibilities | `[Evidence-backed responsibilities]` | `[Type; Evidence state; Decision state; Document state]` | `[SOURCE-ID]` | |
| Outcomes | `[Verified outcomes; no unsupported metrics]` | `[Type; Evidence state; Decision state; Document state]` | `[SOURCE-ID]` | |
| Transferable evidence | `[Interpretation kept distinct from direct experience]` | `[Type: RECOMMENDATION; Evidence state; Decision state]` | `[Reviewer note]` | |

## Skills and tools

| Skill or tool | Proficiency wording | Evidence | Information type and governed states | Last verified |
|---|---|---|---|---|
| `[Item]` | `[Observed level; avoid inflation]` | `[SOURCE-ID]` | `[Type; Evidence state; Decision state; Document state]` | `[YYYY-MM-DD]` |

## Languages

| Language | Capability description | Evidence or confirmation | Information type and governed states | Public-use decision |
|---|---|---|---|---|
| `[Language]` | `[Specific, supportable level]` | `[SOURCE/DECISION-ID]` | `[Type; Evidence state; Decision state; Document state]` | `[Pending human decision / Approved within stated scope / Rejected]` |

## Education, certifications, and learning

| Item | Provider or institution | Completion status | Dates | Evidence | Information type and governed states |
|---|---|---|---|---|---|
| `[Qualification or course]` | `[Public-safe name]` | `[Completed / In progress / Planned]` | `[Date range]` | `[SOURCE-ID]` | `[Type; Evidence state; Decision state; Document state]` |

## Projects

| Project | Contribution | Tools or methods | Evidence | Information type and governed states | Public-safe status |
|---|---|---|---|---|---|
| `[Project title]` | `[Exact personal contribution]` | `[Verified list]` | `[SOURCE-ID]` | `[Type; Evidence state; Decision state; Document state]` | `[Approved within stated scope / Pending human decision / Exclude]` |

## Unresolved facts and conflicts

| Issue | Conflicting or missing sources | Impact | Required confirmation | Owner |
|---|---|---|---|---|
| `[Issue]` | `[SOURCE-IDs]` | `[Where reuse is blocked]` | `[Question]` | `[Human / agent]` |

## Approval checklist

- [ ] Every material claim has a source or decision record.
- [ ] Assumptions are excluded from confirmed wording.
- [ ] Metrics, dates, titles, and qualifications are verified.
- [ ] Public-safe fields have separate publication approval.
- [ ] Privacy and consistency reviews are complete.
- [ ] Exact version approved by the human owner.
