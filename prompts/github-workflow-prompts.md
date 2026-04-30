# GitHub Workflow Prompts

## Purpose
Plan branches, issues, PRs, commits, diffs, pre-push checks, repo hygiene, and release notes safely.

## When To Use
Use for personal repositories before committing, pushing, or opening PRs.

## Related Agents
- Web Development Agent
- Writing Agent
- System Design Agent

## Related Skills
- Code Review
- Technical Documentation
- Deployment Readiness Review

## Related Workflows
- Web App Build Workflow
- Project Triage Workflow
- Integration Safety Review Workflow

## Safety Notes
No push without explicit approval. Do not include secrets, `.env`, hidden files, logs, local config, or job/workplace material.

## Prompts

### Branch Planning
- Best use case: Name and scope a branch.
- Prompt:
```text
Plan a Git branch for this personal change: [change].
Return: branch name, scope, files likely to change, risks, validation, and stopping point before commit/push.
```
- Expected output: Branch plan.
- Safety/approval gates: Ask before branch creation if needed.

### Issue Drafting
- Best use case: Create an issue draft.
- Prompt:
```text
Draft a GitHub issue for this personal repo task: [task].
Return: title, problem, acceptance criteria, scope, non-goals, risks, and labels. Do not create the issue.
```
- Expected output: Issue draft.
- Safety/approval gates: No GitHub write.

### PR Description
- Best use case: Prepare a pull request.
- Prompt:
```text
Draft a PR description from this diff summary: [summary].
Return: title, what changed, why, screenshots/checks needed, tests, risks, and review notes.
```
- Expected output: PR draft.
- Safety/approval gates: Do not open PR unless approved.

### Commit Message Planning
- Best use case: Name a focused commit.
- Prompt:
```text
Suggest commit messages for these changes: [diff summary].
Return: best message, alternatives, body bullets, and whether changes should be split.
```
- Expected output: Commit message options.
- Safety/approval gates: No commit.

### Diff Review
- Best use case: Review before commit.
- Prompt:
```text
Review this repo diff without changing files.
Return: behavioral changes, risks, missing tests, accidental files, secret/workplace-data check, and commit readiness.
```
- Expected output: Diff review.
- Safety/approval gates: No edits.

### Pre-Push Checklist
- Best use case: Final gate before push.
- Prompt:
```text
Create a pre-push checklist for this personal repo.
Include status, diff, tests/build, secrets check, hidden/.env check, branch/remote, deploy risk, and explicit push approval.
```
- Expected output: Checklist.
- Safety/approval gates: No push without approval.

### Repo Hygiene Review
- Best use case: Improve repository cleanliness.
- Prompt:
```text
Review repo hygiene in read-only mode.
Check docs, scripts, tests, ignored files, dependency risk, project structure, and missing safety docs. Do not read hidden files or `.env` files.
```
- Expected output: Repo hygiene report.
- Safety/approval gates: No edits.

### Release Note Draft
- Best use case: Summarize a release.
- Prompt:
```text
Draft release notes from these safe changes: [changes].
Return: summary, improvements, fixes, breaking changes, migration notes, and known issues.
```
- Expected output: Release notes draft.
- Safety/approval gates: No publishing.
