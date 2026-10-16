# Incident lifecycle and MSP operating model

## Purpose and boundary

Use this as a coordination framework, then follow the customer's approved incident plan, contract, and service-specific procedures. The MSP supports the response within its authorized scope; the customer retains decisions reserved to its incident commander, business owner, privacy/legal team, and service owner. Escalate when authority, impact, or reporting duties are unclear.

## Roles

- **Incident lead:** owns the record, severity review, next actions, handoffs, and update schedule.
- **Technical lead:** coordinates investigation and technical responders; records evidence and confidence level.
- **Customer incident authority:** approves customer-impacting containment and restoration decisions where required by contract.
- **Communications owner:** sends approved updates through agreed channels and maintains recipients.
- **Service owner / vendor liaison:** checks dependencies, change history, advisories, vendor cases, and recovery dependencies.
- **Scribe:** records event time, decision, decision-maker, action owner, result, and source.

One person may hold several roles in a small team, but the incident lead and customer decision authority must be explicit. Maintain an out-of-band contact path if primary identity or collaboration services may be affected.

## Intake and triage

1. Open an incident record in the approved service management system. Assign a unique ticket, customer, reporter, affected service, and incident lead.
2. Capture report time, observed start time (if known), symptoms, scope, business impact, affected locations/users/devices, recent changes, and evidence sources.
3. Distinguish confirmed observations from hypotheses. Preserve original timestamps and timezone; record collection method and custodian for material evidence.
4. Check related alerts, incidents, maintenance, vendor advisories, known changes, and customer reports. Do not close as duplicate until linkage and ownership are recorded.
5. Assign severity using the customer's contractual matrix. Reassess when scope or impact changes; record why priority changed.

## Suggested impact rubric (map to customer contract)

| Signal | Lower impact | Higher impact |
| --- | --- | --- |
| Reach | Isolated user or device | Multiple teams, locations, or tenants |
| Business service | Workaround available | Critical workflow unavailable or materially degraded |
| Security | Suspicion with no confirmed compromise | Credible/confirmed access, data exposure, or active spread |
| Duration | Brief with stable recovery | Ongoing, recurring, or recovery uncertain |
| Safety/regulatory | No known exposure | Potential sensitive data, safety, or reporting implications |

This is illustrative and does not define contractual priority, notification deadlines, or regulatory conclusions. Use the signed customer agreement and designated decision-makers.

## Response stages

### Prepare

Confirm on-call coverage, escalation tree, access approvals, service dependencies, communication preferences, evidence storage, and known containment options before an incident occurs. Tabletop scenarios should include authorization, out-of-band communication, and recovery decisions.

### Detect and analyze

Build a bounded scope and working timeline. Identify affected identities, endpoints, services, tenants, locations, and time window. Validate signal quality; seek corroboration from independent telemetry. State confidence and unknowns. Request vendor support when service boundaries or telemetry require it.

### Contain

Choose actions based on threat or outage risk, reversibility, evidence impact, and business disruption. Confirm who may approve each action. Record action, target, reason, approver, execution owner, time, result, and rollback. For suspected compromise, do not destroy evidence without security lead direction.

### Eradicate and recover

Remove the verified cause, rotate/revoke exposed access where authorized, restore from trusted sources, and re-enable service in a controlled sequence. Verify security posture and business function with the customer. Watch for recurrence and preserve relevant evidence. Do not declare recovery solely because an alert cleared.

### Close and learn

Confirm customer acceptance or document remaining limitations, link vendor/root incidents, record known scope and unresolved unknowns, identify corrective actions, and schedule the retrospective. Close only when incident lead and customer process criteria are met.

## Customer communication

Agree on severity-specific update intervals per contract. Each update should state incident ID, current impact, confirmed facts, actions completed, active work, decisions needed, next update time, and safe workaround. If there is no new information, send a brief status as agreed. Avoid speculation, unapproved attribution, or unsupported assurance that data was not accessed.

Use an approved secure channel. Confirm distribution lists and alternates. Sensitive evidence, credentials, personal data, and detailed indicators go only to authorized recipients in the approved system.

## Handoffs and escalation

A handoff includes severity and rationale, timeline link, known facts and confidence, affected scope, actions/approvals/results, outstanding decisions, next update deadline, active vendor cases, and named next owner. The receiving owner acknowledges before the current owner disengages whenever practical.

Escalate to customer incident authority, security/privacy/legal contacts, service owner, or vendor according to contract and incident plan. Do not decide legal reportability or promise regulatory timelines on their behalf.

## Service improvement measures

Use agreed definitions and authorized aggregate data: time to acknowledge, assign lead, first customer update, contain, recovery duration, recurrence rate, action completion, and evidence completeness. Explain clock start/stop rules and exclusions. Do not reward premature closure or penalize staff for raising uncertainty.
