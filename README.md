# Kill Switch

> *"Better to pull the switch now than let the market pull it later."*

A model-agnostic AI skill that runs a ruthless pre-mortem on any startup, app, or product idea. Kill Switch stops weak ideas before you spend months building them, and lets strong ones through only after they've been properly tested.

## What it does

Give your AI your idea and ask it to tear it apart. Kill Switch will:

1. **Restate the idea** in one sentence and name its **magic**: the one thing that makes it interesting.
2. **Attack it from ten angles:** core bet, first ten minutes, retention, distribution, cold start, money, running cost, safety/legal, competition, and founder capacity.
3. **Rank every objection** as FATAL, SERIOUS, or FIXABLE, with evidence labels ([Known], [Pattern], [Assumption]) and what would prove it wrong.
4. **Run the magic erosion test:** do the fixes destroy what made the idea special?
5. **Deliver a verdict** (DEAD, ON LIFE SUPPORT, or SURVIVES INTERROGATION) plus a short pre-mortem: how the idea fails, told from two years in the future.
6. **Design a kill test:** one cheap experiment (two weeks or less) with a pass/fail threshold set in advance.
7. **Name what survives**, if anything.

Then defend your idea. Kill Switch judges each defence as **HOLDS**, **PARTIAL**, **DODGE**, or **MAGIC LOST**, and calls out classic founder escape moves.

## The rules

- Attacks the idea, never the person.
- Never invents statistics or competitor facts.
- No compliment sandwiches, and no manufactured objections either.
- Every objection is falsifiable.

## Works with any LLM

Kill Switch is plain Markdown instructions. No code, no APIs, no model-specific features. It comes in two formats:

| File | Use it with |
|---|---|
| `kill-switch/` folder (or `kill-switch.zip` from Releases) | Any tool that supports the `SKILL.md` skill-folder format |
| `kill-switch-prompt.md` | Any chatbot or LLM: paste it in as a system prompt or custom instructions |

## Install

**Any chatbot (ChatGPT, Gemini, Claude, Copilot, Llama, local models, etc.):**
Copy the contents of `kill-switch-prompt.md` into one of these:
- A custom assistant's instructions (e.g. a custom GPT, a Gemini Gem, a Claude Project)
- The system prompt, if you're using an API or a local model
- The first message of a chat, followed by your idea

**Claude app (web, desktop, mobile):**
1. Download `kill-switch.zip` from the [Releases page](https://github.com/arunjithm/kill-switch/releases/latest).
2. Go to **Customize > Skills**.
3. Click **+**, then **Create skill**, then **Upload a skill**, and choose the ZIP.
4. Make sure the skill is toggled on.

**Coding agents that support skill folders (e.g. Claude Code):**
Copy the `kill-switch` folder into the agent's skills directory. For Claude Code, that's `~/.claude/skills/` (personal) or `.claude/skills/` (project). For other agents, check their docs for where skills live.

**Tip:** Kill Switch checks competitors more reliably when your LLM has web search turned on. Without it, competitor claims are labelled as assumptions.

## Try it

- "Tear apart this app idea: …"
- "Play devil's advocate on my startup idea."
- "Run a pre-mortem on this product."
- "Tell me every reason this will fail."

## Structure

```
kill-switch/
├── SKILL.md                     # Role, rules, and review process
└── reference/
    └── failure-patterns.md      # Common failure patterns per attack zone
kill-switch-prompt.md            # Single-file version for any LLM
```

## Author

Created by Arunjith Mohan Kumar (@ritesandwrites).

## License

MIT. Use it, fork it, improve it.
