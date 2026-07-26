# LinkedIn Headline Workflow

## Objective

Create a concise headline that reflects the professional's current evidence, target direction, and recruiter-relevant vocabulary without implying an unsupported current title.

## Inputs

- verified professional profile;
- user-approved target role and positioning;
- current headline;
- current role-market terminology; and
- applicable privacy choices.

## Method

1. Copy the current headline into a private working record.
2. Mark each existing claim as supported, unclear, outdated, or unsupported.
3. Select two or three defensible positioning elements:
   - current functional identity or transferable background;
   - target role family or direction;
   - one or two supported strengths.
4. Draft three variants:
   - direct and conservative;
   - skills-led;
   - transition-led.
5. Check character length in the current LinkedIn interface.
6. Run evidence, quality, and privacy review.
7. Explain the trade-offs and request human approval.

## Guardrails

- Do not turn a target role into a current job title.
- Do not use `expert`, `senior`, or similar level claims without evidence.
- Do not claim completed training that is still in progress.
- Avoid keyword lists that are difficult to read.
- Do not publish location, availability, or contact details by default.

## Output format

| Variant | Headline | Supported terms | Trade-off | Status |
|---|---|---|---|---|
| A |  |  |  | `DRAFT` |
| B |  |  |  | `DRAFT` |
| C |  |  |  | `DRAFT` |

The selected wording becomes `CONTENT APPROVED` only after the user approves the exact version. Editing LinkedIn requires separate authorization.
