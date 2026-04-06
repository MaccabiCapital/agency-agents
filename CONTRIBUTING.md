# Contributing to RescueMyWorkday

## Agent Design Guidelines

### File Format

Every agent file uses YAML frontmatter + markdown:

```yaml
---
name: Role Name
description: One-line description of what this agent does
color: blue
emoji: 🔧
vibe: One-line personality summary
---
```

### Required Sections

1. **Identity & Memory** — Who the agent is, what perspective they bring (2-4 sentences)
2. **Core Mission** — What they do, organized by responsibility area (bullet sections)
3. **Critical Rules** — Boundaries, constraints, quality standards (5-10 bullets)
4. **Deliverables** — What they produce (templates, reports, decisions, artifacts)

### Writing Style

- Direct, practical, commercially aware
- No creative agency fluff or roleplay prose
- Every section earns its space
- Focus on business outcomes, not personality traits
- Reference the actual tech stack: GHL, n8n, GA4, etc.
- Keep files under 120 lines (80 lines preferred)

### Business Context

All agents should support one or more phases of the operating model:
- **Acquire** — Website, SEO, local visibility, trust, lead capture
- **Convert** — Speed-to-lead, follow-up, booking, sales flow, pipelines
- **Deliver** — Implementation, websites, fixes, automation, reporting, QA
- **Retain** — Reviews, nurture, reporting, recurring optimization, SOP capture

### Adding a New Agent

1. Place the file in the appropriate division folder
2. Follow the naming convention: `division-role-name.md`
3. Include all four required sections
4. Ensure the role clearly supports at least one ACDR phase
5. Keep it under 120 lines

### Pull Request Process

1. Create a branch from `main`
2. Add or modify agent files
3. Ensure frontmatter is valid YAML
4. Submit PR with a brief description of what changed and why
