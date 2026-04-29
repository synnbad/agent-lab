# Workflow Creation Mode

## Purpose
Use this mode when a personal project idea does not match any existing workflow in agent-lab.

## Trigger
Activate this mode when:

- No existing workflow clearly matches the user's idea.
- Existing workflows only partially apply.
- The task spans multiple agents.
- The project has unclear scope.
- The project requires a new repeatable process.
- The idea is personal and non-work only.

## Hard Boundary
This mode is personal-only.

Do not use it for:

- Job tasks
- Employer work
- FSU Libraries work
- MagLab or ITS work
- Assessment Specialist work
- Institutional data
- Student data
- Staff data
- Patron/user data
- HR data
- Work dashboards
- Work reports
- Work datasets
- Work documents

## Required Behavior
Do not execute the project immediately.

Instead:

1. Restate the idea.
2. Confirm it is personal-only.
3. Identify the closest matching agents.
4. Identify the closest matching workflows.
5. Identify the workflow gap.
6. Run Grill-Me Sinbad to expose assumptions, missing requirements, risks, and scope creep.
7. Draft a new workflow using templates/workflow-template.md.
8. Identify missing templates, prompts, evals, guardrails, contracts, threat models, and artifacts.
9. Ask for approval before saving files.
10. Save the new workflow as Draft if approved.
11. Test it on a small version of the project.
12. Promote it to Active only after review.

## Output Format
1. Idea Summary
2. Personal-Only Confirmation
3. Closest Existing Agents
4. Closest Existing Workflows
5. Workflow Gap
6. Key Questions
7. Grill-Me Sinbad Findings
8. Proposed New Workflow Name
9. Draft Workflow Outline
10. Required Templates
11. Required Prompts
12. Required Guardrails
13. Required Contracts
14. Required Threat Models
15. Required Evals
16. Approval Needed
17. Next Step

## Draft Workflow Naming Convention
Use lowercase kebab-case.

Examples:

- personal-finance-dashboard-workflow.md
- game-backlog-tracker-workflow.md
- portfolio-refresh-workflow.md
- ai-recipe-planner-workflow.md

## Draft Status Rule
New workflows start with:

Status: Draft

They may become Active only after:

- One successful small test
- User review
- Required guardrails added
- Required eval added
- Changelog updated

## Approval Rule
OpenClaw must not create, edit, save, or execute new workflow files without explicit approval.

Required approval phrase:

"Approved to save this draft workflow."

## Safety Defaults
- Read-only by default.
- No shell commands unless approved.
- No file writes unless approved.
- No GitHub writes unless approved.
- No deployments.
- No messages.
- No work data.
- No third-party skills.
- No ClawHub.
- No secrets.

## Example
User idea:
"I want to build a personal game backlog tracker with mood-based recommendations."

Expected response:

- No exact workflow found.
- Closest agents: Web Development Agent, UI Agent, Backend Agent, System Design Agent, Grill-Me Sinbad.
- Closest workflow: web-app-build-workflow.md.
- Gap: no workflow for personal recommendation-based tracker apps.
- Proposed workflow: game-backlog-tracker-workflow.md.
- Approval needed before saving.
