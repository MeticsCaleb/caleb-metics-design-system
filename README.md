# Metics Media — Design System Spec

This system is foolproof by design: it locks how a video is **made**, not how it **looks**. Every video is built the same way; every video is free to look completely different — and it *should*, because each product we cover is different. The fewer hard visual rules we impose, the fewer things there are to fight over in revisions. So we lock only what truly has to stay constant and hand everything else to Claude Design's judgment, themed to the product.

---

## What's locked — and only this

1. **The build formula.** The order of operations below. Every video is made this way.
2. **The CTA / link-on-screen.** The one visual element done *exactly* the same every time. Everything else can change; this can't.
3. **The deliverable mechanics.** The SOLID (full-frame) / ALPHA (transparent overlay) model, with true alpha gaps wherever the host is just talking, all pinned to the second-by-second transcript. This is what lets the finished clip drop cleanly over the talking-head footage. It's how the video *works*, not how it looks.
4. **Coverage — no long dead gaps.** Never more than ~5 seconds of bare talking head (alpha with no graphic doing work) at a stretch. If a passage would leave the host talking alone longer than that, treat it as a cue to carry the idea visually — a simple icon, a number, a word, an evolving graphic, or a clever bit of design. This is a prompt to communicate, not a license to add filler: the visual still has to serve a real idea. The only exception is the CTA / link-on-screen, which may dwell as long as the moment needs. (A graphic getting trimmed or shortened to fit is fine — everything composites over the 4K talking-head footage, which is always underneath.)

Everything else — colors, fonts, vibe, layout, composition, motion style, motifs, treatments — is free, and is *expected* to change from video to video.

---

## The build formula (same every video)

You're building the motion-graphics layer for a talking-head video. Work in this order every time — it's the process, not a cage; the creative choices inside each step are yours.

1. **Start from the transcript.** The second-by-second transcript is the source of truth — read it first. Everything is anchored to when each line is spoken. (You're making a video, not a static design.)
2. **Find the beats.** Walk the transcript and mark the moments worth a graphic — a key idea, a number, a name/logo, the CTA. One idea per beat. Short talking stretches can stay empty (alpha) so the host carries them — but never let a bare stretch run past ~5s; if it would, that's the cue to find a visual for it (locked rule 4).
3. **Communicate each beat the clearest possible way — visual first.** Reach for an icon, emoji, real logo, or a number before words; less text, more visual. There's almost always a clearer way to land an idea than the obvious one — find it. If a clever or unexpected layout communicates better than a tidy centered one, use it.
4. **Choose the layer.** Full-frame (SOLID, host off camera) for explained ideas — the default. ALPHA overlay only for the open and the CTA.
5. **Design it for clarity, themed to the product.** Pull the look from the product's assets so it feels in-theme. Bold and uncluttered. Centered is a fine default, but break it with smart composition whenever an idea is served better that way.
6. **Time it to the transcript.** Each graphic enters on its line, settles, holds, exits on a clean cut. Pace to the spoken words.
7. **Self-check.** Walk the whole thing against the transcript for timing, confirm each beat reads instantly, and confirm the talking stretches are true alpha so it drops over the footage. Then build.

---

## The CTA / link-on-screen — the one locked look

This is the only visual that's identical every video, so viewers learn to trust it.

- The YouTube **watch-card** pops up from the bottom, docked low so it never crosses the host's face. Anatomy stays fixed: video title → channel row (Metics glyph, channel name + gray verified check, subscriber count, Subscribe, like/Share/Download) → views → offer line.
- **Offer line:** green check, then "**[Platform] ([offer type]):**" in bold, then the full `meticsmedia.com/<slug>` link in YouTube's link blue. Match the offer type to the deal (the full offer-type table lives in the README playbook). A highlight box sweeps the offer line; an arrow cursor glides in and taps.
- It uses YouTube's own UI styling (light-mode palette, black Metics glyph on the white card) regardless of the video's theme, and holds through the outro crossfade.
- The **plain-text link** that precedes it sits in a clean container over the talking head (the stand-out rule below in action).

---

## The north star: communicate clearly, visual-first

Everything free is still in service of one goal — make each idea instantly clear to a complete beginner, many of whom don't read English. Numbers, icons, and real logos carry meaning; text is a last resort. When choosing between "correct" and "clearest," always pick clearest — even if that means a clever, non-obvious design. This is the lens for every free decision.

---

## Free to flex (Claude Design's room — themed per product)

- **Color, base, and mood:** pulled from the product's assets/screenshots so the video feels in-theme. No fixed channel palette — including the base and overall mood.
- **Fonts:** default to a clean house font (Manrope) for a light through-line, but use the product's own font when it fits.
- **Layout & composition:** centered is just a starting point — dynamic, off-center, or unconventional layouts are encouraged when they land an idea better.
- **Motion, motifs, treatments:** drop shadows, gradients, glows, containers — all fair game, used tastefully. The *one* treatment constraint: an ALPHA element sitting over the talking head must clearly stand out from unknown footage (a bubble/capsule, solid container, or strong contrast — whatever fits).
- **Permission to invent:** make new slides for new ideas, build fresh layouts, make real creative calls. The system starts you in the right place; it doesn't finish the job for you.

---

## Defaults & taste signals (where to start — not rules)

- Full-frame-first; don't over-rely on talking-head overlays (overlays are for the open and CTA).
- Lean clean and uncluttered; let one idea breathe per beat.
- Calm and clear suits the beginner audience — not frantic — but the visual energy can flex to the product.
- Centered reads well by default; break it deliberately, not accidentally.
- Color-tinted soft shadows and bubble/capsule containers usually look better on our work than hard neutral shadows.
- Motion: quick, purposeful entrance, then settle — avoid distracting idle wiggle. Exact easing/timing is yours.
- Never render guides (rule-of-thirds, safe-zone, PiP) into the final.
- The open gets a name card — "Caleb" (no period) + "Metics Media" — but its design is free.

---

## Reference: how the Northwest build did it (examples, not rules)

A worked example to borrow from — especially useful for the parts that don't change. The palette should come from each product, so treat these as one set of choices, not a spec.

- Color roles (values flex per product): base, ink/dark, one main accent (+ lighter/deeper), a muted tone, hairlines. Northwest used base #FFFFFF (subtle white radial wash), ink/navy #003952, accent #1F9E5B. The watch-card keeps YouTube's light-mode palette (text #0F0F0F, secondary #606060, pills #F2F2F2, red #CC0000, link #065FD4) every time.
- Type defaults: Manrope 700/800/900, JetBrains Mono for mono; hero numbers ~380–420px / weight 900; mono chips with wide tracking.
- Radii: cards ~28–32px, icon tiles ~36px, pills 9999px. Shadows soft and color-tinted.
- Motion defaults: ease-out entrance with a gentle settle; rough durations — opening 4s, explainer ~12s, number-pops ~6s, lower-third 4s, link 5s, watch-card ~13s (always adjust to the transcript).

---

## Iconography

1. **Real product logos** as-is — never redrawn or recolored. Metics glyph: white on dark, black (cut-outs read white) on light.
2. **Geometric inline SVG** for generic concepts (envelope, shield, building) — simple, stroke-based.
3. **Flat PNG emoji** for callouts (stopwatch, money bag, check).

---

## Process defaults

- Two-moment skin check before building all beats.
- Build each beat as a cue; review individually; batch change notes.
- **Preview ≠ render:** the iframe preview can misrepresent centering/aspect — reload before reacting.
- Watch for gradient aliasing; re-render if a clip looks low-quality.
- Review the full cut front-to-back on the sequence player over a talking-head placeholder.
- No guides or playback controls in the final render.

---

## Technical contract — do not break (this is what makes clips render)

The repo's `animation-kit/` harness is the strict technical foundation, and it stays exactly as-is. This is the one place with *no* creative liberty — it's what lets clips render to ProRes and composite over the footage.

- Build each clip from the harness (`animation-kit/_template.html`); don't rewrite or replace it.
- Animation must be a pure function of one playhead `t` — deterministic and scrubbable. No CSS `@keyframes`/`transition` driving the final look.
- **Vanilla JS only. Never use JSX or an in-browser compiler** (e.g. `<script type="text/babel">`) — it crashes the 4K renderer.
- Output is ProRes with alpha; keep true transparency on the talking-head gaps.
- Keep the **generic asset library** — product logos, flat-emoji PNGs, device mockups — available for reuse.

(Everything else in this document is about how clips are *made* and how they *look*; this section is about how they're *built to render*, and it never changes.)

---

## Success metric

The system works when a normal video needs only one or two revision passes — because it's built the right *way* every time and Claude Design has room to make good calls, not because the look was pre-dictated.

---

## Per-video vs. system — quick reference

- **Locked (the system):** the build formula; the CTA / link-on-screen format; the SOLID/ALPHA + alpha-gap mechanics; transcript-pinned timing; the ~5s max bare-gap coverage rule.
- **Free, and expected to change every video:** the entire look — color, base, mood, fonts, layout, composition (including non-centered), motion style, motifs, and treatments — themed to the product and chosen for the clearest communication.
