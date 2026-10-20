# New Dev skills

Agent skills for working with [New Dev](https://newdev.org): the dashboard at
[app.newdev.org](https://app.newdev.org) and its MCP server for managing New Dev
Discord bots (Lilith, Hermes and customer-owned premium bots).

## Install

```bash
npx skills add newdevstore/skills
```

## Skills

| Skill | What it teaches |
|---|---|
| [`new-dev`](skills/new-dev/SKILL.md) | Connecting the New Dev MCP server, the tool workflow, the two-step safety harness, configuring systems and commands correctly, the dashboard map and troubleshooting. |

The systems catalog in `skills/new-dev/references/systems.md` is generated from the
dashboard code (`app.newdev.org/scripts/dump-mcp-systems.ts`).
