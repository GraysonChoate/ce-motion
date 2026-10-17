# Format playbook: Instagram carousel (ce-motion)
Read at step 4 (board) and step 7 (audit, every slide). §8 goes into the frame check. Template: core/format-playbook.md. Method and slide rules: carousel.md (static + live), library/motion-graphics.md §4, library/jad-carousel.md (live). Sizes, slide count, safe zone: core/export-table.md. This file adds the numbers a designer works to; it does not restate those.
Graphics version of the template: §1 canvas/grid · §2 layout · §3 eye path · §4 imagery · §5 color · §6 sound (live only) · §7 sequence · §8 checks · §9 build skeleton · §10 references.

## 1. Canvas and grid (what every slide is built on)
- Master 1080×1350 (4:5). 1:1 only if the brief says so. All slides one ratio (slide 1 sets it).
- Safe margin 8% (export table) = 86 px left/right, 108 px top/bottom. Nothing readable outside it.
- Grid crop: the profile grid shows slide 1 at 3:4 = center ~1012 px wide. Slide 1 title and subject sit inside x 120–960.
- 6 columns, 24 px gutters, inside the margins. Baseline 8 px. Same grid on every slide.
- Elements that cross into the next slide (a line, a ball, a card) break exactly at x = 1080 and resume at x = 0 on the next slide, same y.

## 2. Layout and hierarchy (who wins on each slide)
- One idea per slide. 3–5 chunks, headline ≤ 8 words (carousel.md).
- 4 type sizes max. Starting scale at 1080 wide: headline 80–110 px · subhead 44–52 · body 32–38 · label/eyebrow 22–26 (caps, +4% tracking).
- Body ≤ 30 words per slide; line length ≤ 32 characters at body size.
- Fixed furniture in the same spot every slide: eyebrow/slide number ("02 / 08") top-left, logo or handle bottom-left or bottom-right (≤ 60 px tall), never both corners.
- Cover readable at 200 px wide: headline ≥ 80 px at master.

## 3. Eye path (reading order inside a slide and across the swipe)
- One entry point per slide: the headline or the subject, never both the same size.
- Order: entry (top third) → support (middle) → pointer to next slide (right edge).
- Slide 1: hook + a swipe cue (arrow, "→", or an element cut off at the right edge).
- Last slide: the CTA is the entry point.

## 4. Imagery (how photos and people are ordered)
- Motion never makes a photo: every person/lifestyle/scene by ticket from ce-realism, ce-cinematic or Asset Studio (SKILL.md).
- Each ticket names: ratio 4:5, ≥ 2160×2700 px (2× master), which zone stays clean for text (e.g. "top 40% plain"), light direction, and "no text, no logos, no labels in the image".
- One lighting and color grade across all photo slides (same ticket locks, same time of day).
- Products: real transparent packshot, on a measured surface line with a contact shadow (SKILL.md step 5).
- Flat images for live slides: rebuilt in layers first (bg, cut-out subject, text, cards).

## 5. Color and contrast
- Brand palette only, one role per hex. 60/30/10: background / secondary / one accent. The accent marks one thing per slide.
- Contrast: body ≥ 4.5:1, headlines ≥ 48 px ≥ 3:1 (WCAG AA). Check on the actual pixels behind the text.
- Text on photo: solid panel or a 40–60% scrim, never bare over busy detail.

## 6. Sound (live carousels only; static has none)
One song across all slides, whole bars per slide: carousel.md + library/jad-carousel.md + sound.md. Must work muted.

## 7. Sequence and pacing (across slides)
- 7–10 slides default (export table caps at 20). Arc per carousel.md: hook > problem > turn > proof > payoff > CTA.
- Slide 2 must also work as a hook (Instagram may re-show the post starting at slide 2).
- Each slide readable in 3 s. No two text-only slides in a row longer than 3.
- Live: each slide a whole number of bars (6–8 s at 120 BPM), last frame = first frame; nothing moves while being read.
- Rebuild slide 1 at 9:16 if a Reel is named.

## 8. Frame check additions (fail any = rebuild that slide)
- [ ] Slide 1 title or subject cut by the 3:4 grid crop (outside x 120–960).
- [ ] Any text inside a generated image (baked-in headline, fake label, garbled letters, fake UI). Text must be live.
- [ ] Product label differs from the real packshot by any letter.
- [ ] Margins differ between slides by > 4 px, or text outside the 86/108 px safe margin.
- [ ] Eyebrow, slide number or logo jumps position between slides.
- [ ] More than 4 type sizes, or more than one accent color on a slide.
- [ ] Headline > 8 words, or cover not readable at 200 px wide.
- [ ] Contrast below 4.5:1 (body) / 3:1 (≥ 48 px).
- [ ] Cross-slide element misaligned at the seam (> 2 px off in y, or gap at x = 1080).
- [ ] Photo slides with different light direction or grade.
- [ ] Wrong font (fallback rendered) or hex not in the palette.
- [ ] Live: loop jumps, cut not on a bar, text moving while read.
- [ ] Generic AI look: stock-like people, purple gradients, glossy 3D blobs not in the brand.

## 9. Build skeleton (reuse word for word)
Board row per slide: `S[nn] · role [hook/problem/turn/proof/payoff/CTA] · headline "[≤8 words]" · support "[≤30 words]" · visual [TICKET-ID or code] · accent on [one thing] · live: bars [n], move [one lead move] on beat [n].`
Supplier ticket: `[Engine] still, 4:5, 2160×2700. [Subject + action]. [Lock IDs]. Light from [side], [K] K, same grade as [TICKET-ID]. Keep [top/left xx%] plain for text. No text, no logos, no labels, no watermarks in the image.`
Code: one HTML per slide, 1080×1350, local fonts, shared CSS tokens (palette, 4 type sizes, 86/108 px margins, 6-col grid); export PNG (static) or MP4 per slide via HyperFrames (live).

## 10. References (study at step 2)
5 best-in-niche carousels (ce-core research): note slide count, hook words, type sizes measured in px, grid, where the swipe cue sits, slide 2. Jad M.H live builds (library/jad-carousel.md). To verify before relying on it: 3:4 (1080×1440) carousel uploads; export table still says 4:5 or 1:1.

## Lessons (one line per real mistake, then fixed above)
- none yet
