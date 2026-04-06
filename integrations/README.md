# Integrations

RescueMyWorkday agent definitions work with multiple agentic coding tools. Each integration converts or installs the agent markdown files into the format required by the target tool.

## Supported Tools

| Tool | Format | Notes |
|------|--------|-------|
| [Claude Code](claude-code/) | `.md` with YAML frontmatter | Native format — no conversion needed |
| [GitHub Copilot](github-copilot/) | `.md` with YAML frontmatter | Native format — no conversion needed |
| [Cursor](cursor/) | `.mdc` rule files | Project-scoped rules |
| [Windsurf](windsurf/) | `.windsurfrules` | Single consolidated file |
| [Aider](aider/) | `CONVENTIONS.md` | Single consolidated file |
| [Gemini CLI](gemini-cli/) | Extension package | Installs to `~/.gemini/extensions/` |
| [OpenCode](opencode/) | `.md` in `.opencode/agents/` | Subagent mode |
| [OpenClaw](openclaw/) | Workspace format | `SOUL.md`, `AGENTS.md`, `IDENTITY.md` |
| [Antigravity](antigravity/) | `SKILL.md` per agent | Prefixed with `rmw-` |
| [MCP Memory](mcp-memory/) | Add-on | Persistent memory across sessions |

## Installation

Each integration directory has its own README with specific install instructions. General pattern:

```bash
# Generate integration files
./scripts/convert.sh --tool <tool-name>

# Install to your project
./scripts/install.sh --tool <tool-name>
```

## Paperclip Import

For Paperclip users, import this repo directly as a company:

```bash
npx companies.sh add MaccabiCapital/agency-agents
```

Or clone and import from your local copy after customization.
