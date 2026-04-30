# Debugging Prompts

## Purpose
Diagnose and fix personal-project bugs with minimal, safe changes.

## When To Use
Use when a build, test, runtime behavior, UI flow, or integration is failing.

## Related Agents
- Web Development Agent
- Backend Agent
- System Design Agent
- UI Agent

## Related Skills
- Code Review
- Architecture Review
- Technical Documentation
- Data Privacy Review

## Related Workflows
- Web App Build Workflow
- Backend API Workflow
- Project Triage Workflow

## Safety Notes
Do not read hidden files or `.env` files. Do not access job/workplace material. Do not print secrets. Do not commit, push, deploy, send messages, or connect accounts unless explicitly approved.

## Prompts

### Reproduce And Isolate
- Best use case: Start a bug investigation.
- Prompt:
```text
Debug this personal-project issue: [issue].
First reproduce or inspect the failure using safe commands. Do not read hidden files or `.env` files. Return: reproduction steps, observed behavior, expected behavior, likely area, and next safe check.
```
- Expected output: Repro and hypothesis.
- Safety/approval gates: Ask before edits.

### Build Error Triage
- Best use case: Fix failing build.
- Prompt:
```text
Run or inspect this failing build command: [command].
Find the smallest fix. Do not change unrelated behavior. Do not read `.env` files. Return: root cause, files to edit, fix plan, validation command.
```
- Expected output: Build repair plan or fix.
- Safety/approval gates: Edits require approval.

### Runtime Bug Trace
- Best use case: Track bad behavior through code.
- Prompt:
```text
Trace this runtime bug through the code: [bug].
Inspect only relevant non-hidden files. Return: data/control flow, likely defect, evidence, minimal fix, and regression test idea.
```
- Expected output: Debug trace.
- Safety/approval gates: No broad scans.

### UI Interaction Bug
- Best use case: Debug broken interactions.
- Prompt:
```text
Debug this UI interaction: [description].
Review component state, event handlers, routing, responsive behavior, and accessibility impact. Return likely cause, fix options, and validation checklist.
```
- Expected output: UI bug plan.
- Safety/approval gates: No external actions.

### API Failure Triage
- Best use case: Diagnose backend or function failures.
- Prompt:
```text
Diagnose this API/backend failure: [error or behavior].
Do not print secrets. Do not inspect `.env` files. Return: request path, validation/auth/data/error-handling risks, likely cause, minimal fix, and test cases.
```
- Expected output: Backend diagnosis.
- Safety/approval gates: No secret access.

### Regression Guard
- Best use case: Prevent repeat failures.
- Prompt:
```text
Design a regression check for this fixed bug: [bug and fix].
Return: test case, manual QA steps, edge cases, and where the check belongs. Do not implement unless approved.
```
- Expected output: Regression plan.
- Safety/approval gates: Draft only.
