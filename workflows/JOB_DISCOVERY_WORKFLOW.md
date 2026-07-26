# Job Discovery Workflow

## Purpose

Find a bounded set of current opportunities and record enough evidence to support later assessment without treating search results as verified vacancies.

## Inputs

- Approved career goal and search constraints
- Approved professional profile
- [Job opportunity template](../templates/JOB_OPPORTUNITY_TEMPLATE.md)
- Authorized job sources
- Search date and freshness threshold

## Participating agents

- **Job Research Agent:** searches and captures source evidence.
- **Career Strategy Agent:** checks alignment with the approved search direction.
- **Evidence Checking Agent:** verifies source, date, and status.
- **Privacy Review Agent:** prevents collection of unnecessary third-party data.
- **Orchestrator Agent:** controls the candidate queue and deduplication.

## State model

`FACT`, `DECISION`, `ASSUMPTION`, and `RECOMMENDATION` are compact information-type tags only. Every opportunity record must separately carry the applicable **Evidence**, **Decision**, **Document**, and **Execution** states from [Source Governance](../SOURCE_GOVERNANCE.md). Queue inclusion is a decision `Approved within stated scope`; it is not content approval or external authorization.

## Procedure

1. Confirm target roles, geography, work model, languages, employment type, and freshness window.
2. Search only authorized sources and capture the retrieval date.
3. Open the original posting before recording an opportunity.
4. Record employer, role, location, work model, contract type, required qualifications, closing information, and source link only when directly supported.
5. Mark missing fields as unresolved; do not infer them from similar postings.
6. Detect duplicates using source identity, requisition details, and materially equivalent descriptions.
7. Exclude expired, inaccessible, clearly ineligible, misleading, or unverifiable listings.
8. Apply a lightweight relevance screen; do not perform the full fit assessment here.
9. Submit a manageable candidate batch with evidence quality and freshness notes.
10. Require human confirmation before promoting an item to the assessment queue.

## Human approval gate

Human approval is required to change search boundaries, include a sensitive or high-risk opportunity, contact any person, or promote a discovered item into active assessment. Discovery never authorizes an application.

## Outputs

- Evidence-backed opportunity records
- Duplicate and exclusion log
- Freshness and verification status
- Approved assessment queue

## Stop and escalation conditions

Stop when the original posting cannot be verified, access would require unauthorized credentials, the source appears deceptive, or the listing requests sensitive information prematurely. Escalate ambiguous eligibility, relocation, compensation, or legal-status questions without guessing.

## Related controls

Use the full [Opportunity Assessment Workflow](OPPORTUNITY_ASSESSMENT_WORKFLOW.md) next. Apply [Source Governance](../SOURCE_GOVERNANCE.md) and [Privacy and Data Governance](../PRIVACY_AND_DATA_GOVERNANCE.md) throughout.
