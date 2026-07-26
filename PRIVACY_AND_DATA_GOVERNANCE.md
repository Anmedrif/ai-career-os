# Privacy and Data Governance

Privacy is an architectural requirement, not a final editing step. The system minimizes data at collection, limits who or what may use it, separates private sources from public outputs, and requires review before external use.

## Data classes

| Class | Examples | Default treatment |
|---|---|---|
| Public portfolio content | Approved project descriptions and synthetic examples | May be versioned after approval |
| Professional facts | Employment, education, languages, skills | Keep private until each public use is approved |
| Sensitive personal data | Address, identity documents, birth date, immigration details | Do not place in this repository |
| Operational career data | Applications, recruiter messages, interviews, offers, salary | Private workspace only |
| Employer or client data | Internal tools, policies, cases, screenshots, documents | Exclude unless independently public and authorized |
| Secrets | Passwords, tokens, keys, cookies, recovery codes | Never store |
| Third-party personal data | Recruiter or contact details | Exclude or replace with synthetic data |

## Public/private boundary

This repository contains reusable logic and fictional examples. A real deployment should keep:

- the verified professional profile;
- evidence files;
- job records;
- applications and communications;
- private review notes; and
- account or environment information

in a separate private location with appropriate access controls.

Relative links in this repository must never point to the private workspace.

## Minimum-necessary rule

Before collecting or copying a field, ask:

1. Is it necessary for the current approved purpose?
2. Is a reference sufficient instead of a copy?
3. Can a category or range replace an exact value?
4. Does the intended reviewer need this field?
5. What is the deletion or reassessment trigger?

If the answer is unclear, omit the field and escalate.

## Synthetic-data standard

Public examples must:

- state that they are fictional;
- use fictional people, companies, roles, and identifiers;
- avoid combining facts that could reasonably identify a real person;
- contain no copied job text, conversations, or screenshots; and
- remain useful without resembling a private case.

## Publication review

The Privacy Review Agent checks:

- direct identifiers and contact details;
- quasi-identifiers that become identifying in combination;
- private paths, usernames, machine names, and private URLs;
- credentials and secret-like values;
- employer or client names and confidential details;
- real application or assessment content;
- third-party personal data;
- image metadata and screenshots; and
- whether every personal claim has publication approval.

A clean pattern scan is supporting evidence, not a guarantee. Manual contextual review remains required.

## Retention and correction

- Do not keep private data “just in case.”
- Keep only the version history needed for accountability and recovery.
- Remove data from public drafts when its approval expires or its purpose ends.
- Correct the authoritative private source first; then identify and review affected public derivatives.
- Record material supersession without leaving the old claim active.

## Incident response

If sensitive information is found:

1. stop publication or distribution;
2. identify the exact affected files and versions;
3. remove the exposure from the working tree and history using an approved recovery process;
4. rotate any exposed secret through its issuing service;
5. review derived copies and external destinations;
6. document the incident without repeating the sensitive value; and
7. require a new privacy approval before release.

For repository controls, see [Security](SECURITY.md). For decision gates, see [Human in the Loop](HUMAN_IN_THE_LOOP.md).
