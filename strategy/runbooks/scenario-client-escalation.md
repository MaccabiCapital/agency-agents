# Runbook: Client Escalation

**Scenario**: A client has raised a complaint, expressed dissatisfaction, threatened to cancel, gone silent after an issue, or a live error is impacting their business.

**Response time**: Acknowledge within 2 hours for HIGH severity. Resolution plan within 24 hours.
**Owner**: Operations Lead or Support Lead — specialists do not communicate directly with clients during escalations.

---

## When to Use This Runbook

- Client sends an angry or frustrated message
- Client mentions cancelling, stopping payment, or going with a competitor
- Client reports a live issue (site down, wrong automation firing, form not working)
- Client has not responded to 3+ outreach attempts after a known issue
- Internal team identifies a live error before the client does (get ahead of it)

---

## Severity Classification

| Severity | Definition | SLA |
|----------|-----------|-----|
| HIGH | Live error affecting client's leads / revenue. Churn imminent. | Acknowledge 2 hrs, resolve 24 hrs |
| MEDIUM | Client complaint without live impact. Dissatisfied but not threatening churn. | Acknowledge 4 hrs, resolution plan 48 hrs |
| LOW | Minor friction, slow response complaint, feature request framed as complaint. | Acknowledge same day, resolve in next sprint |

---

## Escalation Steps

**Step 1: Assess and classify** (Operations Lead — within 30 min of escalation being flagged)
- Read the client communication in full
- Check GHL for any error logs or automation failures
- Determine severity: HIGH / MEDIUM / LOW

**Step 2: Acknowledge the client** (before anything is fixed)
- Send a brief, calm acknowledgment: "We're looking into this now and will have an update by [time]."
- Do not promise a specific fix before you know the cause.
- Do not assign blame to a team member in client communication.

**Step 3: Diagnose the root cause**
- Pull the relevant agent or lead to identify what went wrong
- Document: what happened, when, what the impact was
- Separate: is this a build error (our fault), a scope gap (not our fault), or a client misunderstanding?

**Step 4: Fix or contain** (if live error)
- If an automation is firing incorrectly: pause it immediately, then fix
- If the site is down: triage with Web Lead, restore from backup if needed
- If a form is broken: disable form page, redirect to phone number, fix and re-test

**Step 5: Client communication** (after diagnosis)
Use clear, accountable language:
- Explain what happened briefly
- Explain what we did or are doing to fix it
- Give a realistic resolution timeline
- If it was our error: own it, offer a concrete remedy (extra work, credit, call)

**Step 6: Complete escalation package**
Fill out Template 4 (Client Escalation Handoff) from handoff-templates.md and log it.

---

## After Resolution

- [ ] Root cause documented in incident log
- [ ] SOP updated if this was a repeatable failure pattern
- [ ] Client confirmed satisfied (response or call)
- [ ] Operations Lead reviews: does this indicate a systemic issue?
- [ ] If client retention is at risk: flag to Strategy Lead for account review
