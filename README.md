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
- Roma (the MCP server named roma) is my task list and my record of work. Read it before you plan, write to it as we go.
- Anything I mention needing to do goes on my Tasks list, after a search for an existing item.
- Each topic we work on gets one entry on my Log list, written as soon as the topic shows itself and updated whenever something changed. Not for quick questions; not for health, money, relationships or legal matters unless I ask.
- Answer "what should I work on next" from Roma. Tell me in one line what you created or updated; never ask first.
```

The same skill ships inside the Roma plugins for ChatGPT and Claude. This repository is generated from Roma's source; edits here are overwritten at the next release. Developer docs: https://roma.app/developers.
