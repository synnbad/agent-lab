# Assessment Data Threat Model

## System Or Workflow Being Modeled
Assessment Data Threat Model

## Assets At Risk
- Student data
- Staff data
- Patron/user data
- Small group re-identification

## Trust Boundaries
External content, user-provided files, Integration Adapters, public repositories, deployment systems, and stakeholder-facing artifacts.

## Possible Attackers Or Failure Sources
Malicious external content, accidental user error, over-permissioned tools, stale assumptions, misconfigured deployments, and unclear ownership.

## Abuse Cases
- Student data
- Staff data
- Patron/user data
- Small group re-identification
- Overclaiming impact
- Misleading metrics
- Unsafe dashboards
- Unapproved data sharing
- Weak aggregation
- Stakeholder misinterpretation

## Likely Failure Modes
- Unapproved action or publication
- Sensitive data exposure
- Unsupported claims or incorrect assumptions
- Weak review before handoff

## Preventive Controls
- Prefer aggregated, anonymized, or redacted data
- Define metrics before reporting
- Review privacy risk before dashboarding
- Separate activity counts from outcomes
- State limitations clearly

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
