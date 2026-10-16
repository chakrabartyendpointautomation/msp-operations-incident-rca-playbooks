# MSP Operations & Incident RCA Playbooks

Practical, reusable runbooks for managed service provider (MSP) service operations, major incident coordination, customer communication, and blameless root cause analysis. The material is vendor-neutral with examples shaped around endpoint and Microsoft cloud service work.

> **Portfolio status:** These are reference templates and synthetic scenarios. They do not document a real customer incident, employment history, service level agreement, or tested production response. Adapt them to approved contracts, customer contacts, authority boundaries, legal obligations, and tooling before use.

## Why this is a separate project

The portfolio's endpoint remediation and health assessment repositories focus on technical endpoint checks and device remediation; the Entra, Intune, PKI, and Jamf projects focus on specific platforms. This repository covers the cross-customer service operating model around an incident: intake, severity, ownership, escalation, customer updates, evidence, recovery coordination, and retrospective actions. It does not duplicate device scripts or platform implementation labs.

## Playbook set

- [Incident lifecycle and MSP operating model](docs/operations-model.md): roles, intake, severity, handoffs, evidence, communications, and closure.
- [Identity compromise response](playbooks/identity-compromise.md): safe triage and coordinated containment for a suspected user/admin account takeover.
- [Endpoint rollout / service degradation](playbooks/service-degradation.md): triage for a change-associated widespread endpoint or cloud service impact.
- [Incident record template](templates/incident-record.md): time-ordered evidence, decisions, and ownership.
- [Customer update template](templates/customer-update.md): concise initial, ongoing, and resolved messages.
- [RCA report template](templates/rca-report.md): impact, causal chain, contributing conditions, and tracked corrective actions.
- [Synthetic scenarios](samples/scenarios.json): fictional examples for tabletop discussion only.

## Operating principles

1. Protect people, customer data, and service availability. Use the least disruptive safe containment and get the authorized customer decision-maker involved when action can affect access, evidence, or business operations.
2. Establish a single incident lead and an auditable timeline. Record facts, uncertainty, decisions, owners, and timestamps in the approved ticketing or incident system.
3. Separate detection, investigation, containment, eradication, recovery, and lessons learned while keeping them coordinated. Use evidence to decide when a phase is complete.
4. Communicate impact and next update time without speculation. Distinguish confirmed facts, working hypotheses, and unknowns.
5. Write blameless RCAs. Explain how system design, process, tooling, workload, and decision context interacted; do not use the retrospective to assign personal fault.
6. Track corrective actions to an owner, due date, priority, verification evidence, and closure decision.

## Start here

1. Review docs/operations-model.md and confirm role boundaries with the customer.
2. Open a record from templates/incident-record.md in the approved ticketing system. Do not copy real personal data or secrets into this public repository.
3. Select the closest playbook, verify that it applies, and make a situation-specific plan with the customer incident authority.
4. Use templates/customer-update.md to coordinate communication cadence and templates/rca-report.md after the incident is stable.
5. Store production evidence only in approved customer systems under the relevant retention and access policy.

## Severity and response targets

This repository provides impact-based severity examples, not contractual response or restoration targets. Each MSP must map its own priority levels to signed service agreements, customer business impact, coverage hours, on-call capability, and applicable reporting requirements. Do not promise a resolution time before scope and dependencies are understood.

## Safety boundaries

- This repository is documentation-first; it contains no scripts that disable accounts, isolate endpoints, change Conditional Access, or alter customer services.
- Never test containment or recovery actions on a customer environment without explicit authority, an approved change/incident record, and a rollback or recovery plan.
- Preserve evidence and coordinate legal, privacy, security, insurer, and law-enforcement notifications through the organization's designated decision-makers. Notification timelines and duties depend on contract and jurisdiction; do not infer them from this playbook.
- Use least-privilege, customer-approved access. Avoid collecting more personal data or telemetry than needed.
- Scenarios contain fictional names, times, services, and impact descriptions.

## Validation status

No tabletop, customer exercise, technical simulation, or production incident was performed for this repository. These templates have not been approved as an operational policy or contractual SLA. Review and test locally with authorized stakeholders before adopting them.

## References

- [NIST SP 800-61 Rev. 3, final (April 2025)](https://csrc.nist.gov/pubs/sp/800/61/r3/final): incident response recommendations integrated with CSF 2.0 risk management.
- [CISA Federal Government Cybersecurity Incident and Vulnerability Response Playbooks](https://www.cisa.gov/resources-tools/resources/federal-government-cybersecurity-incident-and-vulnerability-response-playbooks): a public example of structured incident response; federal-specific instructions do not automatically apply to MSP customers.
- [Microsoft incident response planning](https://learn.microsoft.com/en-us/security/operations/incident-response-planning): preparation and tabletop exercise guidance.
- [Microsoft Defender incident workflow planning](https://learn.microsoft.com/en-us/unified-secops/plan-incident-response): platform-specific workflow context.

## License

MIT. See LICENSE.
