# Bertnosmirk

Context repository for the Bertnosmirk project.

## What's here

| File | Purpose |
|---|---|
| `BERTNOSMIRK_HANDOFF.md` | **The master context file.** Single source of truth — project definition, current state, decisions, open questions, and a dated session log. |
| `CLAUDE.md` | Auto-loaded by Claude Code. Points every session at the handoff file and requires it to be updated before the session ends. |

## How to use it

**With Claude Code** — nothing to do. `CLAUDE.md` loads automatically and directs the
session to read the handoff file.

**With any other AI tool** (ChatGPT, Gemini, Copilot, local models) — upload or paste
`BERTNOSMIRK_HANDOFF.md` at the start of the session. Section 0 of that file tells the
model how to behave and how to hand off when it's done.

**Raw link for tools that fetch URLs:**

```
https://raw.githubusercontent.com/gotelecommunicationsllc-cloud/Bertnosmirk/main/BERTNOSMIRK_HANDOFF.md
```

## The one rule

Every session updates `BERTNOSMIRK_HANDOFF.md` before it ends. That is what makes the
next handoff work.
