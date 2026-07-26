# Portfolio Project Template

Use with the [Portfolio Development Workflow](../workflows/PORTFOLIO_DEVELOPMENT_WORKFLOW.md). Replace private source material with public-safe explanations and synthetic examples.

## Record metadata

| Field | Entry |
|---|---|
| Project record ID | `[PROJECT-ID]` |
| Working title | `[Public-safe title]` |
| Version | `[MAJOR.MINOR]` |
| Intended audience | `[Audience]` |
| Target capability | `[Capability the project demonstrates]` |
| Source audit reference | `[AUDIT-ID]` |
| Created or updated | `[YYYY-MM-DD]` |
| License status | `[Not selected / Approved license]` |
| Document state | `[Draft / Unapproved / Approved exact version / Current / Historical predecessor / Review required]` |
| Decision state | `[Proposed / Pending human decision / Approved within stated scope / Rejected / Withdrawn / Superseded]` |
| Execution state | `[Prepared / Content approved / Externally authorized / Attempted / Completed / Outcome recorded]` |

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every material entry must separately record the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). Never collapse `Approved exact version`, `Content approved`, and `Externally authorized`.

## Project brief

| Field | Content | Information type and governed states | Evidence |
|---|---|---|---|
| Problem | `[Generic problem statement]` | `[Type; Evidence state; Decision state; Document state: Draft]` | `[SOURCE-ID]` |
| Intended users | `[Generic user group]` | `[Type; Evidence state; Decision state; Document state: Draft]` | `[SOURCE/DECISION-ID]` |
| Constraints | `[Privacy, evidence, tool, and scope constraints]` | `[FACT / DECISION]` | `[ID]` |
| Proposed solution | `[Concise system description]` | `[Type; Evidence state; Decision state; Document state: Draft]` | `[SOURCE-ID]` |
| Success criteria | `[Observable and supportable criteria]` | `[DECISION]` | `[DECISION-ID]` |

## Author contribution

| Contribution | Evidence | Information type and governed states | Public wording |
|---|---|---|---|
| `[Concept, architecture, instruction design, review, implementation, testing, or other]` | `[SOURCE-ID]` | `[FACT]` | `[Accurate wording]` |

AI-assisted or third-party contribution:

`[Describe tools and assistance without implying independent authorship of every line.]`

## Architecture and workflow

- Components: `[List]`
- Source hierarchy: `[Describe]`
- Human approval points: `[List]`
- Stop and escalation conditions: `[List]`
- Privacy controls: `[List]`
- Evaluation method: `[Describe or link]`

## Synthetic demonstration

| Element | Synthetic content | Label |
|---|---|---|
| Persona | `[Fictional profile]` | `SYNTHETIC` |
| Organization | `[Fictional organization]` | `SYNTHETIC` |
| Opportunity or task | `[Fictional scenario]` | `SYNTHETIC` |
| Expected output | `[Public-safe expected behavior]` | `SYNTHETIC` |

## Evaluation evidence

| Test | Method | Result | Limitation | Information type and governed states |
|---|---|---|---|---|
| `[Test]` | `[Protocol]` | `[Observed result]` | `[Limitation]` | `[Type: FACT; Evidence state; Document state: Draft]` |

## Privacy and publication review

- [ ] No private source file copied.
- [ ] No personal contact, identity, account, or credential data.
- [ ] No real application, recruiter, employer-confidential, or client data.
- [ ] Synthetic examples are clearly labeled.
- [ ] Contribution and limitation claims are evidence-backed.
- [ ] Secret scan and path scan completed on the exact version.
- [ ] License decision recorded separately.

## Approval record

| Gate | Decision | Exact version | Date | Governed state |
|---|---|---|---|---|
| Content approval | `[Approve / Revise / Reject]` | `[Version]` | `[YYYY-MM-DD]` | `[Document: Approved exact version; Execution: Content approved]` |
| Publication authorization | `[Authorize / Not authorized]` | `[Version and destination]` | `[YYYY-MM-DD]` | `[Decision: Approved within stated scope; Execution: Externally authorized]` |
