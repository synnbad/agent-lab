# Grill-Me Prompts

## Purpose
Use Grill-Me Sinbad to stress-test ideas, scopes, plans, prompts, architecture, and delivery decisions.

## When To Use
Use before implementation, client handoff, deployment, workflow creation, or any plan that feels too vague or bloated.

## Related Agents
- Grill-Me Sinbad
- System Design Agent
- Web Development Agent
- Client-to-MVP Website Agent
- UI Agent

## Related Skills
- Grill-Me Sinbad
- MVP Scope Control
- Architecture Review
- Code Review
- Deployment Readiness Review

## Related Workflows
- Project Triage Workflow
- Web App Build Workflow
- Client Website Delivery Workflow
- System Design Workflow
- Workflow Creation Mode

## Safety Notes
Keep critique direct, precise, and useful. Do not access job/workplace material. Do not include private client details unless redacted. Do not write files or take external actions unless explicitly approved.

## Prompts

### Grill This Project Idea
- Best use case: Pressure-test a new personal idea.
- Prompt:
```text
Use Grill-Me Sinbad on this personal project idea: [idea].
Identify weak assumptions, unclear users, missing proof, scope creep, likely failure points, and the smallest useful MVP. Be direct and precise, not performatively harsh.
```
- Expected output: Cuts, keeps, risks, MVP.
- Safety/approval gates: Planning only.

### Grill This Portfolio Refresh Plan
- Best use case: Make a portfolio plan less generic.
- Prompt:
```text
Grill this personal portfolio refresh plan: [plan].
Check whether it sells me clearly, proves technical ability, avoids generic claims, supports personal client work, and has a focused MVP. Avoid workplace-specific details.
```
- Expected output: Sharpened direction.
- Safety/approval gates: No file edits.

### Grill This MVP Scope
- Best use case: Cut bloated scope.
- Prompt:
```text
Critique this MVP scope: [scope].
Separate must-have, should-have, later, and cut. Identify the riskiest assumption and the fastest validation step.
```
- Expected output: Prioritized scope.
- Safety/approval gates: No implementation.

### Grill This Technical Architecture
- Best use case: Catch overengineering.
- Prompt:
```text
Review this technical architecture: [architecture].
Find unnecessary complexity, missing failure modes, weak data boundaries, unclear ownership, scaling assumptions, and cheaper simpler options.
```
- Expected output: Architecture critique and revised recommendation.
- Safety/approval gates: No config changes.

### Grill This Client Website Spec
- Best use case: Improve a personal client website spec.
- Prompt:
```text
Grill this redacted personal client website spec: [spec].
Check scope, copy gaps, UX risk, accessibility risk, content readiness, launch blockers, and handoff clarity. Do not include private client details in the output.
```
- Expected output: Spec risks and tighter MVP.
- Safety/approval gates: No deployment or client messages.

### Grill This Deployment Plan
- Best use case: Review before launch approval.
- Prompt:
```text
Critique this deployment plan: [plan].
Identify missing environment variables, rollback gaps, build risks, DNS/domain assumptions, secrets handling, approval gates, and whether production deploy should proceed.
```
- Expected output: Deploy readiness decision.
- Safety/approval gates: No deploy without explicit approval.

### Grill This Prompt Before I Use It
- Best use case: Harden a prompt.
- Prompt:
```text
Review this prompt before I use it: [prompt].
Find ambiguity, missing constraints, unsafe permissions, weak output format, hidden external actions, prompt injection risk, and missing approval gates. Return a safer revised prompt.
```
- Expected output: Safer prompt.
- Safety/approval gates: Do not execute the prompt.
