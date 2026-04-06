---
name: RescueMyWorkday
description: AI-assisted operating company for small service businesses — healthcare practices and local-service operators. Acquire, Convert, Deliver, Retain.
slug: rescuemyworkday
schema: agentcompanies/v1
version: 1.0.0
license: MIT
authors:
  - name: Arthur Smelyansky
goals:
  - Acquire clients through websites, local SEO, and trust-building
  - Convert leads through speed-to-lead, booking flows, and sales pipelines
  - Deliver implementation through websites, automation, QA, and reporting
  - Retain clients through reviews, nurture, recurring optimization, and SOPs
metadata:
  sources:
    - kind: github-dir
      repo: MaccabiCapital/agency-agents
      path: .
      attribution: RescueMyWorkday
      license: MIT
      usage: referenced
---

RescueMyWorkday is an AI-assisted operating company with 103 agents organized into 8 divisions. Each agent is a domain specialist focused on practical delivery for healthcare practices and local-service businesses.

## How It Works

RescueMyWorkday operates on the **ACDR model** — Acquire → Convert → Deliver → Retain. The CEO coordinates across division heads, who manage their teams autonomously. Client engagements follow a structured pipeline with quality gates at each phase: Discovery, Strategy, Foundation, Build, QA & Hardening, Launch, and Operate.

## Divisions

- **Engineering** (19 agents) — Websites, integrations, automation, DevOps, security, data, and AI systems for local-service business clients
- **Design** (8 agents) — UX architecture, UI design, brand identity, accessibility, and visual content for client deliverables
- **Marketing & Paid Media** (20 agents) — Local SEO, content, social media, reviews, AI visibility, paid search, paid social, tracking, and retargeting
- **Product & Project Management** (11 agents) — Service design, conversion optimization, delivery tracking, and client project execution
- **Sales** (8 agents) — Discovery, proposals, pipeline management, outbound, and account growth for healthcare and local-service businesses
- **Quality Assurance** (8 agents) — Website QA, automation testing, performance benchmarking, accessibility auditing, and evidence collection
- **Operations & Support** (6 agents) — Client support, analytics reporting, finance, infrastructure, and legal compliance
- **Specialized Operations** (15 agents) — Orchestration, workflows, compliance, automation governance, training, document generation, and integration building

## Leadership

| Role | Slug | Reports To |
|------|------|------------|
| Managing Director & CEO | ceo | — |
| VP of Engineering & CTO | vp-engineering | CEO |
| Creative Director | creative-director | CEO |
| Chief Marketing Officer | cmo | CEO |
| VP of Product | vp-product | CEO |
| VP of Sales | vp-sales | CEO |
| VP of Operations | vp-operations | CEO |
| QA Director | qa-director | VP-ENGINEERING |

## Tech Stack

- **GHL (GoHighLevel)** — Primary CRM, automation, and pipeline platform
- **n8n** — Workflow automation and integration orchestration
- **Vercel / Railway / DigitalOcean** — Hosting and deployment
- **Cloudflare** — DNS, SSL, CDN
- **Google Business Profile** — Local SEO and visibility
- **Google Ads / Meta Ads** — Paid acquisition
- **GA4 / GTM / CallRail** — Tracking and attribution

Built from [MaccabiCapital/agency-agents](https://github.com/MaccabiCapital/agency-agents) for [Paperclip](https://github.com/paperclipai/paperclip)
