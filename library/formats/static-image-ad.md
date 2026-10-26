# Format playbook: Static image ad (ce-motion)
Read at step 4 (concept matrix) and step 7 (audit, every concept × ratio). §8 goes into the frame check. Template: core/format-playbook.md. Angles and routes (A fast · B locked-pack composite · C Canva): image-ads.md. Placements, sizes, safe zones: core/export-table.md. This file adds the designer's numbers; it does not restate those.
Graphics version of the template: §1 canvas/grid · §2 layout · §3 eye path · §4 imagery · §5 color · §6 sound (none) · §7 set and ratios · §8 checks · §9 build skeleton · §10 references.

## 1. Canvas and grid
- Master = the primary placement's ratio (export table). Usual: 4:5 1080×1350 feed, 9:16 1080×1920 story/reel, 1:1 1080×1080.
- Safe zones from the export table. 9:16: keep text and pack between y 269–1248 (top 14%, bottom 35% for Reels) or y 269–1536 (stories, bottom 20%); 65 px each side.
- Margin on 4:5 and 1:1: 64 px min all sides. 6 columns, 24 px gutters, baseline 8 px.
- Every ratio laid out natively (SKILL.md step 6): never scaled or squeezed from another ratio.

## 2. Layout and hierarchy (3 things, in this order)
- 1 visual (product or proof) · 1 headline · 1 CTA. Optional: subline, price/offer badge, logo. Nothing else.
- Headline ≤ 7 words; subline ≤ 12 words; CTA 1–3 words. All strings on the exact copy list.
- Type at 1080 wide: headline 72–120 px · subline 36–48 · CTA/button 32–40 · legal 20–24. 3 sizes + legal max.
- Visual takes 50–70% of the frame. Text area light (Meta recommendation, not a rule): aim ≤ 20% of the frame.
- Logo once, ≤ 8% of frame height, with brand clearspace. CTA as a button or a clear line, bottom third.

## 3. Eye path (0–2 s)
- Visual first → headline → CTA. Z or top-down; one entry point.
- Thumb-stop test: at 300 px wide, you can say what it is and the offer in 1 s.
- The product faces or points toward the headline, not off the frame.

## 4. Imagery (how it is ordered)
- Route per concept from image-ads.md. Label must be exact → route B.
- Scene/people/lifestyle = supplier ticket (ce-cinematic styled, ce-realism phone-real); packshot = Asset Studio transparent PNG.
- Ticket names: ratio, 2× size (≥ 2160 px short edge), the clean text zone per ratio, surface line height, light direction and K, "no text, no logos, no labels, no packaging in the scene" (pack is composited).
- Order one master scene that leaves room for every named ratio, or one per ratio when framing matters (export table, "Make once, cut many"), quoted.

## 5. Color and contrast
- Brand palette, one role per hex; one accent (CTA or offer). 60/30/10.
- Contrast: body ≥ 4.5:1, headline ≥ 48 px ≥ 3:1, CTA button text ≥ 4.5:1 on the button.
- Text over photo: panel or 40–60% scrim. Background differs from the pack color by ≥ 3:1 so the pack reads.

## 6. Sound
None. A static ad is silent. If motion is asked, it is an animated ad: animated.md.

## 7. Set and ratios (pacing across the ad set)
- Step 3: 3 directions → pick 1 → 3+ concepts from different angles (image-ads.md). One row per concept × ratio in the matrix.
- Within a concept, variants change one thing only (headline, visual or offer) so tests read.
- Same type scale, palette, logo spot and CTA style across the set.

## 8. Frame check additions (fail any = rebuild that piece)
- [ ] Text baked into a generated image (headline, price, fake label, garbled letters). All text live.
- [ ] Pack label differs from the real packshot by any letter, or the pack is warped/re-drawn.
- [ ] Pack floating: no surface line, no contact shadow, or light from the wrong side.
- [ ] Text, pack or CTA inside a placement's safe zone (export table).
- [ ] Ratio squeezed or scaled instead of re-laid out.
- [ ] More than one headline, CTA or logo; anything inside the logo clearspace.
- [ ] Headline > 7 words; not readable at 300 px wide.
- [ ] Contrast below the §5 numbers.
- [ ] Price, claim or stat not on the real site/label; review quote not real.
- [ ] Wrong font (fallback) or hex not in the palette.
- [ ] Margins inconsistent across ratios of the same concept (> 4 px).
- [ ] Preset draft passed as a final without the label + frame check.
- [ ] Generic AI look: stock people, plastic skin, extra fingers, warped hands on the pack.

## 9. Build skeleton (reuse word for word)
Matrix row: `C[nn]-[ratio] · angle [benefit/proof/routine/offer/comparison/social] · visual [TICKET-ID / packshot] · headline "[≤7]" · subline "[≤12]" · CTA "[1–3]" · route [A/B/C].`
Scene ticket: `[Engine] still, [ratio], [px]. [Scene], empty surface at [y px] for the pack. [Lock IDs]. Light from [side], [K] K. Keep [zone] plain for text. No text, logos, labels or packaging in the image.`
Finish in Canva or code: tokens (palette, 3 sizes + legal, 64 px margin), real packshot layer, live text, export PNG per ratio, contact sheet.

## 10. References (study at step 2)
Meta Ad Library: 5 best-in-niche ads still running 30+ days (a sign they work); measure headline word count, visual share of frame, CTA spot. Brand's own best performer if the user has one.

## Lessons (one line per real mistake, then fixed above)
- none yet
