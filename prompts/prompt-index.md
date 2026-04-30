# Prompt Index

## Purpose
Index all prompt packs in `prompts/` so users can choose the right operational prompt quickly.

## When To Use
Use this file before starting a task, especially when deciding whether the task is read-only, implementation, deployment, GitHub workflow, or communication-adjacent.

## Related Agents
- All personal project agents in `agents/`

## Related Skills
- Requirements Discovery
- MVP Scope Control
- Code Review
- Data Privacy Review

## Related Workflows
- Project Triage Workflow
- Workflow Creation Mode
- Web App Build Workflow
- Integration Safety Review Workflow

## Safety Notes
Start with the lowest-risk prompt that can answer the question. Do not use prompts to access job/workplace material. Use explicit approval gates before writes, deploys, messages, config changes, commits, pushes, or account connections.

## Prompts
This index points to prompt packs rather than providing task prompts directly. Choose a pack from the table below.

| Prompt Pack | Purpose | Primary Agent | Best Use | Risk Level |
|---|---|---|---|---|
| `accessibility-prompts.md` | Accessibility reviews and remediation plans | Accessibility Agent | WCAG-focused review before implementation | Low |
| `automation-prompts.md` | Safe automation planning and script design | Automation Agent | Dry-run automation design | Medium |
| `backend-prompts.md` | API, data model, validation, auth, and backend safety | Backend Agent | Backend planning or approved implementation | Medium |
| `client-to-mvp-prompts.md` | Turn personal client website notes into an MVP plan | Client-to-MVP Website Agent | Personal client website scoping | Medium |
| `codex-implementation-prompts.md` | Convert approved plans into local code changes | Web Development Agent | Approved Codex implementation | Medium |
| `dashboard-reporting-prompts.md` | Personal dashboard and report planning | Data Analysis Agent | Personal reporting artifacts | Medium |
| `data-analysis-prompts.md` | Cleaning, metrics, EDA, and privacy-safe findings | Data Analysis Agent | Personal or public data analysis | Medium |
| `debugging-prompts.md` | Reproduce, isolate, and fix defects safely | Web Development Agent | Bug triage and repair plan | Medium |
| `github-workflow-prompts.md` | Branch, issue, PR, commit, and pre-push planning | Web Development Agent | GitHub workflow prep without pushing | High |
| `grill-me-prompts.md` | Direct critique of plans, scopes, prompts, and architecture | Grill-Me Sinbad | Stress-test before execution | Low |
| `library-assessment-prompts.md` | Generic assessment planning and reporting | Research Agent | Personal or public assessment-style projects | Medium |
| `netlify-deployment-prompts.md` | Netlify readiness, deploy checks, and rollback notes | Web Development Agent | Deployment planning before approval | High |
| `openclaw-planner-prompts.md` | Read-only OpenClaw planning and validation | OpenClaw planner mode | Sandbox-safe planning | Low |
| `personal-project-scaffold-prompts.md` | Scaffold personal project plans and docs | System Design Agent | Planning a new personal project | Medium |
| `portfolio-refresh-prompts.md` | Refresh the personal portfolio website | Web Development Agent | Portfolio planning and approved implementation | Medium |
| `project-kickoff-prompts.md` | Clarify new project requests and route work | System Design Agent | First pass on a new idea | Low |
| `prompt-review-prompts.md` | Improve rough prompts for clarity and safety | Writing Agent | Prompt hardening | Low |
| `research-prompts.md` | Research questions, evidence tables, and synthesis | Research Agent | Public research and citation-aware summary | Low |
| `safety-check-prompts.md` | Secret, workplace, write, deploy, message, and connector checks | Data Governance Privacy Agent | Pre-action safety review | High |
| `stakeholder-insight-prompts.md` | Generic audience insight and briefing prompts | Writing Agent | Personal stakeholder-style summaries | Medium |
| `survey-assessment-prompts.md` | Generic survey planning and analysis prompts | Research Agent | Personal survey or feedback collection | Medium |
| `system-design-prompts.md` | Architecture, reliability, observability, and ADRs | System Design Agent | Architecture planning | Medium |
| `ui-design-prompts.md` | UI critique, hierarchy, responsiveness, and handoff | UI Agent | Visual and interaction review | Low |
| `ux-assessment-prompts.md` | UX study planning, usability findings, and remediation | UX Assessment Agent | Personal UX review | Medium |
| `web-development-prompts.md` | React/Vite inspection, routing, components, and build triage | Web Development Agent | Web app planning and review | Medium |
| `workflow-creation-mode-prompts.md` | Create a new workflow when none fits | System Design Agent | New repeatable personal process | Medium |
| `writing-prompts.md` | Reports, docs, summaries, posts, and draft-only messages | Writing Agent | Clear writing and documentation | Medium |

Risk levels:
- Low: planning/read-only
- Medium: file edits inside personal projects
- High: deployment, GitHub push, external communication, config changes
- Critical: sensitive data, workplace data, destructive actions
