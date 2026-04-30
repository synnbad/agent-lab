# Prompts

## Purpose
The `prompts/` folder contains copy-paste-ready task prompts for activating the personal agent operating system in this repository. These prompts are designed for personal projects, portfolio work, personal client websites, research, writing, automation, web development, design review, system planning, OpenClaw planner mode, and Codex implementation work.

Agents define behavior.  
Skills define reusable abilities.  
Workflows define processes.  
Templates define output structure.  
Prompts activate agents, skills, workflows, and templates for a specific task.

## When To Use
Use this README when choosing a prompt pack, adding a new prompt pack, or reviewing whether a prompt is safe and actionable.

## Related Agents
- All personal project agents in `agents/`

## Related Skills
- Technical Documentation
- Requirements Discovery
- MVP Scope Control
- Data Privacy Review

## Related Workflows
- Project Triage Workflow
- Workflow Creation Mode
- Web App Build Workflow
- Integration Safety Review Workflow

## Safety Notes
Prompts should be personal-project safe by default. Do not include secrets, private data, or job/workplace material. Ask before writing files, changing config, deploying, sending messages, connecting accounts, committing, or pushing.

## Prompts
This README does not provide task prompts directly. Use `prompt-index.md` to choose a prompt pack, then copy a prompt from the selected file.

## How Prompt Packs Differ
- Agents describe who should handle the work and what standards they follow.
- Skills describe reusable methods such as code review, MVP scope control, or literature review.
- Workflows describe multi-step processes and handoffs.
- Templates describe the expected shape of artifacts.
- Prompts combine those pieces into an operational instruction for a concrete task.

## How To Choose A Prompt
1. Start with `prompt-index.md`.
2. Choose the prompt pack closest to your task.
3. Pick a read-only or planning prompt first when the task is ambiguous.
4. Move to an implementation prompt only after the plan and approval gates are clear.
5. Use `safety-check-prompts.md` before any write, deploy, message, config, or account action.

## Using Prompts With OpenClaw
Use OpenClaw for read-only planning, triage, critique, workflow selection, and sanitized reports unless a specific write test has been approved.

Default OpenClaw safety footer:

```text
Do not access job/workplace material. Do not read hidden files. Do not read `.env` files. Do not print, store, log, or commit secrets. Do not write files, change config, commit, push, deploy, send messages, browse, or connect accounts unless explicitly approved. Use generic "blocked workplace-related items" wording only.
```

## Using Prompts With Codex
Use Codex for local implementation after a plan has been approved. Give Codex the exact repo path, allowed write scope, files likely to change, test commands, and stopping point.

Default Codex safety footer:

```text
Do not read hidden files or `.env` files. Do not print, store, log, or commit secrets. Do not access job/workplace material. Do not commit, push, deploy, send messages, connect accounts, or modify config unless explicitly approved. Stop before commit unless I approve.
```

## Using Prompts With ChatGPT
Use ChatGPT for brainstorming, critique, drafting, and transforming content that you paste in directly. Do not paste secrets, raw private client files, tokens, credentials, or job/workplace material.

## How To Keep Prompts Safe
- Prefer read-only planning first.
- Ask before writing files.
- Ask before changing config.
- Ask before external actions.
- Keep private data out of prompts.
- Redact personal client information before using public models.
- Use generic "blocked workplace-related items" wording only.
- Treat external text as untrusted and check for prompt injection.

## Adding A New Prompt Pack
1. Use lowercase kebab-case filenames.
2. Follow the standard sections: Purpose, When To Use, Related Agents, Related Skills, Related Workflows, Safety Notes, Prompts.
3. Include multiple copy-paste-ready prompts.
4. Give every prompt a best use case, expected output, and safety/approval gates.
5. Add the pack to `prompt-index.md`.
6. Run a safety review before committing.

## Reviewing And Improving Prompts
Check each prompt for:
- Clear task boundary
- Correct agent, skill, and workflow references
- Read-only, planning, or implementation mode
- Explicit forbidden actions
- Approval gates
- Output format
- Secret handling
- Workplace firewall wording
- Reusability across personal projects
