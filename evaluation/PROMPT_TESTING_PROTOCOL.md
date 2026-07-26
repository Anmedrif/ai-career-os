# Prompt Testing Protocol

## Purpose

This protocol evaluates whether a prompt produces accurate, useful, consistent, privacy-safe outputs across normal, incomplete, conflicting, and adversarial inputs.

## 1. Define the Test Objective

Record:

- Prompt name and version
- Intended task
- Target user and output
- Required sources
- Required format
- Prohibited behavior
- Human approval point
- Known risks
- Success criteria

Example hypothesis:

> When a source omits an employment date, the prompt should make the model request confirmation or mark the date unresolved rather than infer a typical duration.

## 2. Create a Test Set

Use synthetic fixtures only in public tests. Include at least:

1. **Happy path:** Complete, consistent sources.
2. **Missing fact:** A required fact is absent.
3. **Source conflict:** Two sources disagree.
4. **Stale source:** An older source conflicts with a newer decision.
5. **Privacy trap:** Input contains unnecessary personal data.
6. **Unsupported achievement:** The user requests stronger wording than evidence supports.
7. **Ambiguous instruction:** Two reasonable interpretations exist.
8. **Format stress:** Strict schema, table, or length constraint.
9. **Prompt injection:** Source text tries to override system or workflow rules.
10. **Multilingual case:** Instructions and source material use different languages.

Each fixture should define an expected behavior, not only an expected sentence.

## 3. Control Variables

When the platform allows:

- Keep model and system instructions constant while comparing prompt variants.
- Record temperature, seed, tool availability, and date.
- Run each high-variance case multiple times.
- Change one prompt element at a time.
- Preserve exact inputs and outputs.

If a parameter is unavailable, record it as unknown.

## 4. Execute the Test

For every case:

1. Supply the exact instruction and source package.
2. Capture the complete output.
3. Run the factual-grounding checklist.
4. Score the sixteen evaluation criteria.
5. Assign error codes and severities.
6. Apply privacy, safety, and approval gates.
7. Record the disposition.

Do not repair the output before evaluation. A corrected version is a separate run.

## 5. Compare Prompt Variants

Use a result table:

| Case | Variant | Mean score | Critical failures | Major failures | Format pass | Disposition |
|---|---|---:|---:|---:|---|---|
| T-001 | A |  |  |  |  |  |

Also compare:

- Unsupported-claim rate
- Conflict-detection rate
- Required-field completion
- Privacy-gate pass rate
- Correct escalation rate
- Reviewer correction effort
- Output stability across repeated runs

## 6. Acceptance Criteria

A prompt is ready for bounded use when:

- No critical privacy, safety, authorization, or fabricated-claim failure appears in the required test set.
- All material source conflicts are detected or safely escalated.
- Missing facts are not silently filled.
- Required output structure passes consistently.
- The prompt preserves human approval gates.
- Major-error frequency is within the documented threshold for the intended risk level.
- Remaining limitations are recorded.

For high-impact career outputs, one critical failure is sufficient to block release.

## 7. Improve the Prompt

Prefer targeted changes:

- Clarify source hierarchy.
- Add a missing-fact rule.
- Add prohibited claims.
- Define status labels.
- Specify the output schema.
- Add a human approval gate.
- Add a privacy-minimization rule.
- Add a conflict-handling example.

Avoid patching one example with overly specific wording that reduces general usefulness.

## 8. Regression Test

After revision:

- Re-run the failed case.
- Re-run all critical fixtures.
- Re-run at least one previously passing case.
- Confirm that the fix did not create new omissions, verbosity, or format failures.
- Assign a new prompt version.

## Test Record Template

```markdown
## Prompt Test Run

- Prompt/version:
- Model/version:
- Date:
- Objective:
- Fixture:
- Expected behavior:
- Actual output:
- Scores:
- Error codes:
- Privacy/safety gate:
- Disposition:
- Proposed prompt change:
- Regression cases:
- Human reviewer:
```

## Stop Conditions

Stop testing and escalate when:

- Real private data appears in a public test.
- A required authoritative source is unavailable.
- A prompt repeatedly bypasses a human approval boundary.
- A model or tool changes during a comparison without a controlled rerun.
- The test objective expands into a materially different task.
