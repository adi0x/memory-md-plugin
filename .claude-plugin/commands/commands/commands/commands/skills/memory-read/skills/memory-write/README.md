# memory-md plugin

Gives your Claude Code agent experiential memory. It tracks decisions, outcomes, and lessons learned in MEMORY.md so your agent gets wiser over time.

## Install

```
claude plugin install github:adi0x/memory-md-plugin
```

## Commands

| Command | What it does |
|---------|-------------|
| `/memory:init` | Set up MEMORY.md in your project |
| `/memory:log` | Create a memory entry from the current conversation |
| `/memory:update` | Add outcomes and lessons to past memories |
| `/memory:recall` | Search for relevant past experiences |

## What happens automatically

Once MEMORY.md exists in your project:

- Before giving advice, the agent checks for relevant past experiences
- After meaningful decisions, the agent offers to create a memory entry
- Past lessons are referenced naturally in conversation, not robotically

## How it works

Your agent writes structured entries with five parts: situation, decision, reasoning, outcome, and lesson. Over time this builds a wisdom layer that makes every future conversation better.

No databases. No servers. Just a markdown file that any agent can read.

## Links

- [MEMORY.md spec](https://github.com/adi0x/memory-md)
- [@0x_adithi](https://twitter.com/0x_adithi)
