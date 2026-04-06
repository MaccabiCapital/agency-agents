# Phase 3 — Build

**Objective**: Execute all scoped deliverables — website, automations, content, integrations. Quality loops run throughout. Nothing goes to QA that hasn't been self-reviewed first.

**Agents**: Web Lead (website), Automation Lead (GHL/n8n), Marketing Lead (content/SEO), QA Lead (internal loops)
**Duration**: 1–2 weeks (typical full build)
**Output**: All deliverables complete, staged, and ready for formal QA

---

## Inputs Required Before Starting

- [ ] Foundation summary from Phase 2 (staging URL, GHL access, all assets)
- [ ] Signed scope with page list and automation list
- [ ] Client brand assets (logo, colors, photos, or note what's missing)
- [ ] Any copy from client, or copy-writing is in scope

---

## Track 1: Website Build (Web Lead)

Run in parallel with automation build where possible.

**Structure**
- [ ] Set up page structure in CMS/builder matching approved page list
- [ ] Apply brand: colors, fonts, logo, favicon
- [ ] Build homepage: hero with primary CTA, trust signals, services overview, contact section
- [ ] Build service pages: one per core service, keyword-optimized, local signals
- [ ] Build contact / booking page: form connected to GHL, phone, address, map embed
- [ ] Build about page: team, credentials, story
- [ ] Add footer: NAP, hours, quick links, legal (privacy policy, terms)

**On-Page SEO (each page)**
- [ ] Unique title tag: `[Keyword] | [Business Name] | [City]` format
- [ ] Meta description: compelling, 150–160 chars
- [ ] H1 present and keyword-relevant
- [ ] Image alt tags filled
- [ ] Internal links between service pages
- [ ] LocalBusiness schema markup on homepage; Service schema on service pages

**Performance**
- [ ] Images compressed before upload (WebP preferred)
- [ ] Lazy loading on below-fold images
- [ ] Minimize render-blocking scripts
- [ ] Target: Lighthouse mobile 80+ before submitting to QA

**Internal QA loop before submitting**
- [ ] View every page on mobile (375px) and desktop
- [ ] Click every link — confirm no 404s
- [ ] Submit test form — confirm GHL pipeline entry created
- [ ] Run Lighthouse — record score

---

## Track 2: Automation Build (Automation Lead)

**Speed-to-Lead**
- [ ] Trigger: new form submission in GHL
- [ ] Action 1: SMS to lead within 5 minutes — confirm send
- [ ] Action 2: Email to lead within 5 minutes — confirm send
- [ ] Action 3: Internal notification to business owner — confirm send

**Booking Sequence**
- [ ] Confirmation SMS + email fires on booking creation
- [ ] Reminder 24 hours before appointment
- [ ] Reminder 1 hour before appointment (SMS)
- [ ] Post-appointment: review request fires 2–4 hours after appointment end

**Nurture Sequence (for non-booked leads)**
- [ ] Day 1: follow-up SMS
- [ ] Day 3: follow-up email with social proof
- [ ] Day 7: check-in SMS
- [ ] Day 14: final email — keep door open

**Internal QA loop before submitting**
- [ ] Run a test record through every automation — screenshot each step
- [ ] Confirm all messages deliver (check GHL activity log)
- [ ] Confirm pipeline stage changes fire correctly
- [ ] Confirm no automation fires on wrong trigger (test negative cases)

---

## Track 3: Content & SEO (Marketing Lead)

- [ ] Write or finalize copy for all pages (if in scope)
- [ ] Keyword-map each service page to primary + secondary terms
- [ ] Write or update GBP description
- [ ] Prepare first 4 GBP posts (to publish at or after launch)
- [ ] Identify and fix top citation inconsistencies
- [ ] Prepare any blog stubs or location pages in scope

---

## Track 4: Integrations (Automation Lead)

- [ ] Connect calendar to GHL booking widget — test booking creates GHL contact
- [ ] Connect payment processor (if in scope) — test transaction
- [ ] Connect any EHR or practice management system (if in scope)
- [ ] Connect n8n workflows (if applicable) — test webhook triggers

---

## Build → QA Loop

Before submitting to Phase 4 QA:

1. Each track lead completes their internal checklist
2. Web Lead and Automation Lead do a joint smoke test: submit a test lead on the live staging site and trace it through the full GHL pipeline to confirmation message
3. Any failures go back into the build track for fixes — not to QA
4. When smoke test passes: submit Phase 4 QA handoff

---

## Quality Gate: Phase 3 → Phase 4

PASS requires:
- [ ] All scoped pages built and accessible on staging URL
- [ ] All scoped automations built and tested with real test records
- [ ] Lighthouse mobile score recorded (80+ target)
- [ ] All forms tested end-to-end (form → GHL entry → automation trigger)
- [ ] No broken links on the site
- [ ] Content complete — no placeholder text remaining
- [ ] Internal QA loop complete (each track lead has self-reviewed)
- [ ] QA handoff doc submitted with staged URL, GHL access, test credentials
