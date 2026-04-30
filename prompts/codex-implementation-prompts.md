# Codex Implementation Prompts

## Purpose
Use Codex to implement approved personal-project plans after OpenClaw or ChatGPT produces a plan.

## When To Use
Use these prompts when file edits are approved inside a personal repo and you need implementation, refactoring, build fixes, or diff review.

## Related Agents
- Web Development Agent
- Backend Agent
- UI Agent
- Accessibility Agent
- System Design Agent

## Related Skills
- Code Review
- Architecture Review
- Technical Documentation
- Deployment Readiness Review
- MVP Scope Control

## Related Workflows
- Web App Build Workflow
- Backend API Workflow
- Accessibility Audit Workflow
- System Design Workflow
- Project Triage Workflow

## Safety Notes
Do not read hidden files or `.env` files. Do not access job/workplace material. Do not print, store, log, or commit secrets. Do not commit, push, deploy, send messages, connect accounts, or change config unless explicitly approved. Stop before commit unless approval is explicit.

## Prompts

### Implement Approved Plan On New Branch
- Best use case: Begin approved implementation safely.
- Prompt:
```text
Work in this personal repo: [repo path].
Implement only this approved plan: [plan].
First inspect non-hidden, non-secret files needed for the change. Create or switch to a new branch named [branch name] only if approved. Do not read `.env` files. Do not access job/workplace material.
Do not commit, push, deploy, send messages, or connect accounts. After edits, run safe validation commands and summarize the diff.
```
- Expected output: Implemented changes, validation result, diff summary.
- Safety/approval gates: Branch creation and file writes must be approved.

### Apply Portfolio Refresh Changes
- Best use case: Implement a reviewed portfolio plan.
- Prompt:
```text
Implement the approved personal portfolio refresh plan in /Users/sinbadadjuik/Projects/personal-projects/portfolio.
Allowed scope: [files or sections].
Do not read hidden files or `.env` files. Avoid workplace-specific details; use generic "blocked workplace-related items" wording if needed.
Do not commit, push, deploy, or connect accounts. Run typecheck/build if available and report changed files.
```
- Expected output: Portfolio source changes and validation.
- Safety/approval gates: Stop before commit.

### Implement Website MVP From Build Prompt
- Best use case: Build a small personal/client website MVP.
- Prompt:
```text
Use the approved MVP build prompt below to implement a personal website MVP.
Repo: [repo path]
Approved write scope: [paths]
Build prompt: [paste prompt]
Do not read hidden files or `.env` files. Do not include secrets or private client details. Do not commit, push, deploy, or message anyone.
Return: files changed, validation, known gaps, next approval needed.
```
- Expected output: MVP implementation and handoff notes.
- Safety/approval gates: No deployment.

### Refactor Without Changing Behavior
- Best use case: Clean code while preserving behavior.
- Prompt:
```text
Refactor the approved files without changing user-visible behavior.
Repo: [repo path]
Files: [file list]
Keep public APIs, routes, copy, and styling behavior stable unless explicitly listed.
Do not read hidden files or `.env` files. Do not commit, push, or deploy. Run tests/build if available. Report behavior-preservation evidence.
```
- Expected output: Focused refactor and checks.
- Safety/approval gates: No unrelated rewrites.

### Fix Build Or Typecheck Errors
- Best use case: Repair failing validation.
- Prompt:
```text
Fix the build/typecheck/test errors in this personal repo.
Run only the relevant failing command first: [command].
Inspect non-hidden files needed for the failure. Do not read `.env` files. Do not change unrelated behavior. Do not commit, push, or deploy.
Return: root cause, files changed, validation command output summary, remaining risks.
```
- Expected output: Minimal fix and validation.
- Safety/approval gates: Stop if secret/config access is required.

### Produce Diff Summary
- Best use case: Review local changes before commit.
- Prompt:
```text
Review the current local diff in this repo without modifying files.
Do not read hidden files or `.env` files. Do not access job/workplace material.
Return: changed files, user-facing behavior changes, risks, tests run or missing, commit readiness, recommended commit message.
```
- Expected output: Review-ready diff summary.
- Safety/approval gates: No edits.

### Stop Before Commit
- Best use case: Make implementation but leave commit to user approval.
- Prompt:
```text
Implement the approved change, then stop before committing.
Do not run git commit, git push, deploy, message, or connect accounts.
At the end, provide exact commands I could run manually after review.
```
- Expected output: Changes plus manual next commands.
- Safety/approval gates: Commit requires explicit approval.

### Commit Only After Review
- Best use case: Prepare a commit after user review.
- Prompt:
```text
Review the staged/unstaged diff first. If and only if I explicitly approve, create one focused commit with message: [message].
Do not push. Do not deploy. Do not include secrets, hidden files, `.env` files, logs, or local config.
Return: commit hash, files committed, and push command for manual review.
```
- Expected output: Local commit only, if approved.
- Safety/approval gates: Explicit commit approval required.
