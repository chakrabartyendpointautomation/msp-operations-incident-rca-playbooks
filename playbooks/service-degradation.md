# Widespread endpoint rollout or service degradation

Use when multiple users/devices experience similar impact, particularly after a change, policy rollout, service update, or vendor event. This guide coordinates investigation; it does not authorize changing tenant policy or disabling controls.

## Stabilize and define scope

- Open one parent incident and link affected-user reports, duplicates, change records, and vendor advisories. Name incident lead, technical lead, service owner, and customer decision authority.
- Determine affected population, locations, platforms, network paths, service dependencies, start time, business workflow, and workaround availability.
- Compare impacted and unaffected examples. Capture device/OS/build, enrollment state, policy/config version, error text/code, correlation IDs, timestamps, and network context where authorized.
- Check whether a staged change, certificate/credential expiry, identity policy, service health event, DNS/proxy/routing change, or endpoint update correlates with onset. Correlation is a lead, not proof.
- Check official service health and vendor support channels. Record source, time checked, status, and case number; do not repeat unverified outage claims.

## Identify safe response options

1. Pause further rollout only if the MSP has delegated authority; otherwise request customer approval and record the decision.
2. Consider a reversible, limited pilot pause or ring rollback before broad rollback. Define scope, approver, owner, expected result, and stop criteria.
3. Avoid disabling security baselines, compliance, Conditional Access, encryption, endpoint protection, or network controls as a general workaround. If a control change is necessary, require explicit customer risk acceptance, narrow scope, expiry, compensating control, and restoration plan.
4. Do not reset, unenroll, wipe, or mass-redeploy devices to test a hypothesis. Preserve diagnostic evidence first and validate a fix on representative lab or pilot devices.
5. Coordinate vendor/customer changes in the system of record; avoid concurrent untracked changes.

## Verify recovery

- Select representative affected and unaffected cohorts and measure the same symptoms before and after the approved action.
- Confirm the business workflow with the customer, then verify enrollment/management status, policy health, security control state, and service telemetry.
- Watch for recurrence during an agreed observation window and update the customer at the contractually agreed cadence.
- If impact expands, security posture worsens, or the hypothesis is disproved, stop the current action and re-escalate.

## Closure and learning

Record affected scope, relationship to changes or vendor events as confirmed or uncertain, approved actions and rollback, recovery evidence, residual impact, and linked problem/change records. The RCA should distinguish trigger, underlying system conditions, detection gaps, response contributors, and corrective actions. Do not claim a vendor or change caused the incident without evidence.
