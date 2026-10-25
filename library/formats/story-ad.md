# Format playbook: Story ad (Instagram / Facebook Stories, 9:16, ≤ 15 s)
Read at step 4 and step 7. §8 goes into the frame check. Template: core/format-playbook.md. Sizes, safe zones, loudness: core/export-table.md (Instagram story row). Animation method: animated.md. Static version: static-image-ad.md (same rules, one frame).
Graphics version of the template: §1 canvas/grid · §2 layout · §3 eye path (by second) · §4 imagery · §5 color · §6 sound · §7 pacing · §8 checks · §9 build skeleton · §10 references.

## 0. Defaults + known failures
Switches on: 9:16 1080×1920, 6–15 s (one card), works muted, product and offer in the first 2 s, live text, CTA sticker zone kept clear at the bottom.
Known failures → prevention:
- Key text under the profile bar or the "Learn more" / swipe-up button → safe zone §1.
- Logo or product appears only at the end → product by 2 s, logo by 3 s.
- Needs sound to make sense → silent-first; captions for every spoken word.
- Squeezed from 4:5 or 16:9 → native 9:16 layout.

## 1. Canvas and grid
- 1080×1920. Keep all text, product and logo between y 269 and y 1536 (top 14%, bottom 20% clear) and 65 px from the sides.
- Bottom 20% stays empty for the platform CTA button.

## 2. Layout and hierarchy
- Per frame: 1 visual + 1 line of text (≤ 7 words). Max 3 text beats across the ad.
- Type: headline 80–110 px, support 44–52 px, CTA line 48–56 px.
- Logo once, small (≤ 6% height), top area inside the safe zone, on screen by 3 s.

## 3. Eye path by second (15 s card)
| Time | Job |
|---|---|
| 0–2 s | Hook: product or person + promise text |
| 2–6 s | Proof or how it works (one beat) |
| 6–11 s | Benefit or offer (one beat) |
| 11–15 s | CTA line + product hold (pointing down to the button) |
A 6 s version keeps rows 1 and 4 only.

## 4. Imagery
- Real packshot (Asset Studio) or approved footage; people/scenes by ticket (ce-realism phone-real looks native in Stories; ce-cinematic for polished). Quote under SPEND LOCK.
- Product held, used or on a surface with a contact shadow; never floating.

## 5. Color
Brand palette, one accent (CTA). Text panel or 40–60% scrim over footage. Contrast ≥ 4.5:1.

## 6. Sound
Silent-first. If sound: music bed (platform library, generated or supplied) + optional voice; −14 LUFS; captions burned in inside the safe zone for every spoken word.

## 7. Pacing
A cut or a motion change every 1.5–3 s. Text stays on screen ≥ 1.5 s per 5 words. Nothing moves while it is being read. Last 1.5 s holds still.

## 8. Frame check additions (fail any = rebuild)
- [ ] Text, product or logo outside y 269–1536 or within 65 px of a side.
- [ ] Product not visible by 2 s; logo not visible by 3 s.
- [ ] Doesn't make sense muted; a spoken word without a caption.
- [ ] More than one line of text on screen at once (except CTA + price).
- [ ] Text moving while it is read; text on screen shorter than 1.5 s per 5 words.
- [ ] Label garbled; text baked into generated footage.
- [ ] Squeezed/scaled from another ratio.
- [ ] Offer or price not live; claim not approved; fake review or result.
- [ ] Over 15 s for one card; loudness off −14 LUFS ±1.

## 9. Build skeleton
`Story · [6/15] s · hook "[≤7]" · beat2 "[≤7]" · beat3 "[≤7]" · CTA "[≤4]" · visual [TICKET-IDs / packshot] · sound [none/bed/voice] · route [code / AE / Canva]` → MP4 H.264 1080×1920 30 fps + a still first-frame PNG.

## 10. References
Meta Ad Library, filtered to Stories placement: 5 in-niche ads running 30+ days; note second-by-second beats and where the product first appears.

## Lessons
- none yet
