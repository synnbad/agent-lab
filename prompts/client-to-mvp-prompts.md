# Client-To-MVP Prompts

## Purpose
Turn redacted personal client website notes into scoped MVP plans, build prompts, review checklists, and handoff artifacts.

## When To Use
Use for personal client website work that is not connected to job/workplace material.

## Related Agents
- Client-to-MVP Website Agent
- Web Development Agent
- UI Agent
- Accessibility Agent
- Writing Agent

## Related Skills
- Client Brief Extraction
- Requirements Discovery
- MVP Scope Control
- Technical Documentation
- Deployment Readiness Review

## Related Workflows
- Client Website Delivery Workflow
- Web App Build Workflow
- Accessibility Audit Workflow
- Project Triage Workflow

## Safety Notes
Do not store raw client files in this public repo. Redact private client information. Do not include secrets, credentials, private URLs, or tokens. Do not deploy, message the client, connect accounts, or change DNS without explicit approval.

## Prompts

### Client Brief Extraction
- Best use case: Turn notes into structured requirements.
- Prompt:
```text
Extract a personal client website brief from these redacted notes: [notes].
Return: business goal, audience, pages, content needed, visual preferences, functional requirements, constraints, unknowns, MVP scope, and questions for the client.
```
- Expected output: Structured client brief.
- Safety/approval gates: Draft only; no client contact.

### Website Spec Generation
- Best use case: Create a build-ready spec.
- Prompt:
```text
Generate a website spec from this approved brief: [brief].
Return: site map, page sections, components, content inventory, form behavior, accessibility requirements, SEO basics, analytics assumptions, and acceptance criteria.
```
- Expected output: Website spec.
- Safety/approval gates: No implementation yet.

### MVP Scope Control
- Best use case: Prevent scope creep.
- Prompt:
```text
Use MVP Scope Control on this personal client website scope: [scope].
Separate launch MVP, post-launch, optional, and cut. Identify risks, missing content, and approval gates.
```
- Expected output: Scoped MVP.
- Safety/approval gates: No promises to client.

### AI Build Prompt Generation
- Best use case: Produce a high-quality build prompt.
- Prompt:
```text
Create an AI build prompt for this approved personal client website MVP.
Include stack assumptions, page structure, components, content placeholders, accessibility, responsive behavior, no secrets, and validation checks.
Do not include private client data. Return the prompt only.
```
- Expected output: Copy-paste build prompt.
- Safety/approval gates: Review before implementation.

### UI Review
- Best use case: Review design before launch.
- Prompt:
```text
Review this personal client website UI: [description or screenshots].
Return: hierarchy issues, clarity issues, responsiveness risks, form UX, content gaps, visual polish, and prioritized fixes.
```
- Expected output: UI punch list.
- Safety/approval gates: No edits unless approved.

### Accessibility Review
- Best use case: Check client site accessibility.
- Prompt:
```text
Run an accessibility review for this personal client website.
Check headings, landmarks, keyboard navigation, focus states, link text, form labels, alt text, contrast risks, and reduced motion. Return remediation steps.
```
- Expected output: Accessibility checklist.
- Safety/approval gates: No deployment.

### Client Handoff
- Best use case: Prepare review materials.
- Prompt:
```text
Draft a client handoff summary for this personal website project.
Use redacted client details only. Include what changed, how to review, known limits, content still needed, launch checklist, and questions.
Do not send the message.
```
- Expected output: Draft-only handoff.
- Safety/approval gates: No outbound message.

### Netlify Readiness
- Best use case: Prepare for deployment without deploying.
- Prompt:
```text
Review Netlify readiness for this personal client website.
Return: build command, publish directory, environment variables checklist, redirects/functions needs, preview URL review plan, rollback plan, and approval needed before deploy.
```
- Expected output: Deployment readiness report.
- Safety/approval gates: No deploy.

### Revision Planning
- Best use case: Convert feedback into next iteration.
- Prompt:
```text
Turn this redacted client feedback into a revision plan: [feedback].
Return: accepted changes, questions, out-of-scope requests, estimated effort, priority, and next approval gate.
```
- Expected output: Revision backlog.
- Safety/approval gates: No client messages.
