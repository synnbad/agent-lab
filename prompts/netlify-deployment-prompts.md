# Netlify Deployment Prompts

## Purpose
Review Netlify readiness, deploy previews, environment variables, production approval gates, rollback notes, and handoff summaries.

## When To Use
Use before deploying a personal or personal-client website to Netlify.

## Related Agents
- Web Development Agent
- Client-to-MVP Website Agent
- System Design Agent

## Related Skills
- Deployment Readiness Review
- Technical Documentation
- Code Review

## Related Workflows
- Client Website Delivery Workflow
- Web App Build Workflow
- Integration Safety Review Workflow

## Safety Notes
No deploy without explicit approval. Do not print secrets. Do not read `.env` files. Do not connect Netlify accounts unless approved.

## Prompts

### Netlify Readiness Review
- Best use case: Check before deploy.
- Prompt:
```text
Review Netlify readiness for this personal project: [repo/path].
Do not deploy. Return: framework, build command, publish directory, functions, redirects, env vars needed, risks, and approval gates.
```
- Expected output: Readiness report.
- Safety/approval gates: No deploy.

### Build Command And Publish Directory
- Best use case: Verify config.
- Prompt:
```text
Check the build command and publish directory for Netlify.
Inputs: [package scripts/netlify config]
Return: recommended build command, publish directory, functions directory, and validation command.
```
- Expected output: Netlify config recommendation.
- Safety/approval gates: No config edits without approval.

### Environment Variable Checklist
- Best use case: Avoid secret leaks.
- Prompt:
```text
Create a Netlify environment variable checklist for this project: [project].
Return variable names only when safe, purpose, required/optional, local vs production, and where not to store them.
Do not ask for or print values.
```
- Expected output: Env checklist.
- Safety/approval gates: Never print secret values.

### Deploy Preview Review
- Best use case: Review a preview manually.
- Prompt:
```text
Create a deploy preview review checklist for this site: [site].
Include routing, forms, assets, accessibility, SEO metadata, responsive behavior, console errors, and rollback criteria.
```
- Expected output: Preview QA checklist.
- Safety/approval gates: No production deploy.

### Production Deploy Approval Gate
- Best use case: Decide if launch is allowed.
- Prompt:
```text
Evaluate production deploy readiness.
Inputs: [checks/results]
Return: pass/fail, blockers, risks accepted, exact deploy command if approved, rollback plan, and required approval phrase.
```
- Expected output: Launch decision.
- Safety/approval gates: Explicit deploy approval required.

### Rollback Notes
- Best use case: Prepare for failed deploy.
- Prompt:
```text
Draft rollback notes for this Netlify site.
Return: how to identify failure, rollback method, verification checks, communication draft, and follow-up fixes.
Do not deploy or message anyone.
```
- Expected output: Rollback runbook.
- Safety/approval gates: Draft only.

### Client Handoff Deployment Summary
- Best use case: Explain launch status.
- Prompt:
```text
Draft a deployment handoff summary for a personal client website.
Use redacted details only. Include what changed, preview status, known limitations, launch approval needed, and next steps.
Do not send.
```
- Expected output: Draft handoff.
- Safety/approval gates: No outbound message.
