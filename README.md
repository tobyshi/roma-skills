# Roma skills

The skill that teaches an agent how to use [Roma](https://roma.app), the to-do list and record of work for you and your agents: when to reach for Roma, how to keep to-dos on Tasks and a record of each topic on Log, and how to answer what you should work on next from it.

## Install

One command puts the skill where your agent reads it (Claude Code, Codex, Cursor, Gemini CLI and the other agents the [skills CLI](https://github.com/vercel-labs/skills) supports):

```sh
npx skills add tobyshi/roma-skills
```

Then connect your agent to Roma's MCP server at `https://api.roma.app/mcp` (the steps per agent: https://roma.app/agents) and add to your agent's instructions file:

```md
## Roma
- Add anything I mention needing to do to my Tasks list in Roma.
- Keep a record of each topic we work on in my Log list in Roma, following the roma skill.
- Answer what I should work on next from Roma.
```

The same skill ships inside the Roma plugins for ChatGPT and Claude. This repository is generated from Roma's source; edits here are overwritten at the next release. Developer docs: https://roma.app/developers.
