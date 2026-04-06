# Phase 2 — Foundation Setup

**Objective**: Get all infrastructure in place before any build work starts. No website, no automations, no content until the foundation is stable.

**Agents**: Automation Lead (lead), Web Lead (support), Operations Lead (coordination)
**Duration**: 1–3 days
**Output**: GHL sub-account configured, domain/hosting live, pipeline stages set up

---

## Inputs Required Before Starting

- [ ] Signed scope from Phase 1
- [ ] Client's domain name and registrar access (or decision to use a new domain)
- [ ] Hosting platform decision (existing or new — Cloudflare, WP Engine, GHL sites, etc.)
- [ ] GHL agency access confirmed
- [ ] Client brand assets: logo, colors, fonts (or note these are TBD)

---

## Step 1: GHL Sub-Account Setup

Automation Lead owns this.

- [ ] Create new sub-account under agency account
- [ ] Name convention: `[ClientName] - [City]` or per agency standard
- [ ] Apply applicable GHL snapshot (healthcare / local service / generic)
- [ ] Configure business info: name, address, phone, email, timezone
- [ ] Connect client phone number (A2P verified or Twilio sub-account)
- [ ] Set up sending domain for email (or use agency domain with subdomain)
- [ ] Verify sending: send test SMS and email, confirm delivery
- [ ] Set up user access: client login created with appropriate permissions

---

## Step 2: Pipeline Configuration

- [ ] Define pipeline stages (standard starting point):
  - New Lead
  - Contacted
  - Appointment Booked
  - Appointment Completed
  - Won / Client
  - Lost / Not Interested
- [ ] Adjust stages to match client's actual sales process
- [ ] Configure lead source tags (website form, GBP call, referral, etc.)
- [ ] Set up basic opportunity card fields: lead name, service interested in, notes

---

## Step 3: Domain & Hosting

Web Lead supports.

- [ ] Confirm domain ownership and registrar access
- [ ] Point domain to hosting platform (or prepare for DNS cutover at launch)
- [ ] Set up staging environment: `staging.[domain].com` or equivalent
- [ ] Confirm SSL certificate will be issued on go-live
- [ ] If using GHL Sites: configure custom domain in sub-account settings
- [ ] If using WordPress: install WP, select/install theme framework, confirm admin access

---

## Step 4: Analytics & Tracking Setup

- [ ] Google Analytics 4: property created or access confirmed
- [ ] Google Search Console: property verified (DNS or HTML tag)
- [ ] GBP access: confirm client has agency access to GBP or transfer initiated
- [ ] Call tracking: configure GHL call tracking number if applicable
- [ ] UTM convention: document UTM structure for all paid or tracked sources

---

## Step 5: Integration Pre-Work

- [ ] Identify all integrations needed (calendar, EHR, payment, etc.)
- [ ] Confirm API keys, credentials, or OAuth access for each
- [ ] Document any integrations that need client action to unlock
- [ ] Note: integrations that are blocked by missing credentials are flagged as Phase 3 risks

---

## Step 6: Foundation Handoff to Build Team

Document and hand off to Web Lead and Automation Lead for Phase 3:

```
FOUNDATION SUMMARY — [CLIENT NAME]
────────────────────────────────────
GHL sub-account: [ID / name]
Pipeline stages: [list]
Sending: SMS [confirmed / pending] | Email [confirmed / pending]
Staging URL: [URL]
Hosting: [provider + access location]
Domain registrar: [provider + access location]
GA4: [property ID]
GSC: [verified / pending]
GBP access: [confirmed / pending]
Integrations needed: [list] | Blocked on: [any pending credentials]
Client assets received: [logo yes/no] [colors yes/no] [photos yes/no] [copy yes/no]
```

---

## Quality Gate: Phase 2 → Phase 3

PASS requires:
- [ ] GHL sub-account created, sending verified (test SMS + email received)
- [ ] Pipeline stages configured
- [ ] Staging environment accessible via URL
- [ ] GA4 and GSC properties set up
- [ ] Foundation summary doc handed off to build team
- [ ] Any blocked integrations flagged with a plan
