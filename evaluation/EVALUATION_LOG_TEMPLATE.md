# Evaluation Log Template

> Copy this template for each evaluation. Public logs must use synthetic or fully sanitized data.

## 1. Evaluation Metadata

- **Evaluation ID:**
- **Date:**
- **Evaluator:**
- **Reviewer role:**
- **Model/version:**
- **Prompt/version:**
- **Output type:**
- **Intended audience/use:**
- **Risk level:** Low / Medium / High
- **Related workflow:**

## 2. Original Instruction

```text
[Insert the exact instruction.]
```

## 3. Required Output and Constraints

- Required sections:
- Required format:
- Required language:
- Prohibited content/actions:
- Human approval gate:
- Stop conditions:

## 4. Source Package

| Priority | Source | Authority and scope | Currentness | Sensitivity | Notes |
|---:|---|---|---|---|---|
| 1 |  |  |  |  |  |

### Known Conflicts or Missing Sources

-

## 5. Output Under Review

```text
[Insert the exact model output or a stable artifact reference.]
```

## 6. Claim Ledger

| Claim ID | Claim | Source | Status | Qualification | Decision |
|---|---|---|---|---|---|
| C-001 |  |  | Verified / user-confirmed / derived / unresolved |  | Keep / revise / omit / escalate |

## 7. Rubric Scorecard

| Criterion | Score | Rationale and evidence |
|---|---:|---|
| Instruction following |  |  |
| Relevance |  |  |
| Completeness |  |  |
| Factual grounding |  |  |
| Internal consistency |  |  |
| Context use |  |  |
| Source compliance |  |  |
| Unsupported claims |  |  |
| Contradictions |  |  |
| Missing context |  |  |
| Ambiguity handling |  |  |
| Tone and language quality |  |  |
| Safety |  |  |
| Privacy |  |  |
| Bias risk |  |  |
| Format compliance |  |  |

- **Mean score:**
- **Any `N/A` explanations:**

## 8. Findings

| Finding ID | Error code | Severity | Output location | Impact | Required correction |
|---|---|---|---|---|---|
| F-001 |  |  |  |  |  |

## 9. Gate Results

- **Factual-grounding gate:** Pass / Fail
- **Source-compliance gate:** Pass / Fail
- **Privacy gate:** Pass / Fail
- **Safety gate:** Pass / Fail
- **Authorization gate:** Pass / Fail
- **Format gate:** Pass / Fail

## 10. Preferred Correction

```text
[Insert corrected wording or exact revision instructions.]
```

## 11. Disposition

Choose one:

- [ ] Pass to human approval
- [ ] Pass with minor edits
- [ ] Revise and re-evaluate
- [ ] Reject
- [ ] Escalate — source conflict
- [ ] Escalate — privacy or safety

**Reason:**

## 12. Human Review

- **Approver:**
- **Decision:** Approved / Approved with changes / Rejected / Deferred
- **Exact version or hash:**
- **Approved scope:**
- **Excluded scope:**
- **Date:**
- **Required follow-up:**

## 13. Regression Record

- Prompt or workflow changed:
- New version:
- Failed cases re-run:
- Previously passing cases re-run:
- Result:
- Remaining limitations:
