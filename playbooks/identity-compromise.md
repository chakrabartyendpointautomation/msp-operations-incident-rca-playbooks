# Suspected identity compromise response

Use this playbook when credible signals suggest a customer identity or privileged account may be compromised. It is a coordination guide, not an automated containment tool. Follow the customer's incident plan, platform guidance, and delegated authority.

## Trigger and immediate coordination

- Signals may include an unexpected sign-in or MFA change, suspicious inbox rule or OAuth consent, anomalous travel corroborated by other evidence, user-reported phishing, or unauthorized privileged action. A single anomaly is not proof of compromise.
- Open a security incident record; assign incident lead and technical lead; notify the customer's designated security contact using an approved channel.
- Confirm affected tenant, identities, roles, services, time window, signal source, confidence, and current business impact. Check whether the reporting or collaboration account itself may be affected; use the agreed out-of-band channel if needed.
- Preserve alert and audit references, sign-in context, message headers or URLs where applicable, timestamps/timezone, and custody notes in approved evidence storage. Never paste tokens, passwords, mailbox content, or sensitive evidence into this public repository.

## Scope and analysis

1. Correlate identity-provider sign-in and audit events with endpoint, email, SaaS, and help-desk context where available and authorized.
2. Determine whether the account is standard or privileged, whether MFA methods or recovery details changed, whether consent or credentials were added, and what resources/actions may have been accessed.
3. Identify related accounts, sessions, devices, applications, mail rules, forwarding, and privilege changes. Record what has not yet been checked.
4. Contact the user through a known-good channel; do not rely on the potentially compromised session.
5. Maintain a hypothesis table: observation, source, timestamp, confidence, alternative explanation, and next check.

## Containment decisions

Containment can disrupt access or destroy volatile evidence. The customer's authorized incident authority must approve actions where required. The security lead should consider evidence preservation, persistence risk, operational impact, and rollback.

Potential actions for authorized responders, chosen for the case rather than executed automatically:

- Revoke active sessions/refresh tokens and block or temporarily disable the affected identity.
- Reset credentials through a verified secure process; revoke or re-register MFA methods if compromise is supported.
- Remove unauthorized OAuth grants, forwarding rules, authentication methods, or role assignments after capturing relevant evidence.
- Restrict affected devices or applications using customer-approved controls.
- Protect dependent break-glass and service accounts; do not indiscriminately rotate unrelated secrets.

For each action record target, rationale, approver, executor, exact time, result, and recovery path. Avoid using the affected identity to perform response actions.

## Eradication and recovery

- Verify attacker access paths and persistence have been removed with evidence from relevant audit sources.
- Restore minimum required access only after credentials and recovery methods are trusted and the customer validates business need.
- Review privileged role assignments, MFA registration, OAuth consent, mailbox rules, device status, and relevant sign-in activity for a defined observation period.
- Ask the customer owner to confirm service restoration and user communication. Maintain heightened monitoring and define criteria for re-escalation.

## Closure and RCA inputs

Document confirmed scope, unknowns, customer impact, response decisions, evidence sources, containment/recovery verification, related tickets/vendor cases, and follow-up owners. Do not claim data was not accessed unless evidence supports that conclusion. Route privacy, contractual, regulatory, insurer, and law-enforcement decisions to the customer's designated advisers.
