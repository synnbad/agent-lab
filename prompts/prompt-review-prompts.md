# Prompt Review Prompts

## Purpose
Improve prompts for clarity, safety, specificity, and tool readiness.

## When To Use
Use before giving a prompt to OpenClaw, Codex, ChatGPT, or another AI tool.

## Related Agents
- Writing Agent
- System Design Agent
- Grill-Me Sinbad

## Related Skills
- Technical Documentation
- MVP Scope Control
- Data Privacy Review
- Grill-Me Sinbad

## Related Workflows
- Project Triage Workflow
- Workflow Creation Mode

## Safety Notes
Do not execute prompts during review. Remove secrets, private data, and job/workplace material. Add approval gates for writes, deploys, messages, config, and external actions.

## Prompts

### Review For Ambiguity
- Best use case: Find unclear instructions.
- Prompt:
```text
Review this prompt for ambiguity: [prompt].
Return: unclear goals, missing context, risky assumptions, vague outputs, and a clearer revised prompt.
```
- Expected output: Clarity review.
- Safety/approval gates: Do not execute.

### Harden This Prompt
- Best use case: Make a prompt safer.
- Prompt:
```text
Harden this prompt: [prompt].
Add boundaries for hidden files, `.env`, secrets, workplace material, writes, commits, pushes, deploys, messages, account connections, and output format.
```
- Expected output: Safer prompt.
- Safety/approval gates: No execution.

### Add Safety Gates
- Best use case: Add approvals.
- Prompt:
```text
Add safety and approval gates to this prompt: [prompt].
Return: required approvals, forbidden actions, allowed scope, rollback/stop conditions, and revised prompt.
```
- Expected output: Approval-aware prompt.
- Safety/approval gates: Review only.

### Make Codex-Ready
- Best use case: Convert a request into an implementation prompt.
- Prompt:
```text
Convert this request into a Codex-ready prompt: [request].
Include repo path, allowed files, implementation scope, forbidden actions, validation commands, and stop-before-commit instruction.
```
- Expected output: Codex prompt.
- Safety/approval gates: No push/deploy.

### Make OpenClaw-Ready
- Best use case: Convert a request into read-only planner mode.
- Prompt:
```text
Convert this request into an OpenClaw read-only planner prompt: [request].
Include personal-only boundary, no hidden/.env files, no writes, no external actions, sanitized reporting, and output format.
```
- Expected output: OpenClaw planner prompt.
- Safety/approval gates: Read-only.

### Convert Rough Request
- Best use case: Structure a messy ask.
- Prompt:
```text
Convert this rough request into a structured prompt: [request].
Return: task, context, constraints, allowed actions, forbidden actions, output format, and approval gates.
```
- Expected output: Structured prompt.
- Safety/approval gates: Do not execute.
