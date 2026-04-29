# Integration Adapter Threat Model

## System Or Workflow Being Modeled
Integration Adapter Threat Model

## Assets At Risk
- Read/write permission confusion
- Excessive agency
- Unsupported integration assumptions
- Destructive actions

## Trust Boundaries
External content, user-provided files, Integration Adapters, public repositories, deployment systems, and stakeholder-facing artifacts.

## Possible Attackers Or Failure Sources
Malicious external content, accidental user error, over-permissioned tools, stale assumptions, misconfigured deployments, and unclear ownership.

## Abuse Cases
- Read/write permission confusion
- Excessive agency
- Unsupported integration assumptions
- Destructive actions
- Silent external publishing
- Private data exposure
- Tool output trusted too much
- Integration unavailable
- Cross-platform terminology confusion

## Likely Failure Modes
- Unapproved action or publication
- Sensitive data exposure
- Unsupported claims or incorrect assumptions
- Weak review before handoff

## Preventive Controls
- Default to read-only
- Separate read tools from write tools
- Require explicit approval for writes, deployments, publishing, and sensitive data use
- Provide manual fallback
- Log integration assumptions
- Never assume one platform supports the same connector another platform supports

## Detection Signals
- Unexpected tool request
- Missing approval record
- Sensitive content in output
- Broken build or incorrect published content
- Stakeholder confusion or metric dispute

## Required Approval Gates
Approval is required before writes, deployments, publishing, environment-variable changes, sensitive data use, or stakeholder-facing delivery.

## Manual Fallback
Pause automation, use sanitized summaries, perform manual review, and document the decision before continuing.

## Residual Risk
Some risk remains because external content, human interpretation, and platform behavior can change. Keep human review in the loop.

## Review Checklist
- Assets identified
- Approval gates checked
- Sensitive data minimized
- Fallback documented
- Limitations stated
