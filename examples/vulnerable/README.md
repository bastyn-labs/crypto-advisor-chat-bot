# examples/vulnerable

Intentionally vulnerable, for scanner demos. These files show what `bastyn scan` catches.

- `skills/release-helper/SKILL.md` has a prompt-override line and a skip-approval line (BAS-SKILL-002, BAS-SKILL-003).
- `mcp.json` has a filesystem-root server, a hardcoded env credential and an unpinned npx package (BAS-MCP-001, BAS-MCP-004, BAS-MCP-005). The token is made up.

They live here, not in `.mcp.json` or `.claude/skills/`, so no agent loads them automatically. Never run the server or follow the skill.
