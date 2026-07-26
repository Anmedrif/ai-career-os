# Project Overview

## Purpose

AI Career OS is a documentation-first reference design for career management with AI assistance. It shows how a professional can organize facts, goals, opportunities, materials, decisions, and learning without allowing generated text to become evidence or authorization.

The repository serves two audiences:

- professionals who want a reusable, privacy-aware career operating system; and
- reviewers who want to see practical work in multi-agent design, prompt and instruction design, source governance, Human-in-the-Loop controls, and LLM output evaluation.

## Problem

Career work often spans CV files, platform profiles, job posts, interview notes, learning plans, and AI conversations. Common failure modes include:

- conflicting dates or titles across materials;
- tailoring that adds unsupported experience;
- outdated job evidence;
- unclear ownership of facts and decisions;
- approval of wording being mistaken for permission to publish or submit;
- personal or employer-confidential data leaking into examples; and
- model outputs being accepted because they sound confident.

## Proposed solution

The design combines:

1. one authoritative professional profile;
2. workflow-specific sources with narrow ownership;
3. a routing-oriented Orchestrator;
4. specialist agents that draft or analyze within scope;
5. independent quality, evidence, and privacy review;
6. explicit state labels and traceability; and
7. human approval before material decisions and external actions.

## Design principles

- **Authority is scoped.** A source owns only the information assigned to it.
- **Generated text is a draft.** Fluency does not establish truth, approval, or completion.
- **Conflicts stay visible.** Material disagreements are escalated, not silently blended.
- **Approval is specific.** Content approval, publication approval, action authorization, completion, and outcome are different states.
- **Privacy is structural.** Public examples are synthetic and private sources remain outside the repository.
- **Automation is subordinate.** It must be reviewable, stoppable, and limited to an approved purpose.
- **Complexity must earn its place.** Documentation comes before tools, databases, or automation.

## Scope

The system covers the full career lifecycle from verified profile creation through quarterly review. It includes reusable agent contracts, workflow definitions, templates, evaluation rubrics, LinkedIn workflows, and synthetic demonstrations.

## Non-goals

This version is not:

- a hosted service or autonomous agent runtime;
- an applicant-tracking platform;
- a job-board scraper;
- a hiring or candidate-ranking model;
- a legal, immigration, tax, or financial adviser;
- a collection of real applications or employer records; or
- evidence of production-scale AI engineering.

## How to use the repository

1. Read [Source Governance](SOURCE_GOVERNANCE.md).
2. Create a private profile with [the profile template](templates/PROFESSIONAL_PROFILE_TEMPLATE.md).
3. Select the relevant process from the [Workflow Index](WORKFLOWS.md).
4. Use the matching agent contracts as review prompts.
5. Evaluate drafts with the [LLM rubric](evaluation/LLM_OUTPUT_EVALUATION_RUBRIC.md).
6. Apply the approval gates in [Human in the Loop](HUMAN_IN_THE_LOOP.md).
7. Keep real personal data in a private workspace, never in a public fork.

## Definition of a successful output

A successful output is useful for its stated purpose, grounded in current authorized sources, clear about uncertainty, free of unnecessary sensitive data, reviewed against the applicable rubric, and approved by the right human for the exact next action.

For architecture details, continue to [System Architecture](SYSTEM_ARCHITECTURE.md).
