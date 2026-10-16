# ITIL 4–aligned incident management rules

This document adapts public, high-level ITIL 4 Incident Management concepts for the MSP operating model in this repository. It is an original practical checklist, not official ITIL guidance, a certification resource, or a replacement for licensed PeopleCert materials. Tailor it to the service contract, customer authority model, applicable law, and the MSP's approved procedures.

ITIL 4 describes Incident Management as minimizing the negative impact of incidents by restoring normal service operation as quickly as possible. The rules below translate that outcome into auditable service desk practices; they do not prescribe universal response or resolution times.

## Operating rules

1. **Recognize and record.** Log an unplanned service interruption or reduction in service quality in the approved ITSM system. Capture a unique ID, reporter/channel, affected service, start/detection times, observed symptoms, and current status. Keep production evidence in approved systems, not this public repository.
2. **Distinguish the work type.** Route user requests through request fulfillment. Record a recurring or underlying cause for problem management. Keep the incident record focused on impact and service restoration, and link related records rather than merging their purposes.
3. **Assess impact and urgency.** Establish affected users, locations, business services, scope, and workarounds. Apply the customer-approved priority matrix consistently; record the rationale and revise priority when evidence changes. Do not invent priority definitions or contractual targets.
4. **Assign accountable coordination.** Name an incident owner; for a significant or multi-team event, designate an incident lead to coordinate technical responders, service owners, suppliers, and customer communications. Record handoffs, decision owners, and dependencies.
5. **Restore service safely.** Investigate proportionately, consider a safe workaround, and restore normal service as promptly as practical. Obtain customer authorization for actions that may affect access, data, security controls, evidence, or business operations. Keep containment and recovery decisions auditable.
6. **Communicate through the agreed channel.** Provide confirmed impact, current actions, known uncertainties, customer decisions needed, and the next update time. Use the customer-update template. Make no unapproved promise about resolution time or service credits.
7. **Verify and resolve.** Confirm service recovery against agreed technical and business checks with the appropriate service owner or customer. Record evidence, residual risk, customer confirmation where required, and the resolution time. Reopen or link a follow-up record if symptoms recur.
8. **Learn and prevent recurrence.** Review significant or recurring incidents. Create or link a problem record when cause investigation or prevention work is needed. Track corrective actions with an owner, due date, priority, measurable completion condition, and verification evidence.
9. **Measure outcomes, then improve.** Choose measures that support service decisions, such as time to acknowledge, restore, recurrence, customer impact, communication cadence, and overdue corrective actions. Define calculation, scope, and data source; review trends and avoid treating a single metric as proof of service quality.

## Suggested incident record minimum

- Incident ID, customer-approved service name, reporter, and timestamps with timezone.
- Confirmed impact, affected scope, urgency, priority, and the reason for the priority.
- Named incident owner/lead, technical owners, customer decision-maker, and handoff history.
- Factual timeline of investigation, decisions, changes, customer updates, and supplier dependencies.
- Workaround, restoration checks, residual risk, and resolution confirmation.
- Links to related change, problem, security, or request records and tracked follow-up actions.

## Major incident coordination

Use the customer's major incident criteria; do not assume a universal threshold. When criteria are met, establish a single coordination channel, name a lead and communication owner, agree the update cadence, track open decisions and dependencies, and involve authorized customer leaders early. Keep technical investigation and business communications coordinated through the incident record. Declare recovery only after the agreed checks pass.

## Source

PeopleCert's [ITIL 4 Practitioner: Incident Management](https://www.peoplecert.org/browse-certifications/it-governance-and-service-management/ITIL-1/itil4-practices-incident-management-3684) describes the practice's focus on minimizing incident impact through swift restoration and covers processes, roles, metrics, and integration with service value streams. Refer to official licensed material for the full ITIL guidance.
