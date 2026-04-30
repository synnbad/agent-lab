# Workflow Creation Mode Prompts

## Purpose
Create new personal workflows when no existing workflow fits.

## When To Use
Use when a task spans multiple agents, lacks a repeatable process, or has no matching workflow in `workflows/`.

## Related Agents
- System Design Agent
- Web Development Agent
- UI Agent
- Backend Agent
- Writing Agent
- Grill-Me Sinbad

## Related Skills
- Requirements Discovery
- MVP Scope Control
- Architecture Review
- Technical Documentation
- Grill-Me Sinbad

## Related Workflows
- Workflow Creation Mode
- Project Triage Workflow
- Web App Build Workflow
- System Design Workflow

## Safety Notes
Workflow Creation Mode is personal-only and draft-first. Do not access job/workplace material. Do not write workflow files unless explicitly approved. New workflows start as Draft and become Active only after testing and review.

## Prompts

### Activate Workflow Creation Mode
- Best use case: Start when no workflow fits.
- Prompt:
```text
Activate Workflow Creation Mode for this personal idea: [idea].
Do not execute the project. Do not write files. Confirm it is personal-only, identify closest existing workflows, identify the workflow gap, and list approval needed before saving anything.
```
- Expected output: Workflow gap analysis.
- Safety/approval gates: No file writes.

### Map Closest Agents And Workflows
- Best use case: Route a new idea before drafting.
- Prompt:
```text
Map this personal task to the closest agents, skills, workflows, templates, guardrails, contracts, and threat models in agent-lab: [task].
Return: matches, gaps, conflicts, and recommended new workflow name if needed.
```
- Expected output: Source-of-truth map.
- Safety/approval gates: Read-only.

### Run Grill-Me Sinbad
- Best use case: Expose weak assumptions before creating a process.
- Prompt:
```text
Run Grill-Me Sinbad on this proposed workflow idea: [idea].
Be direct and precise. Identify weak assumptions, missing requirements, scope creep, risk, and what to cut. Do not be performatively harsh.
```
- Expected output: Critique with cuts and keeps.
- Safety/approval gates: Planning only.

### Draft A New Workflow
- Best use case: Produce a draft workflow artifact.
- Prompt:
```text
Draft a new personal workflow using templates/workflow-template.md.
Workflow name: [lowercase-kebab-case-name]
Status: Draft
Do not save files yet. Return the full draft workflow, required templates, required prompts, required evals, required guardrails, required contracts, and required threat models.
```
- Expected output: Full draft workflow text.
- Safety/approval gates: Save only after approval.

### Draft Supporting Artifacts
- Best use case: Plan the supporting system around a workflow.
- Prompt:
```text
For this draft workflow, propose supporting templates, prompts, evals, guardrails, contracts, and threat models.
Draft names and purposes only. Do not write files. Mark required vs optional. Include the first small test case.
Workflow: [paste workflow]
```
- Expected output: Artifact plan.
- Safety/approval gates: No writes.

### Save As Draft Only After Approval
- Best use case: Turn an approved draft into files.
- Prompt:
```text
Approved to save this draft workflow.
Save only the approved Draft workflow and approved supporting artifacts in the specified paths: [paths].
Do not promote to Active. Do not commit, push, deploy, or connect accounts. Report changed files and validation steps.
```
- Expected output: Draft files saved.
- Safety/approval gates: Exact approval phrase required.

### Promote Workflow To Active
- Best use case: Promote after test and review.
- Prompt:
```text
Review this Draft workflow for promotion to Active.
Evidence: [test results]
Do not edit files unless approved. Return: pass/fail, missing guardrails, missing evals, risk, required changes, and promotion recommendation.
```
- Expected output: Promotion decision.
- Safety/approval gates: Active promotion requires approval.
