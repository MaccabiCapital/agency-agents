# Phase 4 — QA & Hardening

**Objective**: Independent verification of all deliverables before any client sees them. Find and fix everything now. The cost of a client finding a bug is much higher than the cost of finding it here.

**Agents**: QA Lead (lead), Web Lead and Automation Lead (fix owners)
**Duration**: 1–2 days
**Output**: Signed QA checklist with evidence, client preview package

---

## Inputs Required Before Starting

- [ ] Phase 3 quality gate cleared (smoke test passed)
- [ ] QA handoff doc with: staging URL, GHL sub-account access, test contact info
- [ ] Full scope doc (to verify all items were built)
- [ ] Lighthouse scores from build team (baseline)

---

## QA Checklist — Website

Run every item. Mark PASS, FAIL, or N/A with a note.

**Mobile (test at 375px and 390px)**
- [ ] Homepage renders correctly — no overflow, no broken layout
- [ ] CTA button visible and tappable above fold
- [ ] Phone number is a clickable `tel:` link
- [ ] All service pages render correctly
- [ ] Contact/booking page loads and form is accessible
- [ ] Navigation works (menu opens/closes, all links work)

**Desktop (1280px minimum)**
- [ ] All pages render correctly
- [ ] No text overflow or layout breaks
- [ ] Images load at correct resolution

**Performance**
- [ ] Run Lighthouse on homepage: mobile score ____  desktop score ____
- [ ] Run Lighthouse on one service page: mobile score ____
- [ ] Flag any score below 75 mobile as a required fix before launch

**Content & Accuracy**
- [ ] Business name spelled correctly throughout
- [ ] Address, phone, hours are accurate on all pages and match GBP
- [ ] No placeholder text ("Lorem ipsum", "[INSERT NAME]", etc.)
- [ ] No placeholder images
- [ ] All team names and credentials accurate (verify with client if unsure)
- [ ] Privacy policy and terms pages present and linked in footer

**Links & Forms**
- [ ] Click every navigation link — zero 404s
- [ ] Click every in-page CTA — lands on correct destination
- [ ] Submit contact form with test data — confirm GHL entry created
- [ ] Submit booking form — confirm appointment created in GHL calendar
- [ ] Confirm form confirmation message displays to user

**SEO & Technical**
- [ ] Title tags present and unique on all pages
- [ ] Meta descriptions present on all pages
- [ ] H1 on every page — only one H1 per page
- [ ] Schema markup: validate at schema.org/validator — no critical errors
- [ ] robots.txt present and not blocking indexation
- [ ] Sitemap.xml accessible at /sitemap.xml

---

## QA Checklist — Automations

- [ ] Speed-to-lead: submit test form → SMS received within 5 minutes → PASS / FAIL
- [ ] Speed-to-lead: submit test form → email received within 5 minutes → PASS / FAIL
- [ ] Booking confirmation: create test booking → SMS confirmation received → PASS / FAIL
- [ ] Booking confirmation: create test booking → email confirmation received → PASS / FAIL
- [ ] 24-hour reminder: confirm automation is scheduled correctly (manual check in GHL)
- [ ] Review request: complete test appointment → review request fires 2–4 hrs later → PASS / FAIL
- [ ] Pipeline stages: confirm opportunity moves correctly through stages on triggers
- [ ] No automation fires on wrong trigger (check for accidental double-triggers)

---

## Evidence Collection

For every PASS, collect evidence:

| Item | Evidence Required |
|------|-----------------|
| Mobile layout | Screenshot at 375px |
| Desktop layout | Screenshot at 1280px |
| Form submission | Screenshot of GHL contact created |
| Automation fires | Screenshot of GHL activity log |
| Lighthouse scores | Screenshot of full report |
| Schema validation | Screenshot of validator result |

Store all evidence in: [shared folder / client record / per agency protocol]

---

## Fix Protocol

- QA Lead logs all FAIL items with detail
- Pass to Web Lead (site issues) or Automation Lead (GHL issues) for fixes
- Fix owner confirms fix complete, QA Lead re-verifies
- Maximum 2 revision cycles. If cycle 2 fails on the same item: escalate to Strategy Lead

---

## Client Preview Package

Once QA checklist is fully PASSED, prepare client preview:

- [ ] Staging URL accessible
- [ ] Record Loom walkthrough of website (5–10 min): show homepage, key service pages, contact form, mobile view
- [ ] Record brief Loom of GHL pipeline: show pipeline stages, demonstrate a test lead flowing through
- [ ] Write preview summary doc using Template 3 from handoff-templates.md
- [ ] Send to client with 48–72 hour response deadline

---

## Quality Gate: Phase 4 → Phase 5

PASS requires:
- [ ] All QA checklist items PASSED (zero critical FAILs)
- [ ] Evidence collected and stored for all PASS items
- [ ] Lighthouse mobile 80+ confirmed (or exception documented and accepted by lead)
- [ ] Client preview package sent
- [ ] Client has approved or provided final change requests (max 1 round after preview)
- [ ] All preview change requests implemented and re-verified
