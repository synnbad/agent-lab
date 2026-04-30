# Project Kickoff Prompts

## Purpose
Clarify rough personal project requests and route them to the right agent, workflow, and artifact.

## When To Use
Use before planning, implementation, or workflow creation.

## Related Agents
- System Design Agent
- Web Development Agent
- Client-to-MVP Website Agent
- Writing Agent
- Grill-Me Sinbad

## Related Skills
- Requirements Discovery
- MVP Scope Control
- Technical Documentation
- Grill-Me Sinbad

## Related Workflows
- Project Triage Workflow
- Workflow Creation Mode
- Web App Build Workflow
- System Design Workflow

## Safety Notes
Planning-first. Do not access job/workplace material. Do not read hidden files or `.env` files. Ask before writing files, changing config, or external actions.

## Prompts

### Triage A Rough Idea
- Best use case: Turn an idea into a scoped plan.
- Prompt:
```text
Use Project Triage Workflow for this personal idea: [idea].
Do not write files or take external actions. Return: goal, target user, problem, success criteria, MVP scope, deferred scope, risks, open questions, recommended agent, recommended workflow, and next prompt.
```
- Expected output: Kickoff plan.
- Safety/approval gates: Planning only.

### Requirements Discovery
- Best use case: Clarify missing decisions.
- Prompt:
```text
Use Requirements Discovery on these rough notes: [notes].
Return: clarified requirements, assumptions, contradictions, missing inputs, decision log, and questions I need to answer before implementation.
```
- Expected output: Requirements checklist.
- Safety/approval gates: No file writes.

### Choose Agent And Workflow
- Best use case: Route a task.
- Prompt:
```text
Select the best agent, skills, workflow, templates, and guardrails for this personal task: [task].
Return: recommendation, alternatives, why, first action, and approval gates.
```
- Expected output: Routing decision.
- Safety/approval gates: No execution.

### Define MVP And Later Scope
- Best use case: Reduce scope creep.
- Prompt:
```text
Use MVP Scope Control for this personal project: [project].
Return: launch MVP, later features, cut list, assumptions to test, fastest validation step, and risks.
```
- Expected output: MVP boundary.
- Safety/approval gates: No implementation.

### Create First Artifact Plan
- Best use case: Decide what to produce first.
- Prompt:
```text
For this personal project, recommend the first useful artifact: [project].
Choose from brief, spec, ADR, build prompt, checklist, workflow, template, or research plan. Return the artifact outline and why it comes first.
```
- Expected output: First artifact recommendation.
- Safety/approval gates: Draft only.

### Kickoff Review
- Best use case: Review readiness to start.
- Prompt:
```text
Review this kickoff plan: [plan].
Identify missing decisions, unclear users, risky assumptions, privacy concerns, approval gates, and whether the plan is ready for Codex implementation.
```
- Expected output: Readiness decision.
- Safety/approval gates: Stop before edits.
