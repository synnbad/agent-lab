# Integration Safety Review Workflow

## Purpose
Review Integration Adapter use before reads, writes, deployments, or sensitive data access.

## Trigger
Use before enabling Level 2, Level 3, or Level 4 access.

## Inputs
- Goal, audience, and desired artifact
- Source material, constraints, risks, and approval status

## Step-by-Step Process
1. Identify data sensitivity and action type
2. Confirm permissions and approval
3. Separate read tools from write tools
4. Label destructive actions
5. Plan logging and fallback
6. Proceed only within approved scope

## Output
A Markdown-ready deliverable with summary, decisions, assumptions, risks, quality checks, and next steps.

## Quality Control
Verify that the output is grounded in source context, privacy-safe, scoped to the goal, and clear enough for another person or agent to continue.

## Failure Modes
Missing source context, hidden assumptions, overbroad scope, unapproved external actions, weak privacy handling, and unclear ownership.

## Example
Use this workflow to move from a rough request to a reviewed, documented, and safe next-step artifact.
