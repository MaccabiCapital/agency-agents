# Workflow: Client Engagement with Persistent Memory

> The same new client website workflow, but with an MCP memory server handling state between agents. No more copy-paste handoffs.

## The Problem with Manual Handoffs

In the standard workflow, every agent-to-agent transition requires manually passing context:

```
Activate Local SEO Specialist.
Here is the discovery brief from the Discovery Coach: [paste 2 pages of context]
Here are the keyword targets: [paste list]
Here is the client's GHL sub-account ID: [paste]
```

This is error-prone. Context gets lost. Agents make decisions without knowing what happened upstream.

## How MCP Memory Fixes This

With an MCP memory server, each agent stores its work products and decisions in shared memory. The next agent in the pipeline retrieves what it needs automatically.

### Example: Discovery → SEO Audit → Website Build

**Step 1: Discovery Coach completes intake**
```
Store in memory:
- client_name: "Vaughan Family Chiropractic"
- services: ["adjustment", "sports rehab", "pediatric chiro"]
- service_area: "Vaughan, Woodbridge, Thornhill"
- current_website: "vaughanchiro.com"
- ghl_subaccount: "loc_abc123"
- pain_points: ["no online booking", "page 3 on Google", "no reviews system"]
```

**Step 2: Local SEO Specialist picks up from memory**
```
Retrieve from memory: client_name, services, service_area, current_website
→ Runs audit with full context
→ Stores keyword targets, competitor analysis, citation gaps in memory
```

**Step 3: UX Architect picks up from memory**
```
Retrieve from memory: services, keyword_targets, pain_points
→ Creates site structure and wireframes with SEO-informed architecture
→ Stores approved_wireframes, site_map in memory
```

**Step 4: Website Developer picks up from memory**
```
Retrieve from memory: approved_wireframes, ghl_subaccount, site_map, keyword_targets
→ Builds with complete context — no guessing, no missing info
```

## Benefits

- **Zero context loss** between agent transitions
- **Audit trail** — every decision and deliverable is stored with timestamps
- **Cross-session continuity** — agents remember client work across multiple sessions
- **Reduced rework** — downstream agents have complete upstream context

## Setup

See [integrations/mcp-memory/README.md](../integrations/mcp-memory/README.md) for installation and configuration.

## When to Use Memory

- Multi-agent client engagements (3+ agents involved)
- Long-running projects (spanning multiple sessions)
- Recurring client work (monthly reporting, quarterly reviews)
- Complex handoffs with many context variables
