# Synthetic Agent Handoff

> **Synthetic example:** All identities, organizations, opportunity IDs, and facts are fictional. The handoff demonstrates structure only.

## Scenario

The Opportunity Assessment Agent has completed a preliminary review of Maya Elian against a fictional AI Workflow Quality Associate role. It is handing the case to the CV Tailoring Agent.

## Human-Readable Handoff

- **Handoff ID:** SYN-HO-028
- **From:** Opportunity Assessment Agent
- **To:** CV Tailoring Agent
- **Candidate source:** `SYNTHETIC_PROFESSIONAL_PROFILE.md`
- **Opportunity source:** `SYNTHETIC_JOB_OPPORTUNITY.md`
- **Assessment source:** `SYNTHETIC_OPPORTUNITY_ASSESSMENT.md`
- **Authorized action:** Draft a tailored synthetic CV section for human review
- **Prohibited actions:** Submit, upload, contact the company, invent facts, or mark content approved

### Supported Positioning

Use the candidate's:

- Operations-coordination experience
- Process-quality review experience
- Structured written communication
- Guideline application
- Workflow documentation and escalation
- Project-based LLM-output review

### Required Qualifications

- LLM evaluation is project practice, not paid employment.
- Python is beginner-level.
- The learning program is in progress.
- JSON knowledge is unresolved.
- Hybrid availability is unresolved.

### Required Output

1. One tailored professional summary
2. Three role-relevant experience bullets
3. One project entry
4. Selected skills
5. A list of excluded or unresolved claims

### Stop Conditions

Stop and return to the Orchestrator if:

- The draft requires hybrid availability.
- A new metric or achievement is requested.
- A source conflict appears.
- The user requests external submission.

## Machine-Readable Handoff

```json
{
  "handoff_id": "SYN-HO-028",
  "synthetic": true,
  "from_agent": "opportunity_assessment_agent",
  "to_agent": "cv_tailoring_agent",
  "goal": "Draft a tailored synthetic CV section for human review",
  "sources": [
    {
      "id": "SYN-PRO-001",
      "path": "../examples/SYNTHETIC_PROFESSIONAL_PROFILE.md",
      "authority": "professional_facts"
    },
    {
      "id": "SYN-OPP-014",
      "path": "../examples/SYNTHETIC_JOB_OPPORTUNITY.md",
      "authority": "opportunity_requirements"
    },
    {
      "id": "SYN-ASMT-014",
      "path": "../examples/SYNTHETIC_OPPORTUNITY_ASSESSMENT.md",
      "authority": "assessment_recommendation"
    }
  ],
  "supported_claims": [
    "process-quality review",
    "operations coordination",
    "guideline application",
    "workflow documentation",
    "issue escalation",
    "project-based LLM-output review"
  ],
  "constraints": [
    "Do not claim paid AI employment",
    "Keep Python at beginner level",
    "Keep the learning program in progress",
    "Do not infer JSON knowledge",
    "Do not infer hybrid availability"
  ],
  "approval_state": "drafting_authorized_human_approval_pending",
  "external_action_authorized": false
}
```

## Receiving-Agent Acceptance Check

- [ ] All source paths are available.
- [ ] Source authority is understood.
- [ ] Required qualifications are preserved.
- [ ] Output format is clear.
- [ ] Stop conditions are clear.
- [ ] No external action is authorized.

If any check fails, the receiving agent returns a focused clarification request instead of continuing.
