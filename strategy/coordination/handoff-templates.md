# Handoff Templates

Standardized formats for transferring work between agents, phases, and client-facing delivery. Fill every field — never hand off without context.

---

## Template 1: Phase Gate Handoff

Use at every phase transition. The receiving agent must confirm receipt before proceeding.

```
PHASE GATE HANDOFF
──────────────────
From: [AGENT / LEAD NAME]
To: [RECEIVING AGENT / LEAD NAME]
Date: [DATE]
Client: [CLIENT NAME]
Phase completing: [Phase X — Name]
Phase starting: [Phase X+1 — Name]

WHAT WAS COMPLETED
- [Deliverable 1] — Status: DONE / PARTIAL (note if partial)
- [Deliverable 2]
- [Deliverable 3]

QUALITY GATE STATUS
- QA checklist: PASSED / NOT REQUIRED / PENDING
- Evidence location: [link or file path]
- Outstanding issues: [list or "none"]

CONTEXT FOR NEXT PHASE
- Key decisions made: [summarize]
- Client preferences noted: [tone, colors, process preferences, sensitivities]
- Access/credentials needed: [GHL login, domain registrar, etc.]
- Hard deadlines: [client launch date or "none set"]

BLOCKERS / WATCH ITEMS
- [Any known risks or items to monitor]

Receiving agent: confirm receipt and surface any questions before starting.
```

---

## Template 2: QA Pass / Fail

Use when QA Lead completes a review of any deliverable.

```
QA RESULT
─────────
Agent: [QA LEAD NAME]
Date: [DATE]
Client: [CLIENT NAME]
Deliverable: [website / automation / form / content / full package]

VERDICT: PASS ✓ / NEEDS WORK ✗

CHECKLIST RESULTS
- [ ] Mobile display: PASS / FAIL — [note]
- [ ] Desktop display: PASS / FAIL — [note]
- [ ] All forms submit to GHL: PASS / FAIL — [note]
- [ ] Automations tested end-to-end: PASS / FAIL — [note]
- [ ] Lighthouse mobile 80+: [SCORE] — PASS / FAIL
- [ ] No broken links or missing images: PASS / FAIL — [note]
- [ ] Content proofread: PASS / FAIL — [note]
- [ ] Schema validates: PASS / FAIL — [note]
- [ ] Business info correct throughout: PASS / FAIL — [note]

EVIDENCE
- Screenshots: [links or "attached"]
- Lighthouse report: [link or score]
- Test automation log: [link or "attached"]

REQUIRED FIXES (if NEEDS WORK)
1. [Fix description] — Owner: [agent] — Priority: HIGH / MED
2. [Fix description] — Owner: [agent] — Priority: HIGH / MED

Revision cycle: 1 of 2. If cycle 2 fails, escalate to lead.
```

---

## Template 3: Client Preview Handoff

Use when delivering a client-preview package (typically end of Phase 4).

```
CLIENT PREVIEW PACKAGE
──────────────────────
Prepared by: [AGENT NAME]
Date: [DATE]
Client: [CLIENT NAME]

WHAT'S READY FOR REVIEW
- Staged website: [URL]
- Loom walkthrough: [URL]
- GHL pipeline demo: [URL or "included in Loom"]
- Supporting docs: [links]

WHAT WE NEED FROM CLIENT
- [ ] Website content approval
- [ ] Confirm business hours / service areas are correct
- [ ] Approve CTA text and button placement
- [ ] Confirm booking calendar is connected correctly
- [ ] [Other specific item]

REVIEW DEADLINE
Client should respond by: [DATE — typically 48–72 hours]
If no response by deadline: follow up via [phone / email / GHL].

KNOWN ITEMS NOT YET DONE (explain to client)
- [e.g., "We'll add the team photos once you send them"]
- [e.g., "Blog section will go live with the first post in week 2"]

NEXT STEP AFTER APPROVAL
Phase 5 launch. DNS cutover can happen within [timeframe] of approval.
```

---

## Template 4: Client Escalation Handoff

Use when escalating a client issue to a lead or owner.

```
ESCALATION NOTICE
─────────────────
Raised by: [AGENT NAME]
Date/Time: [DATE TIME]
Client: [CLIENT NAME]
Severity: HIGH (churn risk / live error) / MEDIUM (delay / complaint) / LOW (friction)

ISSUE SUMMARY
[One clear paragraph: what happened, when, what the client said or did]

TIMELINE
- [Date]: [Event]
- [Date]: [Event]
- [Date]: [Event]

WHAT HAS BEEN TRIED
- [Action 1] — Result: [outcome]
- [Action 2] — Result: [outcome]

WHAT CLIENT HAS BEEN TOLD
[Quote or summarize the last client communication]

RECOMMENDED RESOLUTION
[Your suggested path: fix, call, scope adjustment, credit, etc.]

DECISION NEEDED FROM LEAD
[Specific question: "Approve X", "Override Y", "Call client now?"]

Escalation SLA: Lead responds within 2 hours for HIGH, 24 hours for MEDIUM.
```

---

## Template 5: Go-Live Handoff (Phase 5 → Phase 6)

Use at launch to transition from delivery to ongoing operations.

```
GO-LIVE HANDOFF
───────────────
From: [DELIVERY LEAD]
To: [OPERATIONS / SUPPORT LEAD]
Date: [DATE]
Client: [CLIENT NAME]

WHAT WENT LIVE TODAY
- Website: [LIVE URL] — DNS propagated: YES / PENDING
- GHL pipeline: ACTIVE — sub-account: [ID/name]
- Automations live: [list]
- Monitoring: [uptime tool or "manual check scheduled"]

ACCESS SUMMARY
- GHL: [login or access method]
- Website hosting: [provider + login location]
- Domain registrar: [provider + login location]
- Google Analytics / Search Console: [access confirmed: YES / NO]
- GBP: [access confirmed: YES / NO]

CLIENT BRIEFED ON
- [ ] How to log into GHL
- [ ] How to check pipeline activity
- [ ] How to respond to review requests
- [ ] Who to contact for support: [contact info]
- [ ] What to expect in month 1: [brief description]

RECURRING TASKS NOW ACTIVE
- Monthly report: [due date each month]
- GBP post cadence: [frequency]
- Review request automation: ACTIVE / PENDING
- [Other recurring item]

OPEN ITEMS (hand these off explicitly)
- [Item] — Owner: [name] — Due: [date]
```
