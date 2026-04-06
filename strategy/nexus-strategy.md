# RescueMyWorkday — Operating Doctrine

## Purpose

This document defines how RescueMyWorkday operates: how work is initiated, routed, executed, quality-checked, and closed. It covers all four phases of the ACDR operating model, agent routing by phase, quality standards, and escalation rules.

Every agent in the system operates within this doctrine. When in doubt, refer here.

---

## The ACDR Operating Model

```
ACQUIRE → CONVERT → DELIVER → RETAIN
```

This is not a project methodology — it is the commercial loop. Every deliverable we produce either helps a client attract more leads, convert them faster, deliver a better experience, or keep clients longer. Work that doesn't serve one of these four functions should not be on the list.

---

## Phase Definitions

### ACQUIRE — Visibility, Trust, Lead Capture

**Goal**: Make the client findable, credible, and worth contacting.

**Inputs**: Business details, current website, Google Business Profile, competitor landscape.

**Core work**:
- Website audit and rebuild (RescueMyWebsite wedge)
- Local SEO: on-page optimization, keyword targeting, metadata, schema markup
- Google Business Profile: completion, category optimization, photo cadence, Q&A
- Citation building and NAP consistency
- Trust signals: reviews, testimonials, credentials, before/after evidence
- Lead capture: forms, call tracking, booking widgets above the fold

**Done when**: Site is live, GBP is optimized, structured data validates, contact forms submit to GHL, organic visibility is tracked with a baseline.

**Agent routing**:
- Web Lead → website build and on-page SEO
- Marketing Lead → GBP, citations, content, authority
- QA Lead → site QA, form testing, structured data validation

---

### CONVERT — Speed-to-Lead, Booking, Pipeline

**Goal**: Turn interest into a booked appointment or closed sale as fast as possible.

**Inputs**: GHL sub-account, lead sources, existing follow-up gaps.

**Core work**:
- GHL pipeline setup: stages, automations, notifications
- Speed-to-lead: automated SMS/email within 5 minutes of form submission
- Booking flow: calendar integration, confirmation sequences, reminder automations
- Follow-up sequences: 7–14 day multi-touch for non-booked leads
- Sales scripts and intake form design
- Lead source tracking and attribution

**Done when**: New lead triggers automated follow-up in under 5 minutes, booking confirmation fires, pipeline stages are mapped and tested, test lead has been run end-to-end.

**Agent routing**:
- Automation Lead → GHL pipeline, automations, n8n workflows
- Web Lead → booking widget, form integrations
- QA Lead → test lead execution, automation verification

---

### DELIVER — Implementation, QA, Handoff

**Goal**: Execute all scoped work to a quality standard that doesn't create rework.

**Inputs**: Signed scope, Phase 2 foundation, client assets.

**Core work**:
- Website build: design, copy, mobile, speed, accessibility basics
- Automation build: sequences, workflows, integrations
- Content: service pages, location pages, blog stubs, GMB posts
- Reporting setup: dashboard, baseline metrics capture
- QA: full checklist execution, evidence collection, client preview package
- Handoff: SOP docs, walkthrough Loom, training where needed

**Quality standard**:
- Every deliverable reviewed against checklist before client sees it
- Evidence required: screenshots, Loom walkthroughs, test results
- Default posture: NEEDS WORK. PASS requires evidence, not assertion.
- Maximum 2 revision cycles before escalation

**Done when**: QA checklist is signed, client preview is approved, handoff doc is delivered.

**Agent routing**:
- Web Lead → website, landing pages, design
- Automation Lead → GHL, n8n, integrations
- Marketing Lead → content, GMB posts, on-page copy
- QA Lead → full QA package, evidence, sign-off
- Operations Lead → project coordination, SOP capture

---

### RETAIN — Reviews, Nurture, Reporting, Optimization

**Goal**: Keep the client, generate evidence of value, and find the next improvement.

**Inputs**: Live client, baseline metrics, GHL data, review velocity.

**Core work**:
- Monthly reporting: traffic, leads, conversions, pipeline activity
- Review generation: post-service automated requests, monitoring, responses
- Nurture sequences: past-lead re-engagement, referral campaigns
- Recurring optimization: site speed, content updates, GBP post cadence
- SOP updates: capture what's working, update playbooks
- Upsell identification: flag clients ready for next-phase work

**Done when**: Client is on a recurring reporting cadence, review velocity is positive, next optimization cycle is scoped.

**Agent routing**:
- Support Lead → review management, nurture, client communication
- Marketing Lead → reporting, content updates, authority maintenance
- Automation Lead → nurture sequence optimization
- Operations Lead → SOP capture, recurring task management

---

## Quality Standards

### Evidence Requirements

| Deliverable | Required Evidence |
|------------|------------------|
| Website launch | Lighthouse scores (mobile + desktop), form submission screenshot, mobile view screenshot |
| GHL pipeline | Test lead screenshot showing all stages triggered, automation log |
| SEO optimization | Before/after metadata, schema validation tool screenshot, GBP completeness score |
| Review automation | Test send confirmation, GHL automation log |
| Reporting | Dashboard screenshot, data source verification |

### QA Gate Criteria

A deliverable **PASSES** when:
- All checklist items are checked with evidence
- No critical issues remain open
- Client-facing content has been proofread
- Mobile and desktop have been verified
- All integrations have been tested with real test data

A deliverable **NEEDS WORK** when:
- Any checklist item lacks evidence
- Any critical issue is open
- Forms, automations, or integrations have not been tested end-to-end
- Content has obvious errors

### Revision Limits

- Max 2 revision cycles per deliverable
- After cycle 2, escalate to lead with: original brief, revision history, current blockers
- Lead decides: scope adjustment, reassignment, or client conversation

---

## Agent Routing by Phase

| Phase | Lead Agent | Supporting Agents | QA Agent |
|-------|-----------|-------------------|---------|
| Phase 0: Discovery | Strategy Lead | Marketing Lead, Web Lead | — |
| Phase 1: Strategy | Strategy Lead | Operations Lead | — |
| Phase 2: Foundation | Automation Lead | Web Lead | Operations Lead |
| Phase 3: Build | Web Lead / Automation Lead | Marketing Lead | QA Lead |
| Phase 4: QA | QA Lead | Web Lead, Automation Lead | — |
| Phase 5: Launch | Operations Lead | Web Lead, Automation Lead | QA Lead |
| Phase 6: Operate | Support Lead | Marketing Lead, Automation Lead | Operations Lead |

---

## Escalation Rules

**Escalate immediately when**:
- Client is threatening churn or has gone silent after a complaint
- A live automation is firing incorrectly to real leads
- A site is down or broken post-launch
- A deliverable has been in revision cycle 3 or beyond

**Escalation package must include**:
1. What the issue is (one sentence)
2. When it started
3. What has already been tried
4. What the client has been told (if anything)
5. Recommended resolution path

**Resolution SLAs**:
- Client escalation (churn risk): acknowledge within 2 hours, resolution plan within 24 hours
- Live automation error: fix or disable within 1 hour
- Site down: acknowledge within 30 minutes, restore within 2 hours
- Stalled deliverable: lead review within 24 hours

---

## Reusable Asset Doctrine

Every engagement should produce reusable outputs:
- GHL snapshot (exportable pipeline + automations)
- Website template or component library additions
- SOP doc for any new process executed
- Checklist updates if gaps were found
- Content templates for vertical (healthcare vs. local service)

Reusable assets reduce delivery time on future engagements. Capturing them is not overhead — it is how the business scales without proportional headcount growth.

---

## Deployment Modes

| Mode | Phases | Agents | Timeline |
|------|--------|--------|----------|
| **Full Engagement** | 0–6 | All divisions | 6–10 weeks |
| **Build Sprint** | 2–4 | Web, Automation, QA | 2–3 weeks |
| **Micro Task** | Single phase | 1–3 agents | 1–5 days |

**Full Engagement**: New client, start to finish. Discovery through first 30 days of Operate.

**Build Sprint**: Scoped deliverable for an existing client or a client with known requirements. Skip discovery if brief is already locked.

**Micro Task**: Single output — SEO audit, GBP fix, one automation, content batch. Activate only the agents needed. Still requires QA sign-off before delivery.

---

## Business Rules (Non-Negotiable)

1. Lowest total cost of good work beats cheapest output. Rework is not free.
2. Good enough and live beats perfect and stalled — but only after quality gates clear.
3. Every role must serve acquisition, conversion, delivery, retention, compliance, or reusable systems.
4. Specialists execute. Leads prioritize, coordinate, inspect, and escalate.
5. No deliverable ships to a client without QA sign-off and evidence.
6. Client communication is owned by the Operations or Support Lead — specialists do not communicate directly with clients unless briefed to do so.
