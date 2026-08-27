# Bertnosmirk

Working repository for **H.I.MVelli** — *From the Block Pushing Rocks to Free Phones Fresh
Out the Box*, a five-track rap project produced in Suno. Plus the context file that keeps
every AI session on the same page.

## What's here

| Path | Purpose |
|---|---|
| `suno/` | **The session sheet.** Every Suno command for all five tracks — Style, Exclude Styles, and lyrics — one Markdown file per track, in paste order. Start at `suno/README.md`. |
| `BERTNOSMIRK_HANDOFF.md` | **The master context file.** Single source of truth — project definition, current state, decisions, open questions, and a dated session log. |
| `CLAUDE.md` | Auto-loaded by Claude Code. Points every session at the handoff file and requires it to be updated before the session ends. |

## Running the tracks

Open <https://suno.com/create>, set up from `suno/00-session-settings.md`, then work
`01` → `05`. Each track file holds the three blocks you paste, in order. Log what lands in
the checklist at the bottom of `suno/99-playlist.md`.

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
