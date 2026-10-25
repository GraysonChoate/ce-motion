# Format playbook: Reel / TikTok cover (ce-motion)
Read at step 4 and step 7. §8 goes into the frame check. Template: core/format-playbook.md. Sizes and safe zones: core/export-table.md. Default speed: QUICK (one still), unless it is part of a larger job.
Graphics version of the template: §1 canvas/grid · §2 layout · §3 eye path · §4 imagery · §5 color · §6 sound (none) · §7 series · §8 checks · §9 build skeleton · §10 references.

## 0. Defaults + known failures
A cover is the thumbnail that sells the tap from the profile grid and from search. Switches on: 9:16 master, everything that matters inside the center 3:4 crop, live text, the frame taken from the reel itself (or its exact look).
Known failures → prevention:
- Title cut off on the profile grid (it shows the center 3:4) → title and subject inside x 0–1080, y 240–1680 (§1).
- Cover promises something the reel doesn't deliver → the title is the reel's own hook, word for word or shorter.
- Generated cover that doesn't match the reel's people or product → use a real frame from the cut; generate only if no frame works, with the same locks.
- Series covers look different every week → fixed template (§7).

## 1. Canvas and grid
- 1080×1920 (9:16). Profile grid crop = center 1080×1440 (3:4) → keep title and subject inside y 240–1680.
- Inside that, keep text 65 px from each side. Title block sits in the upper half of the 3:4 crop (y 360–900) so the grid's view count and pin icons don't cover it.

## 2. Layout and hierarchy
- One subject (face, product or result) + one title (≤ 5 words, 2 lines max) + optional series tag ("EP 03", "DAY 12/30").
- Title 96–140 px at 1080 wide, heavy weight, high contrast; tag 36–44 px.
- Product: real packshot or the real frame, label readable at 200 px wide or cropped off entirely.

## 3. Eye path
Face/product → title. Readable at 200 px wide (grid size on a phone) in 1 s.

## 4. Imagery
- Order of preference: (1) a real frame from the reel at the hook moment (ffmpeg, full res), (2) a re-shot still with the same locks, (3) a generated still on the same locks (SPEND LOCK quote).
- Faces: eyes open, expression matches the hook; no motion blur.
- Background simplified or darkened 20–40% behind the title; never a busy patch behind text.

## 5. Color
Brand palette; one accent for the tag or one keyword. Title contrast ≥ 4.5:1 against what's behind it (panel or scrim if not).

## 6. Sound
None.

## 7. Series template (when covers repeat)
Fixed: title position, type size, tag spot, accent color, face/product side. Changes per post: the frame and the words only. Checked side by side with the last 6 covers on a grid mock.

## 8. Frame check additions (fail any = rebuild)
- [ ] Title or subject outside the 3:4 grid crop (y 240–1680).
- [ ] Title over 5 words or unreadable at 200 px wide.
- [ ] Title not the reel's actual hook (promise mismatch).
- [ ] Person, product or setting differs from the reel.
- [ ] Label garbled or redrawn; text baked into a generated image.
- [ ] Contrast below 4.5:1; fallback font.
- [ ] Series cover breaks the fixed template (§7).

## 9. Build skeleton
`Cover · reel [id] · frame [timecode or TICKET-ID] · title "[≤5]" · tag "[optional]" · subject side [L/R/center] · template [series name]` → built in code or Canva, PNG 1080×1920, plus a 3:4 grid preview.

## 10. References
The account's own grid (consistency) and 3 accounts in the niche with strong grids; note title length, face vs product covers, and which covers led their best-viewed reels.

## Lessons
- none yet
