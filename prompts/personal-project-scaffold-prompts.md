# Personal Project Scaffold Prompts

## Purpose
Plan safe scaffolds for new personal projects before creating files.

## When To Use
Use when starting a personal app, website, AI tool, documentation set, or project repo.

## Related Agents
- System Design Agent
- Web Development Agent
- UI Agent
- Backend Agent
- Writing Agent

## Related Skills
- Requirements Discovery
- MVP Scope Control
- Technical Documentation
- Architecture Review

## Related Workflows
- Project Triage Workflow
- Web App Build Workflow
- System Design Workflow
- Workflow Creation Mode

## Safety Notes
All scaffolding must ask before writing files. Do not read hidden files or `.env` files. Do not commit, push, deploy, or connect accounts without approval.

## Prompts

### New Personal Project Scaffold
- Best use case: Start any personal project.
- Prompt:
```text
Plan a scaffold for this personal project: [idea].
Return: folder structure, README outline, initial docs, MVP tasks, risks, and exact files to create after approval.
```
- Expected output: Scaffold plan.
- Safety/approval gates: Ask before writing files.

### Personal Web App Scaffold
- Best use case: Start a web app.
- Prompt:
```text
Plan a personal web app scaffold for: [idea].
Return: stack recommendation, routes, components, data model, docs, tests, scripts, and files to create.
```
- Expected output: Web scaffold plan.
- Safety/approval gates: No package install without approval.

### Personal Portfolio Project Scaffold
- Best use case: Add a project to portfolio.
- Prompt:
```text
Scaffold a new personal portfolio project entry from these notes: [notes].
Return: project title, summary, proof points, tech stack, images needed, links needed, and content file changes after approval.
```
- Expected output: Portfolio content scaffold.
- Safety/approval gates: Avoid workplace-specific details.

### Game Backlog Tracker Scaffold
- Best use case: Plan a personal tracker app.
- Prompt:
```text
Plan a personal game backlog tracker scaffold.
Return: user stories, data fields, views, filters, recommendation rules, import/export plan, and MVP vs later scope.
```
- Expected output: Tracker scaffold.
- Safety/approval gates: Ask before files.

### AI Tool MVP Scaffold
- Best use case: Plan a small AI utility.
- Prompt:
```text
Plan an AI tool MVP scaffold for this personal use case: [use case].
Return: user flow, prompt boundaries, model assumptions, data safety, UI, backend needs, evals, and guardrails.
```
- Expected output: AI tool plan.
- Safety/approval gates: No secrets or external accounts.

### Documentation Scaffold
- Best use case: Create project docs.
- Prompt:
```text
Plan documentation for this personal project: [project].
Return: README, project brief, architecture notes, runbook, changelog, safety notes, and file list.
```
- Expected output: Docs scaffold.
- Safety/approval gates: No writes without approval.

### Prompt-To-Project Scaffold
- Best use case: Convert prompt into project plan.
- Prompt:
```text
Convert this rough prompt into a personal project scaffold: [prompt].
Return: clarified goal, repo structure, tasks, prompts, workflows, evals, risks, and approval gates.
```
- Expected output: Project scaffold.
- Safety/approval gates: Planning only.
