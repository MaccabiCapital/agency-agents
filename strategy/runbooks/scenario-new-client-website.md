# Runbook: New Client Website

**Scenario**: Build and launch a website for a new or existing client. Full build from brief to go-live.

**Typical timeline**: 2–3 weeks
**Agents**: Web Lead (build), Automation Lead (forms + GHL), Marketing Lead (SEO + copy), QA Lead (QA), Operations Lead (coordination + launch)

---

## When to Use This Runbook

- New client whose website is the primary deliverable
- Existing client needing a full website rebuild
- Client where Phase 0 audit confirmed the site is unfixable (not worth patching)

Use the **Build Sprint** deployment mode. Start at Phase 2 if scope is already confirmed.

---

## Activation Prompt

```
Activate Web Lead for new client website build — Build Sprint mode.

Client: [CLIENT NAME] | Vertical: [vertical] | URL (if existing): [URL]
Staging: [URL] | GHL sub-account: [name/ID]
Pages: [list all pages in scope]
Forms: [contact form / booking / other — describe]
Brand assets: [received / pending — note what's missing]
Target go-live: [DATE]

Run Phases 2 → 3 → 4 → 5.
QA gate required before client preview. Client preview required before launch.
Escalate any scope changes or client-side blockers immediately.
```

---

## Phase Sequence

| Phase | Focus | Owner | Done When |
|-------|-------|-------|-----------|
| 2 — Foundation | Staging env, GHL sub-account, domain confirmed | Automation Lead | Staging URL accessible, GHL ready |
| 3 — Build | Pages, SEO, forms connected, automations | Web Lead + Automation Lead | All pages live on staging, smoke test passed |
| 4 — QA | Full QA checklist, client preview | QA Lead | Checklist signed, client approved |
| 5 — Launch | DNS, go-live, handoff | Operations Lead | Live on HTTPS, client briefed |

---

## Common Blockers and How to Handle Them

| Blocker | Action |
|---------|--------|
| Client hasn't sent photos | Build with stock photos, flag for swap — don't stall the build |
| Client wants to write their own copy | Give them a 48-hour window with a template. After that, write it. |
| Domain registrar access not confirmed | Build on staging, launch when access arrives — don't hold the build |
| Client requests scope additions mid-build | Log the request, do not build it yet — bring to Operations Lead for scope decision |
| GHL sending not verified | Build automations, test locally — flag as a blocker for go-live, not for build |

---

## Go/No-Go Criteria for Launch

All must be YES:
- [ ] QA checklist fully PASSED with evidence
- [ ] Client has approved staging preview in writing or on a recorded call
- [ ] Domain registrar access confirmed
- [ ] GHL sub-account sending verified
- [ ] GA4 property ready to receive live traffic
- [ ] Operations Lead has completed client briefing on GHL access and support process
