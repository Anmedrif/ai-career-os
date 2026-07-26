# Human in the Loop

## Purpose

Human-in-the-Loop control keeps consequential career decisions, professional claims, privacy choices, and external actions under human authority. Agents may prepare options and evidence, but the human decides what is true enough to use, what risk to accept, and whether an external step should occur.

This is a reference control model, not evidence of automated enforcement.

## Human Authority

The human retains final authority over:

- material professional facts and achievements;
- career goals, priorities, and accepted risks;
- exact artifact content;
- public disclosure of personal information;
- applications, communications, uploads, scheduling, and publication;
- offers, contracts, salary, legal eligibility, relocation, and financial commitments;
- material profile changes;
- use of employer or client information; and
- consequential automation or account access.

Source ownership and agent responsibility do not replace human approval.

## Approval Gates

| Gate | Human decision required | Evidence expected |
|---|---|---|
| Professional profile | Confirm or reject material facts and qualifications | Claim list, source status, limitations, unresolved conflicts |
| Career strategy | Approve goals, priorities, constraints, and material risk | Options, trade-offs, dependencies, open questions |
| Opportunity pursuit | Decide whether to pursue or pause | Current posting, fit, gaps, risk, eligibility limits |
| Exact artifact content | Approve the exact CV, answer, message, or profile version | Version identifier, factual checks, unresolved issues |
| Application or communication | Authorize the specific external action | Destination, recipient, exact artifact, permitted data |
| Interview preparation | Approve final answer set and claims | Question set, source mapping, uncertainty notes |
| LinkedIn change | Approve exact section text and direct account action separately | Before/after text, factual review, privacy review |
| Portfolio or repository publication | Approve the exact release | Release tree, privacy report, secret scan, limitations |
| Metrics or achievements | Approve use and qualification | Evidence strength, source date, wording limits |
| Employer or client information | Approve disclosure when lawful and appropriate | Public status, confidentiality check, minimum necessity |
| Automation or account access | Approve bounded operation | Platform, permissions, duration, stop rules, logging |

## Approval Is Exact and Scoped

An approval record should identify:

```text
Approver:
Exact version:
Decision:
Permitted purpose:
Destination or recipient:
Permitted data:
Constraints:
Validity period or expiry:
Stopping condition:
Date:
```

Approval of one version, destination, or action does not authorize another.

## Required State Separation

The system preserves these separate states:

1. source facts exist;
2. a draft is prepared;
3. review is complete;
4. the human approves the exact content;
5. the human authorizes a specific external action;
6. the action is attempted;
7. evidence shows whether it completed; and
8. an original outcome is recorded.

No state proves the next state.

## Human Review Workflow

### 1. Review the Decision Packet

The human receives:

- purpose and intended use;
- exact content or decision;
- sources and source status;
- material claims;
- conflicts and unknowns;
- reviewer findings;
- privacy classification;
- alternatives and trade-offs; and
- the precise approval requested.

### 2. Choose a Disposition

The human may:

- approve within a stated scope;
- request revision;
- reject;
- defer pending evidence;
- approve with explicit qualification; or
- withdraw a prior approval.

### 3. Record the Decision

The decision is recorded in the source responsible for that subject. A global approval label must not silently replace source-specific status.

### 4. Integrate and Recheck

Affected sources and derivatives are updated or marked `approved decision pending integration`. Consequential use pauses until required corrections and reviews are complete.

## When Automation Stops

Automated or AI-assisted work must stop when:

- required information is missing or contradictory;
- the output would strengthen an unsupported claim;
- a human value judgment or material risk decision is needed;
- legal, contract, salary, eligibility, relocation, privacy, or financial interpretation is consequential;
- the exact version or intended destination is unclear;
- personal or confidential information may be exposed;
- a requested action changes an external account or communicates with another party;
- a reviewer reports a hard failure; or
- the authorized scope, duration, or stop condition has been reached.

## Escalation Packet

An escalation should be concise:

```text
Decision needed:
Why work cannot continue safely:
Relevant authoritative sources:
Known facts:
Conflicting or missing information:
Options:
Material trade-offs:
Recommended next step:
Work that can continue unaffected:
```

Agents should ask the smallest question that resolves the material issue.

## Hard-Failure Conditions

The output cannot progress to human approval if it:

- invents or materially upgrades a professional claim;
- hides a material contradiction;
- exposes a secret or prohibited personal data;
- relies on stale information without qualification;
- misrepresents a structural or automated check as human review;
- claims an external action occurred without evidence;
- uses an unapproved exact version; or
- bypasses a required privacy or evidence review.

## Manual and Automated Review

Automated checks can validate structure, required text, metadata, links, prohibited terms, and consistency rules. They do not prove:

- factual truth;
- visual quality in every rendering environment;
- human comprehension;
- acceptability of a professional claim;
- legal sufficiency; or
- approval.

When visual presentation matters, the rendered artifact requires human visual review. A structural pass must not be described as a completed visual review.

## Public-Release Gate

Before a repository, profile, post, or portfolio item is published, the human should receive:

- the exact release version;
- a summary of source material used;
- the public-safe professional claims;
- facts still requiring confirmation;
- excluded content categories;
- secret, local-path, and privacy-check results;
- known limitations;
- the proposed destination and visibility; and
- a precise publication-approval request.

Creating a local draft does not authorize publication.

## Auditability

Human decisions should remain reconstructable from:

- the exact reviewed version;
- decision date and scope;
- source and reviewer status;
- any limitations;
- external-action authorization where applicable; and
- completion or outcome evidence if an action later occurs.

Auditability should remain proportionate to risk and should not require storing unnecessary personal data.

## Related Documents

- [System Architecture](SYSTEM_ARCHITECTURE.md)
- [Agent Roles](AGENT_ROLES.md)
- [Source Governance](SOURCE_GOVERNANCE.md)
- [Evaluation Framework](EVALUATION_FRAMEWORK.md)
- [Privacy and Data Governance](PRIVACY_AND_DATA_GOVERNANCE.md)
