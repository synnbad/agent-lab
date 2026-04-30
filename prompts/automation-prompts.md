# Automation Prompts

## Purpose
Plan safe personal automations, scripts, file processing workflows, and dry-run behavior.

## When To Use
Use before writing scripts, scheduling jobs, modifying files, or automating repetitive personal tasks.

## Related Agents
- Automation Agent
- Backend Agent
- System Design Agent

## Related Skills
- Requirements Discovery
- Technical Documentation
- Code Review
- Data Privacy Review

## Related Workflows
- Project Triage Workflow
- Backend API Workflow
- Integration Safety Review Workflow

## Safety Notes
Dry-run first. Do not access job/workplace material. Do not read hidden files or `.env` files. Do not schedule cron jobs, modify files, send messages, or connect accounts without approval.

## Prompts

### Python Automation Planning
- Best use case: Plan a script safely.
- Prompt:
```text
Plan a Python automation for this personal task: [task].
Return: inputs, outputs, dry-run behavior, file scope, error handling, logging, safety checks, and approval gates.
```
- Expected output: Script plan.
- Safety/approval gates: No file writes until approved.

### File Processing Workflow
- Best use case: Process files safely.
- Prompt:
```text
Design a file processing workflow for: [task].
Allowed folder: [path]
Return: file selection rules, excluded files, hidden/`.env` avoidance, dry-run output, backup strategy, and validation.
```
- Expected output: File workflow spec.
- Safety/approval gates: Path-scoped writes only after approval.

### Logging And Error Handling
- Best use case: Make scripts debuggable.
- Prompt:
```text
Design logging and error handling for this automation: [automation].
Return: log levels, redaction rules, recoverable errors, fatal errors, retry policy, and user-facing summary.
```
- Expected output: Logging plan.
- Safety/approval gates: Do not log secrets.

### CLI Script Design
- Best use case: Define command interface.
- Prompt:
```text
Design a CLI for this personal automation: [automation].
Return: commands, flags, defaults, dry-run mode, confirmation prompts, examples, and unsafe operation guards.
```
- Expected output: CLI spec.
- Safety/approval gates: Confirm destructive actions.

### Automation Safety Review
- Best use case: Review before implementation.
- Prompt:
```text
Review this automation plan for safety: [plan].
Find risks involving files, secrets, external accounts, messages, scheduling, deletions, and prompt injection. Return approval gates and safer alternatives.
```
- Expected output: Safety review.
- Safety/approval gates: No execution.

### Dry-Run Mode Design
- Best use case: Add preview behavior.
- Prompt:
```text
Design dry-run mode for this automation: [automation].
Return: what it would print, what it must not change, sample output, and criteria for switching to live mode.
```
- Expected output: Dry-run spec.
- Safety/approval gates: Live mode requires approval.

### Cron Scheduler Caution
- Best use case: Avoid unsafe scheduling.
- Prompt:
```text
Evaluate whether this automation should be scheduled: [automation].
Return: why scheduling may be risky, safer manual trigger, required monitoring, rollback, and approval needed.
```
- Expected output: Scheduling decision.
- Safety/approval gates: No cron without explicit approval.

### Automation Documentation
- Best use case: Document scripts.
- Prompt:
```text
Draft documentation for this automation: [description].
Include purpose, setup, inputs, outputs, dry-run examples, safety warnings, troubleshooting, and rollback.
```
- Expected output: README-style docs.
- Safety/approval gates: Do not include secrets.
