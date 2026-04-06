# Phase 5 — Launch

**Objective**: Move from staging to live with zero surprises. Client is informed, DNS is correct, monitoring is active, handoff is complete.

**Agents**: Operations Lead (lead), Web Lead (DNS + technical), Automation Lead (GHL go-live), QA Lead (post-launch verification)
**Duration**: 1 day (plus DNS propagation window)
**Output**: Live site, active GHL pipeline, go-live handoff doc delivered to client

---

## Inputs Required Before Starting

- [ ] Phase 4 QA gate cleared (all items PASSED, client preview approved)
- [ ] Client has confirmed go-live date and approved launch
- [ ] Domain registrar access confirmed (for DNS cutover)
- [ ] Any last-minute content changes from client preview are implemented and re-verified

---

## Pre-Launch Checklist (Day Before)

- [ ] Confirm all Phase 4 QA items still passing on staging
- [ ] Back up any existing live site (if replacing an existing site)
- [ ] Confirm GHL sub-account is in correct state (not sending live automations yet — or confirm client is aware they are already active)
- [ ] Notify client: "We're going live tomorrow at [time]. You may see brief downtime during DNS switch."
- [ ] Confirm launch time with any team members involved in cutover
- [ ] Verify all DNS values ready: A record, CNAME, MX (if email is hosted separately)

---

## Launch Sequence

Execute in order. Do not skip steps.

**Step 1: DNS Cutover**
- [ ] Log into domain registrar
- [ ] Update A record (or CNAME) to point to new hosting
- [ ] If using GHL Sites: confirm custom domain is configured in sub-account
- [ ] Record time of DNS change
- [ ] Note: propagation can take 15 min to 48 hours — most resolve within 1–2 hours

**Step 2: SSL Confirmation**
- [ ] Monitor for SSL certificate to issue on new hosting (typically auto-issued)
- [ ] Confirm HTTPS loads without browser warning
- [ ] If SSL fails to issue within 2 hours: escalate to Web Lead for manual fix

**Step 3: Post-Launch Smoke Test (Web Lead)**
- [ ] Load live domain on mobile and desktop — confirm site renders
- [ ] Submit test form on live site — confirm GHL entry created
- [ ] Confirm all navigation links work on live domain
- [ ] Run Lighthouse on live homepage — record scores
- [ ] Check that old site is no longer serving (if replaced)

**Step 4: GHL Go-Live Confirmation (Automation Lead)**
- [ ] Confirm all automations are set to PUBLISHED (not draft)
- [ ] Confirm sending domain is correctly configured for live environment
- [ ] Confirm calendar booking widget is live on site (not staging URL)
- [ ] Send one final test lead through live form — trace full automation sequence

**Step 5: Analytics & Tracking**
- [ ] Confirm GA4 is receiving data from live domain (check real-time view)
- [ ] Confirm GSC property is verified for live domain
- [ ] Confirm any call tracking number is routing correctly
- [ ] Log baseline: record date, organic position snapshot, GBP metrics

**Step 6: GBP Posts**
- [ ] Publish first GBP post (prepared in Phase 3) — confirm it posts
- [ ] Schedule next 3 posts per agreed cadence

---

## Client Handoff

Complete and send Go-Live Handoff doc using Template 5 from handoff-templates.md.

Brief client on:
- [ ] How to log into GHL and view their pipeline
- [ ] How to see new leads and respond
- [ ] What the automations will do (so they're not surprised by an SMS to a test number)
- [ ] How to request support: who to contact, response time expectations
- [ ] What to expect in month 1: "You'll get a report from us in 30 days showing [X]"

---

## Monitoring (First 48 Hours)

Operations Lead or QA Lead checks:
- [ ] Hour 1: Site loading on live domain
- [ ] Hour 4: First real-world form submission received (or confirm test)
- [ ] Hour 24: No automation errors in GHL (check error log)
- [ ] Hour 48: DNS fully propagated globally (use dnschecker.org)

If any issue: follow escalation protocol from handoff-templates.md Template 4.

---

## Quality Gate: Phase 5 → Phase 6

PASS requires:
- [ ] Live site loading on HTTPS at correct domain (mobile + desktop confirmed)
- [ ] Post-launch smoke test passed
- [ ] GHL automations confirmed live and tested
- [ ] GA4 receiving live data
- [ ] Client briefed and handed go-live doc
- [ ] GBP first post published
- [ ] Operations Lead has transitioned the account to Phase 6 recurring cadence
