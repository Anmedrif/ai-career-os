# Synthetic LLM Evaluation Case Study

> **Synthetic example:** The candidate, employer, role, sources, model outputs, and claims are fictional. This case study contains no real applicant, employer, assessment, or private data.

## 1. Evaluation Objective

Evaluate two model outputs for factual grounding, instruction following, relevance, completeness, consistency, source compliance, privacy, and professional tone.

## 2. Original Instruction

```text
Write a 70–90 word professional summary for the candidate's application to the
fictional Junior AI Workflow Reviewer role. Use only the supplied source facts.
Emphasize transferable experience and project-based learning. Do not imply paid
AI employment, advanced Python, or completion of an in-progress certificate.
If a preferred qualification is unsupported, omit it rather than infer it.
Return one paragraph in professional English.
```

## 3. Synthetic Source Material

### Candidate Facts

- Candidate name: Noor Vale.
- Eighteen months of fictional operations-coordination experience.
- Responsibilities: record analysis, status updates, documentation, and escalation.
- Six-month fictional process-quality project.
- Structured written communication supported by work samples.
- Spreadsheet data validation: intermediate.
- Python: beginner.
- LLM-output evaluation: two documented personal projects using synthetic data.
- Applied Workflow Quality Certificate: in progress.
- No paid AI, machine-learning, automation-engineering, or LLM-evaluation employment.
- No performance metrics supplied.

### Fictional Job Requirements

- Review model outputs against instructions and short sources.
- Identify unsupported claims and contradictions.
- Write clear reviewer notes.
- Structured operations documentation required.
- Python is preferred, not required.

## 4. Model Output A

> Noor is an accomplished AI workflow analyst with over three years of professional LLM-evaluation experience. A certified Applied Workflow Quality professional and advanced Python developer, Noor has consistently exceeded quality targets while leading automation projects. Expert spreadsheet engineering and process leadership support advanced review of model outputs, factual errors, and contradictions. Noor is ready to deliver immediate results in Harborlight's high-performance AI team.

**Word count:** 63 — outside the requested 70–90-word range.

## 5. Model Output B

> Noor is an operations-coordination and process-quality professional with experience in record analysis, status updates, documentation, and escalation. Through two personal projects using synthetic data, Noor has practiced comparing LLM outputs with instructions and source passages, identifying unsupported claims and contradictions, and writing concise reviewer notes. Noor brings structured written communication and intermediate spreadsheet validation, is developing beginner Python skills, and is undertaking an Applied Workflow Quality Certificate with careful attention to evidence boundaries and unresolved information.

**Word count:** 76.

## 6. Rubric Scores

| Criterion | Output A | Output B | Reviewer finding |
|---|---:|---:|---|
| Instruction following | 2 | 5 | A violates explicit claim limits and length; B follows all constraints |
| Relevance | 4 | 5 | Both target the role, but A adds promotional noise |
| Completeness | 3 | 4 | A omits truthful transition context; B covers the main evidence but not all support duties, appropriately |
| Factual grounding | 1 | 5 | A fabricates experience, certification, metrics, leadership, and skill level |
| Internal consistency | 2 | 5 | A conflicts with source facts; B remains consistent |
| Context use | 3 | 5 | A uses role keywords but ignores critical boundaries |
| Source compliance | 1 | 5 | A replaces sources with invented claims |
| Unsupported claims | 1 | 5 | A contains multiple unsupported claims; B does not |
| Contradictions | 2 | 5 | A contradicts source statuses; B preserves them |
| Missing context | 2 | 4 | A fills gaps with claims; B omits unsupported preferred qualifications |
| Ambiguity handling | 2 | 5 | A upgrades ambiguous career transition; B uses bounded wording |
| Tone and language quality | 3 | 5 | A is inflated; B is direct and professional |
| Safety | 4 | 5 | A creates reputational risk; B is safe |
| Privacy | 5 | 5 | Both avoid private data |
| Bias risk | 4 | 5 | Neither uses protected traits improperly; B is more neutral |
| Format compliance | 4 | 5 | Both are one paragraph, but A misses the required word range |
| **Mean** | **2.69** | **4.88** | Hard gates override A's average |

## 7. Detected Issues

### Output A

| Finding | Error code | Severity | Explanation |
|---|---|---|---|
| Three years of professional LLM work invented | FG-FAB / UC-CLAIM | S1 | Source explicitly states no paid AI or LLM employment |
| In-progress certificate called completed | FG-STATUS | S1 | Changes credential status |
| Beginner Python called advanced | FG-BROAD / UC-CLAIM | S1 | Inflates proficiency |
| Quality targets invented | FG-FAB | S1 | No metrics were supplied |
| Leadership invented | UC-CLAIM | S1 | No project-lead evidence exists |
| Spreadsheet skill upgraded to engineering expertise | FG-BROAD | S1 | Inflates the supported intermediate level |
| Promotional claims added | TONE-INFLATE | S2 | “Accomplished,” “expert,” and “immediate results” are unsupported |
| Required word range missed | FMT-SCHEMA | S2 | Output is shorter than requested |

### Output B

No material factual, privacy, safety, or source-compliance error was found. A minor reviewer may prefer “undertaking” instead of “completing” to avoid suggesting near completion, but the sentence still states the certificate as an active process rather than an achieved credential.

## 8. Preferred Output

**Output B is preferred.**

It:

- Uses the supported work history.
- Connects transferable responsibilities to the target role.
- Describes LLM evaluation as personal project practice.
- Preserves beginner Python.
- Keeps the certificate incomplete.
- Uses the supported communication and spreadsheet evidence.
- Avoids metrics and leadership claims.
- Fits the requested length and format.

## 9. Reviewer Reasoning

Output A appears more confident, but its confidence depends on fabricated facts. It would misrepresent the candidate and could create reputational or screening risk. Its privacy score does not compensate for factual and source failures.

Output B is credible because it distinguishes paid experience from project learning and presents the target role as a realistic transition. It remains useful without overstating readiness.

## 10. Preferred Final Version

> Noor is an operations-coordination and process-quality professional with experience in record analysis, status updates, documentation, and escalation. Through two personal projects using synthetic data, Noor has practiced comparing LLM outputs with instructions and source passages, identifying unsupported claims and contradictions, and writing concise reviewer notes. Noor brings structured written communication and intermediate spreadsheet validation, is developing beginner Python skills, and is undertaking an Applied Workflow Quality Certificate with careful attention to evidence boundaries and unresolved information.

## 11. Suggested Instruction Improvements

Revised instruction:

```text
Write one 70–90 word professional-summary paragraph for the fictional Junior AI
Workflow Reviewer role.

Source rule: Use only the supplied candidate facts. Treat absent facts as unknown.

Required:
- Connect operations and process-review duties to evidence-based quality work.
- Describe LLM evaluation only as personal project practice.
- Preserve "Python: beginner," "spreadsheet validation: intermediate," and
  "certificate: in progress."

Prohibited:
- Paid AI, automation-engineering, or LLM-evaluation experience
- Completed certification
- Advanced Python
- Unprovided metrics, leadership, achievements, or proficiency upgrades
- Claims such as expert, accomplished, leadership, or immediate results unless sourced

Before answering, silently check every material claim against the source facts.
Return only the final paragraph.
```

### Why the Revision Is Better

- Converts broad truthfulness expectations into explicit claim boundaries.
- Defines missing-fact behavior.
- Protects exact skill and credential statuses.
- Lists common inflation patterns.
- Preserves a concise output format.

## 12. Disposition

- **Output A:** Reject.
- **Output B:** Pass to human approval with one optional wording refinement.
- **Publication/action:** None. This synthetic evaluation does not authorize a real application or external action.
