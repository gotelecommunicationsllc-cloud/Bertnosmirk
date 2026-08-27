# Suno Prompt Pack — H.I.MVelli Rap Track (Heavy 808 / Strict Bar Delivery)

Ready-to-paste blocks for suno.com. Copy each block into the matching field.
Nothing here needs editing to work — the optional tweaks are marked.

---

## BLOCK A — STYLE box (paste as-is)

```
Aggressive inner-city street rap, grimy East Coast boom-trap. Hard-knocking 808s with deep
distorted sub-bass tuned to rattle a car trunk, punchy kick, sharp cracking snare, rapid
hi-hat rolls and triplet fills. Dark minor-key piano loop, sparse menacing strings, heavy
low-end mix. Strict spoken rap delivery — percussive, syllable-dense cadence locked tight
in the pocket, hugging the drums bar for bar. Hard consonants, heavy emphasis on the one.
Dry close-mic'd vocal, forward and raw, minimal reverb, no vocal layering. 88 BPM.
```

Character count is inside Suno's 1000-char style limit.

**Optional BPM swaps:** `82 BPM` = heavier, more menacing drag · `95 BPM` = more
aggressive forward push. Keep the halftime feel either way.

---

## BLOCK B — EXCLUDE STYLES box (paste as-is)

```
singing, sung vocals, melodic rap, sung hook, chorus melody, autotune, pitch correction,
harmony, harmonies, vocal layering, doubled vocals, backing vocals, melodic ad-libs,
falsetto, crooning, humming, choir, R&B, pop, trap soul, EDM, acoustic, lo-fi, jazzy,
female vocals, reverb wash, ambient pads, whispering
```

This field is doing most of the "no singing" work. Do not shorten it — Suno's default
pull is toward melody, and the exclusion list is the strongest counterweight in the UI.

---

## BLOCK C — Header for the LYRICS box

Paste this at the very top of the lyrics box, above the first bar. It steers delivery
per-section rather than globally, which is what actually holds a rap flow together.

```
[Style: aggressive street rap, spoken bar delivery, no melody]
[Vocal: dry close-mic rap, percussive, syllable-heavy, hard consonants, no singing]

[Intro - spoken, dry, 808 only]

[Verse 1 - strict bars, locked to the beat, no melody]

[Hook - chanted, spoken rhythm, NOT sung]

[Verse 2 - strict bars, heavier emphasis, no melody]

[Outro - 808 fade, spoken tag]
```

Repeat `- no melody` on every section tag you add. Section tags without it are where
Suno slips back into singing.

---

## BLOCK D — Single-paragraph version

For a one-box workflow (simple mode, or any tool that takes one prompt string):

```
Create an aggressive inner-city street rap track at 88 BPM with heavy 808s — deep
distorted sub-bass that vibrates a car trunk, punchy kick, cracking snare, rapid hi-hat
rolls — over a dark, sparse, minor-key grimy loop. Vocals are strict rap only: no singing,
no melody, no harmonies, no melodic ad-libs. Punchy, percussive, spoken flow with a
syllable-heavy cadence that rides the beat and hugs the pocket bar for bar, heavy emphasis
and clear hard consonants. Vocal is dry and close-mic'd, forward in the mix, minimal
reverb, no layering. Metaphor-dense street writing.
```

---

## SETTINGS CHECKLIST (in the Suno UI)

| Setting | Value | Why |
|---|---|---|
| Mode | **Custom** | Simple mode ignores the exclude-styles field |
| Model | **v5** (or latest) | Best rap-pocket adherence and vocal clarity |
| Instrumental | **OFF** | — |
| Style box | Block A | — |
| Exclude styles | Block B | — |
| Lyrics box | Block C header + your bars | — |
| Persona / Suno Voices | **H.I.MVelli** | See below |
| Weirdness | **~20–30%** | Higher values invent melody |
| Style Influence | **~75–85%** | Keeps it locked to the aggressive street brief |

---

## USING THE H.I.MVelli VOICE

Suno Voices needs the voice registered to your account before any prompt can call it —
it can't be referenced by name from a text prompt alone.

1. suno.com → **Create** → find the **Persona / Voices** control on the Custom panel.
2. **Add / Upload voice** → upload the H.I.MVelli file.
   - Best results: 30–60 seconds, one voice only, dry, no beat under it, no other
     speakers, no music bed. A clean a cappella rap take beats a mixed song every time.
3. Name it `H.I.MVelli` and save.
4. Select it as the voice/persona for this generation **before** hitting Create.
5. Generate with Blocks A, B, and C in place.

If the upload is a full mixed track, isolate the vocal stem first — Suno will otherwise
model the beat's tonality into the voice and the result drifts melodic.

---

## IF IT STILL SINGS

In order of effectiveness:

1. Confirm **Exclude styles** (Block B) actually saved — it silently clears on some mode
   switches.
2. Add `[no melody]` inline mid-verse, not just at section heads.
3. Drop **Weirdness** to 10%.
4. Shorten your bars. Long lines give Suno room to stretch syllables into pitch; dense,
   clipped lines force percussive delivery.
5. Write the bars with hard stop-consonants at line ends (k, t, p, ck) — sung endings
   need open vowels, so consonant endings physically resist melody.
6. Regenerate rather than fighting one seed. Two or three rolls with the same prompt is
   normal for strict spoken delivery.

---

## NOT YET DONE

- **Lyrics.** No bars are written. The prompt pack controls sound and delivery; the
  metaphor-heavy street writing you asked for still needs to be authored.
- **The generation itself.** Requires account access (see Section 3 of the handoff file).
