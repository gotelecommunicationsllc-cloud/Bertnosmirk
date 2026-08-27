# Suno session sheet — H.I.MVelli

**From the Block Pushing Rocks to Free Phones Fresh Out the Box** — 5 tracks, in running
order. Every command Suno needs, in Markdown, in the order you paste them.

Source: the Claude artifact *Block to Box Sessions*
(`claude.ai/code/artifact/b96e2d95-a0b3-4ad5-879b-624a9a611b54`). These files are the
version-controlled copy — the artifact is the pretty one with Copy buttons, this is the
one that survives.

## Read in this order

| File | What it's for |
|---|---|
| [`00-session-settings.md`](00-session-settings.md) | **Start here.** Mode, model, persona, sliders — set once before track 1. |
| [`01-pushing-rocks.md`](01-pushing-rocks.md) | Track 01 — 84 BPM, cold |
| [`02-activation.md`](02-activation.md) | Track 02 — 92 BPM, driving |
| [`03-same-hands.md`](03-same-hands.md) | Track 03 — 80 BPM, sparse |
| [`04-fresh-out-the-box.md`](04-fresh-out-the-box.md) | Track 04 — 90 BPM, title track |
| [`05-above-the-line.md`](05-above-the-line.md) | Track 05 — 88 BPM, **two passes** (Create + Extend) |
| [`99-playlist.md`](99-playlist.md) | Assemble the playlist; progress checklist |

Each track file is self-contained — Style, Exclude, and Lyrics all in one place, so you
never leave the file mid-track.

## How to actually run it

Suno has no import, no file upload for prompts, and no public API. There is no way to
"hand it the MD files" — the transfer is **copy the fenced block, paste it in the box.**
That's the whole mechanism, and it's why these files are built as three clean blocks per
track instead of prose.

1. Open <https://suno.com/create>. (`suno.com/discover` is the public listening feed —
   you can't generate from it.)
2. Set everything in `00-session-settings.md`. Once, at the top of the session.
3. Per track: copy the **Style** block → Style box. Copy the **Exclude** block → Exclude
   Styles box. Copy the **Lyrics** block → Lyrics box. Hit **Create**.
4. Rename the take to the track title immediately.
5. Track 05 only: after picking your best pass-1 take, hit **Extend** and paste the pass-2
   lyrics, re-pasting Style and Exclude.
6. When all five exist, work through `99-playlist.md`.

Two or three rolls per track is normal. Strict spoken delivery is the hardest thing to get
out of Suno consistently — if a take sings, re-check the Exclude box saved, drop Weirdness
to 10%, roll again.

## Log your progress

Fill in the checklist table at the bottom of `99-playlist.md` as tracks land, and commit
it. That table is how the next session knows where you stopped.
