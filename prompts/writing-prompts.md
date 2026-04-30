# Writing Prompts

## Purpose
Draft, revise, and clarify personal-project writing, reports, documentation, summaries, and public-facing copy.

## When To Use
Use for README work, reports, memos, executive summaries, project posts, documentation cleanup, and draft-only messages.

## Related Agents
- Writing Agent
- Research Agent
- Client-to-MVP Website Agent
- Data Analysis Agent

## Related Skills
- Technical Documentation
- Assessment Report Writing
- Stakeholder Briefing
- Dashboard Storytelling
- Literature Review

## Related Workflows
- Report Generation Workflow
- Client Website Delivery Workflow
- Data Analysis Workflow
- Project Triage Workflow

## Safety Notes
Do not include secrets, private client details, or job/workplace material. Email and message prompts are draft-only unless explicitly approved.

## Prompts

### Report Writing
- Best use case: Turn notes into a clear report.
- Prompt:
```text
Write a clear report from these safe notes: [notes].
Return: title, summary, findings, evidence, limitations, recommendations, and next steps. Use generic "blocked workplace-related items" wording if needed.
```
- Expected output: Structured report.
- Safety/approval gates: No private data.

### Memo Writing
- Best use case: Create a concise decision memo.
- Prompt:
```text
Draft a memo for this personal project decision: [context].
Return: context, decision needed, options, tradeoffs, recommendation, risks, and next step.
```
- Expected output: Decision memo.
- Safety/approval gates: Draft only.

### Executive Summary
- Best use case: Summarize long material.
- Prompt:
```text
Create an executive summary from this safe content: [content].
Return: 5-bullet summary, key decision, evidence, risks, and recommended action.
```
- Expected output: Concise summary.
- Safety/approval gates: No hidden/private content.

### Documentation Cleanup
- Best use case: Improve docs.
- Prompt:
```text
Rewrite this documentation for clarity: [text].
Preserve meaning. Return improved version, assumptions, missing details, and suggested headings.
```
- Expected output: Clearer docs.
- Safety/approval gates: Do not invent facts.

### Email Draft Only
- Best use case: Draft a personal email without sending.
- Prompt:
```text
Draft an email for this personal context: [context].
Do not send. Return subject, body, tone notes, risks, and whether exact approval would be needed before sending.
```
- Expected output: Draft email.
- Safety/approval gates: No send without exact approval.

### Project Post
- Best use case: Write public project update copy.
- Prompt:
```text
Draft a LinkedIn/project post for this personal project: [project notes].
Avoid private client details and workplace-specific details. Return short, medium, and technical versions.
```
- Expected output: Post drafts.
- Safety/approval gates: Draft only.

### README Rewrite
- Best use case: Improve project README.
- Prompt:
```text
Rewrite this README for a personal project: [README text].
Return: improved README, missing sections, install/use assumptions, and safety notes.
```
- Expected output: README draft.
- Safety/approval gates: Do not include secrets.

### Plain-Language Rewrite
- Best use case: Make writing easier to understand.
- Prompt:
```text
Rewrite this text in plain language: [text].
Preserve technical accuracy. Return plain version, glossary, and any claims that need evidence.
```
- Expected output: Plain-language copy.
- Safety/approval gates: No unsupported claims.
