# Blameless RCA report template

Complete after response is stable and use the customer's approved problem-management system. State scope and confidence; distinguish known from inferred. Do not include personal blame, credentials, tokens, or unapproved customer evidence.

## Summary

- Incident / problem ID and customer-approved title:
- Incident date and review date (UTC):
- Authors / reviewers / customer approval:
- Executive summary (impact, duration, current state):

## Customer impact

- Services and business processes affected:
- Population, locations, and duration (confirmed scope):
- Data/security impact and confidence; unknowns explicitly listed:
- Workarounds and customer impact:
- SLA/service credit assessment owner (per contract):

## What happened

Provide a factual timeline linked to the incident record. Separate trigger, detection, escalation, containment, recovery, and verification. Cite source records and timestamps; avoid unsupported vendor attribution.

## Causal analysis

- **Trigger:** What event immediately preceded the failure or compromise?
- **Technical cause:** What mechanism allowed the impact to occur?
- **Contributing conditions:** Which design, configuration, process, dependency, monitoring, or workload conditions increased likelihood or impact?
- **Detection:** What signals were available? When were they noticed? What gaps or noise affected detection?
- **Response:** What helped or delayed containment and recovery? Include authorization and communication constraints.
- **Counterfactual:** What control or change would likely have reduced likelihood, duration, or scope?
- **Confidence and alternatives:** What remains uncertain? Which hypotheses were rejected, and why?

Use causal chains and system conditions. “Human error” is not a complete root cause; describe context, control design, feedback, workload, and safeguards.

## Response assessment

- Actions that reduced risk or restored service:
- Actions that increased risk, delay, or uncertainty:
- Recovery and security verification evidence:
- Residual risks / accepted risks / decision owner:

## Corrective action register

| ID | Action | Category | Priority | Owner | Due date | Verification evidence | Status |
| --- | --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |  |

Actions should be specific, measurable, and tracked in the approved system. Do not close an action based only on intent; attach verification evidence and an approver.

## Approval and distribution

- Customer owner / approval date:
- Security, service, privacy/legal review as applicable:
- Distribution list and secure storage location:
- Redactions applied for any external copy:

This report is a learning artifact, not a legal finding or a substitute for required customer or regulatory reporting.
