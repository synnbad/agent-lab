# OpenClaw Planner Prompts

## Purpose
Use OpenClaw as a read-only planner for personal projects while preserving strict safety boundaries.

## When To Use
Use these prompts for sandbox validation, project triage, agent/workflow selection, portfolio planning, and sanitized reports.

## Related Agents
- Active OpenClaw main agent
- Client-to-MVP Website Agent
- Web Development Agent
- UI Agent
- Accessibility Agent
- Writing Agent
- Grill-Me Sinbad

## Related Skills
- Requirements Discovery
- MVP Scope Control
- Code Review
- Technical Documentation
- Grill-Me Sinbad

## Related Workflows
- Project Triage Workflow
- Web App Build Workflow
- Accessibility Audit Workflow
- Client Website Delivery Workflow
- Workflow Creation Mode

## Safety Notes
Keep OpenClaw read-only unless explicitly approved. Do not access job/workplace material. Do not read hidden files. Do not read `.env` files. Do not print, store, log, or commit secrets. Do not write, commit, push, deploy, send messages, browse, connect accounts, or change config unless explicitly approved. Use generic "blocked workplace-related items" wording only.

## Prompts

### Read-Only Project Inspection
- Best use case: Inspect a personal repo before planning.
- Prompt:
```text
Use OpenClaw read-only planner mode for this personal project: [repo path].
Inspect only non-hidden, non-secret project files needed to understand structure, stack, scripts, and docs.
Do not read hidden files or `.env` files. Do not access job/workplace material. Do not write files, commit, push, deploy, browse, send messages, connect accounts, or change config.
Return: stack, structure, scripts, main content files, risks, missing docs, recommended next safe step.
```
- Expected output: Concise repo inspection with safe next step.
- Safety/approval gates: Stop before edits or external actions.

### Agent Selection
- Best use case: Decide which repo agent should handle a task.
- Prompt:
```text
Use agent-lab as source of truth. For this personal task, recommend the best agent or agent combination: [task].
Do not execute the task. Do not inspect hidden files or `.env` files. Do not access job/workplace material.
Return: primary agent, supporting agents, why, risks, workflow match, approval needed.
```
- Expected output: Agent routing recommendation.
- Safety/approval gates: Planning only.

### Workflow Selection
- Best use case: Pick an existing workflow before work begins.
- Prompt:
```text
Use read-only planner mode. Match this personal task to the closest workflow: [task].
Compare Project Triage, Web App Build, Accessibility Audit, Client Website Delivery, Data Analysis, Backend API, System Design, and Workflow Creation Mode.
Do not execute. Return: chosen workflow, alternatives rejected, first three steps, required artifacts, approval gates.
```
- Expected output: Workflow routing decision.
- Safety/approval gates: No execution.

### OpenClaw Safety Check
- Best use case: Verify current posture before using OpenClaw.
- Prompt:
```text
Run a read-only safety check using the latest known sandbox facts. Do not change config.
Report: runtime, mode, scope, workspace access, denied tools, enabled channels, write status, external action status, remaining risks, pass/fail.
Use generic "blocked workplace-related items" wording only.
```
- Expected output: Safety posture report.
- Safety/approval gates: No config changes.

### Portfolio Planning
- Best use case: Plan the personal portfolio refresh without edits.
- Prompt:
```text
Use read-only planner mode for my personal portfolio website refresh.
Repo: /Users/sinbadadjuik/Projects/personal-projects/portfolio
Do not write files, commit, push, deploy, browse, send messages, connect accounts, or access job/workplace material.
Inspect only non-hidden, non-secret files. Return: current site summary, positioning, homepage plan, project card improvements, content gaps, UI/UX improvements, accessibility/SEO/performance improvements, files likely to change later, approval gates.
```
- Expected output: Concrete portfolio MVP plan.
- Safety/approval gates: Stop before implementation.

### No-Write Project Triage
- Best use case: Turn a rough idea into a scoped plan.
- Prompt:
```text
Use Project Triage Workflow in read-only mode for this personal idea: [idea].
Do not write files or run external actions. Return: clarified goal, assumptions, questions, MVP scope, deferred scope, risks, recommended agent, recommended workflow, next prompt.
```
- Expected output: MVP-ready triage.
- Safety/approval gates: Ask before file writes.

### Report Sanitization
- Best use case: Clean a report before sharing.
- Prompt:
```text
Sanitize this report for personal-only use.
Replace any job/workplace-specific identifiers or raw names with "blocked workplace-related items".
Do not add details. Do not infer private facts. Return: sanitized report, removed categories, remaining risks.
Report: [paste report]
```
- Expected output: Sanitized report.
- Safety/approval gates: No raw workplace details.
