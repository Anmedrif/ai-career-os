# Quality Control Checklist

Use this checklist before an output moves to human approval. Mark each item `Pass`, `Fail`, or `N/A`, and explain every failure or `N/A`.

## 1. Task Contract

- [ ] The original instruction is recorded.
- [ ] The intended audience and use are clear.
- [ ] Required sections, format, and language are present.
- [ ] Prohibited actions and stop conditions were respected.
- [ ] No external action is described as completed unless separately verified.
- [ ] The output stayed within the authorized file, system, and workflow scope.

## 2. Source Control

- [ ] Sources are listed in priority order.
- [ ] The current authoritative source was used where available.
- [ ] Historical, derivative, or example material did not override authority.
- [ ] Source scope and currentness were checked.
- [ ] Conflicting sources are visible and not silently blended.
- [ ] Missing authoritative sources are recorded as limitations.

## 3. Factual Quality

- [ ] Every material factual claim has a source or an explicit uncertainty label.
- [ ] Dates, titles, names, education, credentials, skills, tools, and metrics retain exact supported meaning.
- [ ] User-confirmed information is not called independently verified.
- [ ] Drafts, approvals, actions, completions, and outcomes are distinguished.
- [ ] No achievement, metric, proficiency level, or responsibility was inflated.
- [ ] Derived statements can be reconstructed from their source facts.

## 4. Content Quality

- [ ] The response answers the actual question.
- [ ] Required information is complete.
- [ ] Repetition and irrelevant content are removed.
- [ ] Conclusions follow from the evidence.
- [ ] Recommendations are labeled as recommendations.
- [ ] Limitations and next decisions are clear.
- [ ] Terminology is consistent across headings, tables, and prose.

## 5. Language and Tone

- [ ] Language matches the requested audience and locale.
- [ ] Sentences are direct, natural, and readable.
- [ ] Marketing clichés and inflated claims are absent.
- [ ] The tone is professional without hiding uncertainty.
- [ ] Grammar, spelling, punctuation, and capitalization are consistent.
- [ ] Accessibility is considered: clear headings, descriptive links, and understandable labels.

## 6. Privacy and Confidentiality

- [ ] Only minimum-necessary information is included.
- [ ] No phone number, private email, exact address, private URL, credential, token, or secret appears.
- [ ] No identification, immigration, health, financial, salary, or account detail appears without explicit need and authorization.
- [ ] No private recruiter, applicant, client, or third-party data appears.
- [ ] No employer-confidential policy, tool, process, case, or assessment content appears.
- [ ] Public examples use clearly fictional people, companies, and opportunities.
- [ ] Local paths, usernames, machine names, and private project identifiers are absent.

## 7. Safety, Fairness, and Human Control

- [ ] High-impact judgments use job-relevant evidence.
- [ ] Protected traits and irrelevant proxies do not influence recommendations.
- [ ] The output does not claim legal, financial, medical, or security certainty without appropriate authority.
- [ ] Human approval gates are visible.
- [ ] The system stops where human judgment or new authority is required.
- [ ] Rejected or escalated outputs explain the reason and safe next step.

## 8. Format and Technical Checks

- [ ] Required filenames and headings are correct.
- [ ] Markdown links resolve relative to the repository.
- [ ] Tables render legibly.
- [ ] Mermaid or structured data syntax is valid where used.
- [ ] Placeholders are explicit and cannot be mistaken for confirmed facts.
- [ ] No secret-like sample values or real identifiers were used.

## 9. Release Decision

- [ ] All critical and major findings are resolved.
- [ ] Any remaining minor findings are recorded.
- [ ] The exact output version is identified.
- [ ] The evaluation log is complete.
- [ ] The human approver is identified.
- [ ] Publication, sending, uploading, or account modification has **not** occurred without explicit authorization.

## Result

- **Disposition:** `PASS TO HUMAN APPROVAL / PASS WITH MINOR EDITS / REVISE / REJECT / ESCALATE`
- **Blocking findings:**
- **Required corrections:**
- **Reviewer:**
- **Date:**
