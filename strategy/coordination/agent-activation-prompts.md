# Agent Activation Prompts

Ready-to-use prompts for activating agents in common RescueMyWorkday scenarios. Copy, fill in the brackets, and send.

---

## Full Engagement — New Client Onboarding

```
Activate Strategy Lead for full client engagement.

Client: [CLIENT NAME]
Vertical: [healthcare practice / dental / chiro / med spa / home services / other]
URL: [CURRENT WEBSITE OR "none"]
Known issues: [describe or "unknown — run full audit"]

Execute full engagement sequence: Phase 0 → 1 → 2 → 3 → 4 → 5 → 6.
Quality gate required between every phase.
Surface blockers immediately — do not hold issues until end of phase.
```

---

## Phase 0 — Discovery Audit

```
Activate Marketing Lead + Web Lead for discovery audit.

Client: [CLIENT NAME] | URL: [URL]
Deliver audit covering:
- Website: speed, mobile, UX, trust signals, CTAs, technical SEO
- Local SEO: GBP completeness, citation consistency, keyword gaps
- Pipeline: current lead follow-up process (if known)
- Competitive snapshot: top 3 competitors in local search

Output: Discovery audit doc with prioritized findings and quick wins flagged.
```

---

## Phase 2 — Foundation Setup

```
Activate Automation Lead for GHL foundation setup.

Client: [CLIENT NAME]
GHL sub-account: [create new / existing ID: ___]
Domain: [DOMAIN] | Hosting: [provider or "TBD"]

Setup tasks:
- Create/configure sub-account
- Import applicable snapshot or build pipeline from scratch
- Connect domain, configure email/SMS sending
- Set up lead pipeline stages: [New Lead / Contacted / Booked / Won / Lost]
- Configure basic speed-to-lead automation (5-min SMS + email)

Deliver: GHL access confirmation, pipeline screenshot, test lead result.
```

---

## Phase 3 — Website Build

```
Activate Web Lead for website build.

Client: [CLIENT NAME] | Vertical: [vertical]
Reference: [style references or "none"] | Colors: [brand colors or "derive from logo"]
Pages needed: Home, About, Services ([list]), Contact, [others]

Requirements:
- Mobile-first, fast-loading (target Lighthouse 85+)
- Clear CTA above fold (call / book / contact)
- Trust signals: reviews, credentials, photos
- Forms connected to GHL pipeline
- Local SEO: on-page, schema markup, location data

Deliver: Staged URL, Lighthouse scores, mobile screenshot, QA checklist submitted.
```

---

## Phase 3 — Automation Build

```
Activate Automation Lead for automation build.

Client: [CLIENT NAME]
Automations to build:
- [ ] Speed-to-lead (form → SMS + email within 5 min)
- [ ] Booking confirmation + reminder sequence
- [ ] No-show follow-up
- [ ] Post-service review request
- [ ] Long-term nurture (14-day sequence for non-converted leads)
- [ ] [OTHER: describe]

Platform: GHL (primary) | n8n: [yes / no]
Deliver: Each automation tested with a real test record, log screenshot for each.
```

---

## Phase 4 — QA

```
Activate QA Lead for full QA pass.

Client: [CLIENT NAME]
Deliverables to QA: [website / automations / forms / content / all]
Staged URL: [URL] | GHL sub-account: [ID or name]

QA checklist:
- All pages load on mobile + desktop
- All forms submit and trigger correct GHL pipeline entry
- All automations fire correctly on test records
- Lighthouse mobile score 80+
- No broken links, missing images, or placeholder text
- Content proofread (no typos, correct business info)
- Schema markup validates

Deliver: Completed QA checklist with evidence, PASS or NEEDS WORK verdict per item.
```

---

## Phase 6 — Monthly Reporting

```
Activate Support Lead for monthly client report.

Client: [CLIENT NAME] | Reporting month: [MONTH YEAR]
Data sources: GHL, Google Analytics / Search Console, GBP Insights

Report should cover:
- Lead volume: total, by source
- Pipeline activity: new, contacted, booked, won
- Website: sessions, top pages, organic vs. paid
- GBP: views, calls, direction requests
- Reviews: new this month, total count, avg rating
- Priority for next month: [one focus area]

Deliver: Report doc + send to client via [email / GHL / other].
```

---

## Micro Task — SEO Audit Only

```
Activate Marketing Lead for SEO audit.

Client: [CLIENT NAME] | URL: [URL] | Location: [CITY, STATE]
Target keywords: [if known, or "derive from business type and location"]

Audit scope:
- On-page: title tags, H1s, meta descriptions, keyword usage
- Technical: Core Web Vitals, crawlability, mobile
- GBP: completeness, categories, reviews, posts
- Citations: NAP consistency, top directory presence
- Quick wins: list top 5 actions that would move rankings fastest

Deliver: Audit doc, prioritized fix list, estimated impact per fix.
```
