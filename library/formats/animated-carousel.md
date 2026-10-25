# Format playbook: Animated (live) carousel (ce-motion)
Read at step 4 (board, bar map) and step 7 (audit, every slide looped 3×). §8 goes into the frame check. Template: core/format-playbook.md. Static rules it inherits word for word: library/formats/instagram-carousel.md §1–5. Method: carousel.md §Live carousel and library/jad-carousel.md. Sizes: core/export-table.md.
This file adds only what motion changes: §6 sound · §7 timing and loops · §8 checks · §9 build skeleton.

## 0. Defaults + known failures
Switches on: every slide a seamless video loop, one song across all slides, fixed BPM, every slide a whole number of bars, built in code (HTML + GSAP, deterministic frame render, local fonts) + ffmpeg. Must read fully with sound off.
Known failures → prevention:
- Loop seam jumps → last frame = first frame, checked by playing 3 loops back to back.
- Cuts or hits off the beat → bar map (§7) written before any animation.
- Text moves while it's being read → text animates in, then holds still for its read time.
- Generated footage drifts between slides → one lock set for all photo slides; footage by ticket only (SPEND LOCK).
- Song leaves the platform library or rights unclear → generated, platform library or a user-supplied track only.

## 1–5. Canvas, layout, eye path, imagery, color
As instagram-carousel.md §1–5 (4:5 1080×1350, 8% margins, 3:4 grid-safe cover, ≤ 8-word headlines, 4 type sizes, live text, real packshots, 60/30/10, contrast ≥ 4.5:1).

## 6. Sound
- One track, fixed BPM (default 120 = 2 s per bar). Slide n plays bars from where slide n−1 ended, so swiping feels continuous.
- Hits (pack lands, number ticks up, card flips) on beat 1 of a bar. No voice unless the brief asks.
- −14 LUFS master; each slide's audio cut on a bar line with 10 ms fades.

## 7. Timing and loops
- Each slide 3–4 bars (6–8 s at 120 BPM). Structure per slide: in (1st bar) → hold and read (middle bars) → reset to the first frame (last half bar).
- Read time: hold ≥ 1.5 s per 5 words with nothing moving behind the text faster than 2% of frame width per second.
- Motion grammar (library/motion-graphics.md): eased, weighted, one idea per slide; cross-slide elements continue at the seam (same y, same speed).
- Slide 1 also exported at 9:16 as a Reel opener when asked.

## 8. Frame check additions (fail any = rebuild that slide)
- [ ] Everything in instagram-carousel.md §8.
- [ ] Loop seam visible (frame 1 ≠ last frame) on a 3× loop.
- [ ] A slide length not a whole number of bars; a hit not on a beat (> 1 frame off).
- [ ] Text moving during its read time; held text shorter than 1.5 s per 5 words.
- [ ] Slide doesn't make sense muted.
- [ ] Cross-slide element jumps at the seam (> 2 px or speed change).
- [ ] Fallback font in rendered frames (render from local font files).
- [ ] Music source not generated, platform library or user-supplied.

## 9. Build skeleton
Bar map row: `Slide [n] · bars [a–b] · in "[move]" (bar a) · hold "[text ≤8]" · hit "[event]" on bar [x] beat 1 · reset (last ½ bar) · visual [TICKET-ID / code]`
Render: HTML + GSAP timeline per slide → deterministic recorder at 30 fps → ffmpeg H.264 1080×1350 + slice of the song per slide → preview page with all slides in a swipe mock.

## 10. References
3 live carousels in the niche (save each slide as video); note BPM, bars per slide, where text holds, and how slide 1 hooks.

## Lessons
- none yet
