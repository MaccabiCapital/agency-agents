# Runbook: Pipeline Buildout

**Scenario**: Build a complete GHL lead pipeline and automation stack for a client — from first contact through booking, follow-up, and review generation.

**Typical timeline**: 1–2 weeks
**Agents**: Automation Lead (lead), Web Lead (form integration), QA Lead (testing)
**Deployment mode**: Build Sprint (Phases 2–4) or Micro Task if GHL sub-account already exists

---

## When to Use This Runbook

- New client with no CRM or automation in place
- Client using a different CRM being migrated to GHL
- Existing client adding an automation layer after website launch
- Client has GHL but it's unused or incorrectly configured

---

## Activation Prompt

```
Activate Automation Lead for GHL pipeline buildout.

Client: [CLIENT NAME] | GHL sub-account: [create new / existing ID: ___]
Business type: [healthcare / home services / other]
Lead sources: [website form / GBP calls / paid ads / referrals / all]
Booking platform: [GHL calendar / external — specify]
Automations needed:
- [ ] Speed-to-lead (form → SMS + email within 5 min)
- [ ] Booking confirmation + reminders
- [ ] No-show follow-up
- [ ] Long-term nurture (non-converted leads)
- [ ] Review request (post-appointment)
- [ ] [OTHER: describe]

Deliver: each automation tested with evidence. SOP doc included.
```

---

## Build Sequence

### Stage 1 — Account Setup (if new sub-account)

Follow Phase 2 Foundation playbook for GHL setup. When sub-account is confirmed:
- [ ] Sending verified (test SMS + email received)
- [ ] Pipeline stages configured for this client's sales process
- [ ] Lead source tags configured

### Stage 2 — Pipeline Design

Before building automations, map the client's lead flow:

```
Lead arrives → [source: form / call / referral]
    ↓
Speed-to-lead contact (5 min)
    ↓
Booked? → YES → Confirmation → Reminder(s) → Appointment → Review request
         → NO  → Day 1 follow-up → Day 3 → Day 7 → Day 14 → Archive
```

Adjust for client's actual process. Document the map before building.

### Stage 3 — Build Automations

Build in this order (dependencies):

1. **Speed-to-lead** (highest revenue impact)
   - Trigger: new form submission or GHL contact created
   - Actions: SMS within 5 min, email within 5 min, internal notification
   - Test: submit test form, confirm all three fire within 5 minutes

2. **Booking confirmation**
   - Trigger: appointment created in GHL calendar
   - Actions: SMS confirmation, email confirmation with details + reschedule link
   - Test: create test appointment, confirm both messages received

3. **Appointment reminders**
   - Trigger: appointment date/time approaching
   - Actions: 24-hour SMS, 1-hour SMS
   - Test: create appointment for near-future time, confirm reminders scheduled

4. **Post-appointment review request**
   - Trigger: appointment status changed to "Completed"
   - Wait: 2–4 hours
   - Actions: SMS with Google review link
   - Test: mark test appointment complete, confirm SMS received after wait time

5. **Nurture sequence (non-converted)**
   - Trigger: lead in pipeline for 24 hours without booking
   - Day 1: friendly SMS check-in
   - Day 3: email with testimonial or social proof
   - Day 7: SMS — "still interested?"
   - Day 14: final email — "leaving the door open"
   - Test: create test contact, advance manually through sequence to verify each step

---

### Stage 4 — Form & Website Integration

- [ ] Connect website contact form to GHL (webhook or native integration)
- [ ] Confirm form submission creates correct pipeline opportunity
- [ ] Confirm lead source tag populates correctly
- [ ] Test full path: form submit → GHL contact created → speed-to-lead fires

---

### Stage 5 — QA & Evidence

For each automation, collect:
- [ ] Screenshot of automation workflow in GHL
- [ ] Screenshot of activity log showing test record triggered correctly
- [ ] Screenshot of test SMS/email received (use a real test number/email)
- [ ] Screenshot of pipeline opportunity created with correct stage and source

---

## Deliverables

- [ ] GHL pipeline: configured and live
- [ ] All automations: built, tested, evidence collected
- [ ] SOP doc: 1-page summary of what each automation does, how to test it, and how to turn it off if needed
- [ ] Client handoff: brief Loom walking through GHL — how to view leads, read the pipeline, and see automation activity
- [ ] GHL snapshot exported (for reuse on similar clients)
