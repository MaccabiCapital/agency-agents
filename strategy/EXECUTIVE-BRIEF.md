# RescueMyWorkday — Executive Operating Brief

## Company at a Glance

RescueMyWorkday is an AI-assisted operating company serving small service businesses — primarily healthcare practices and local-service operators. The public-facing acquisition wedge is **RescueMyWebsite**: fix the website, fix the funnel, fix the follow-up. The full operating model extends beyond websites into every revenue-critical system a small service business runs.

**Core problem set**: weak online presence, missed leads, poor follow-up, booking friction, no repeatable delivery systems.

---

## The Operating Model: Acquire → Convert → Deliver → Retain

Every client engagement maps to one or more phases of the ACDR loop:

| Phase | What We Fix | Key Outputs |
|-------|------------|-------------|
| **Acquire** | Website, local SEO, Google Business Profile, trust signals, lead capture | Live site, GBP optimized, structured data, review presence |
| **Convert** | Speed-to-lead, follow-up automations, booking flows, sales pipelines | GHL pipeline, booking widget, automated nurture sequences |
| **Deliver** | Implementation, QA, automation, reporting, handoff | QA-signed deliverables, SOPs, evidence packages, client preview |
| **Retain** | Review generation, nurture campaigns, recurring reporting, optimization | Monthly reports, review velocity, upsell touchpoints, SOP updates |

The loop is continuous. Retained clients re-enter Acquire and Convert with improvements as data accumulates.

---

## Agent Division Structure

| Division | Primary ACDR Role | Key Responsibilities |
|----------|------------------|---------------------|
| **Strategy** | All phases | Coordination, playbooks, doctrine, QA gates |
| **Marketing** | Acquire, Retain | SEO, content, GBP, authority campaigns, nurture |
| **Web / Design** | Acquire, Deliver | Website builds, landing pages, brand, visual QA |
| **Automation** | Convert, Deliver | GHL config, n8n workflows, pipeline setup, integrations |
| **QA** | Deliver | Evidence collection, testing, client preview packages |
| **Operations** | Deliver, Retain | Project coordination, reporting, SOP capture |
| **Support** | Retain | Client communication, escalation handling, review management |

---

## Quality Gates

Quality gates apply at every phase transition. No phase advances without a signed-off handoff.

| Gate | Trigger | Requirement |
|------|---------|-------------|
| Discovery → Strategy | Audit complete | Audit doc signed, gaps identified |
| Strategy → Foundation | Scope agreed | Signed scope, GHL sub-account created |
| Foundation → Build | Infra ready | Domain/hosting live, GHL pipeline configured |
| Build → QA | Build complete | All deliverables submitted with evidence |
| QA → Launch | QA pass | QA checklist signed, client preview approved |
| Launch → Operate | Go-live confirmed | DNS live, monitoring active, handoff doc sent |

**QA Standard**: Default posture is NEEDS WORK. Evidence (screenshots, test results, Loom walkthroughs) required for any PASS. Maximum 2 revision cycles before escalation to lead.

---

## Deployment Modes

| Mode | Scope | Timeline | Typical Use |
|------|-------|----------|-------------|
| **Full Engagement** | All 7 phases | 6–10 weeks | New client: audit → launch → first 30 days retained |
| **Build Sprint** | Phases 2–4 | 2–3 weeks | Existing client adding pipeline or automation |
| **Micro Task** | Single deliverable | 1–5 days | SEO audit, GBP fix, single automation, content batch |

---

## Business Rules

- Lowest total cost of good work beats cheapest output. Weak output that creates rework is not acceptable.
- Good enough and live beats perfect and stalled — but only when quality gates have been cleared.
- Every active role must support acquisition, conversion, delivery, retention, compliance, or reusable systems.
- Reusable SOPs, templates, GHL snapshots, checklists, and playbooks are valuable outputs, not overhead.
- Specialists execute. Leads prioritize, coordinate, inspect, and escalate.

---

## File Structure

```
strategy/
├── EXECUTIVE-BRIEF.md              ← You are here
├── QUICKSTART.md                   ← 5-minute activation guide
├── nexus-strategy.md               ← RescueMyWorkday Operating Doctrine
├── playbooks/
│   ├── phase-0-discovery.md        ← Client discovery & audit
│   ├── phase-1-strategy.md         ← Strategy & recommendations
│   ├── phase-2-foundation.md       ← GHL setup, infra, pipeline config
│   ├── phase-3-build.md            ← Website, automations, content
│   ├── phase-4-hardening.md        ← QA, testing, client preview
│   ├── phase-5-launch.md           ← Go-live, DNS, handoff
│   └── phase-6-operate.md          ← Reviews, reporting, retention
├── coordination/
│   ├── agent-activation-prompts.md ← Ready-to-use activation prompts
│   └── handoff-templates.md        ← Standardized handoff formats
└── runbooks/
    ├── scenario-new-client-website.md    ← End-to-end website build
    ├── scenario-client-escalation.md     ← Client issue / escalation handling
    ├── scenario-seo-authority-campaign.md← Local SEO authority push
    └── scenario-pipeline-buildout.md     ← GHL pipeline from scratch
```
