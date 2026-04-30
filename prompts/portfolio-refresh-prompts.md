# Portfolio Refresh Prompts

## Purpose
Plan, critique, implement, and review updates to the personal portfolio website.

## When To Use
Use for the personal portfolio repo at `https://github.com/synnbad/portfolio` and local clone paths approved by the user.

## Related Agents
- Web Development Agent
- UI Agent
- Accessibility Agent
- Writing Agent
- Grill-Me Sinbad

## Related Skills
- Code Review
- Technical Documentation
- MVP Scope Control
- Deployment Readiness Review
- Grill-Me Sinbad

## Related Workflows
- Project Triage Workflow
- Web App Build Workflow
- Accessibility Audit Workflow
- Client Website Delivery Workflow

## Safety Notes
Personal portfolio only. Do not access job/workplace material. Avoid workplace-specific details. Do not read hidden files or `.env` files. Do not write, commit, push, deploy, send messages, browse, or connect accounts unless explicitly approved.

## Prompts

### Read-Only Portfolio Inspection
- Best use case: Understand the current repo.
- Prompt:
```text
Inspect my personal portfolio repo in read-only mode: [local path].
Allowed: README.md, package.json, client/, src/, app/, pages/, components/, public/, content/, data/, styles/, docs/, vite.config.ts, netlify.toml.
Forbidden: hidden files, `.env` files, secrets, credentials.
Return: stack, structure, scripts, main pages, content sources, risks, and next safe step.
```
- Expected output: Concrete repo summary.
- Safety/approval gates: No edits.

### Portfolio Positioning Critique
- Best use case: Clarify what the site should sell.
- Prompt:
```text
Critique my personal portfolio positioning.
Audience: [audience]
Current positioning: [paste]
Return: sharper positioning, proof points needed, weak claims to cut, project evidence to highlight, and homepage headline options. Avoid workplace-specific details.
```
- Expected output: Positioning recommendation.
- Safety/approval gates: Planning only.

### Homepage Refresh Plan
- Best use case: Redesign the homepage structure.
- Prompt:
```text
Create a homepage refresh plan for my personal portfolio.
Use the current repo structure if available. Return: hero, proof strip, featured projects, services/client work, about preview, writing/contact, CTA, responsive considerations, and files likely to change later.
```
- Expected output: Section-by-section plan.
- Safety/approval gates: No file writes.

### Project Card Rewrite
- Best use case: Improve project descriptions.
- Prompt:
```text
Rewrite these project cards for a personal portfolio.
Project notes: [paste]
For each card return: title, one-line outcome, problem, build details, stack, proof/result, links needed, and missing evidence. Avoid workplace-specific details.
```
- Expected output: Stronger project cards.
- Safety/approval gates: Do not invent results.

### About Page And Content
- Best use case: Improve bio and resume flow.
- Prompt:
```text
Draft improved personal portfolio About content from these notes: [notes].
Return: short bio, longer bio, skills framing, credibility proof, personal-client angle, resume CTA, and content to avoid.
```
- Expected output: About page copy.
- Safety/approval gates: Draft only.

### Contact Flow Improvement
- Best use case: Make contact clearer.
- Prompt:
```text
Review the portfolio contact flow.
Return: desired user actions, form/link recommendations, spam/privacy concerns, accessible labels, response expectation copy, and no-backend fallback.
```
- Expected output: Contact flow plan.
- Safety/approval gates: No messages or account connections.

### SEO And Accessibility Improvement
- Best use case: Improve discoverability and usability.
- Prompt:
```text
Review the portfolio for SEO and accessibility opportunities.
Return: page titles, descriptions, headings, landmarks, alt text needs, link text, keyboard/focus checks, performance risks, and a prioritized remediation checklist.
```
- Expected output: SEO/accessibility checklist.
- Safety/approval gates: Review only.

### Codex Implementation For Portfolio Refresh
- Best use case: Implement an approved refresh.
- Prompt:
```text
Use Codex to implement the approved personal portfolio refresh plan in [local path].
Approved files: [file list]
Do not read hidden files or `.env` files. Do not include secrets. Do not commit, push, deploy, send messages, browse, or connect accounts.
Run safe validation and return changed files, diff summary, risks, and next approval gate.
```
- Expected output: Local changes and validation.
- Safety/approval gates: Stop before commit.

### QA Checklist
- Best use case: Test after changes.
- Prompt:
```text
Create a QA checklist for the personal portfolio refresh.
Include: responsive checks, navigation, content accuracy, project links, accessibility, SEO metadata, build command, Netlify assumptions, and rollback notes. Do not deploy.
```
- Expected output: Manual QA checklist.
- Safety/approval gates: No deploy.

### Commit Review
- Best use case: Review before committing.
- Prompt:
```text
Review the portfolio repo diff before commit.
Do not modify files. Return: changed files, user-facing changes, risk, tests run, missing checks, secret/workplace-data check, and recommended commit message.
```
- Expected output: Commit readiness report.
- Safety/approval gates: No commit or push.
