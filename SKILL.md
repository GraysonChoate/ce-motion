---
name: ce-motion
description: The motion design engine. Carousels (static and live), image ads, animated ads, kinetic type, product loops, logo stings, interactive ads, pitch decks. No footage of its own: it lays out and animates, and orders every photo, person or clip by ticket from ce-realism, ce-cinematic or Core's Asset Studio. Assembler. Runs the ce-core spine.
version: 3.0.0
---
> Load ce-core first. Always on: quote credits before spend (routing row, every input slot named, takes max); real label only, checked against the real image; brand text in code; real people fine when the user says approved; locks before any clip; build only approved tickets; retake cap 2; report tool failures; see it before approval; WAKE-UP at every stop.

# CE-MOTION v3
Read every run: intake.md · sound.md · library/motion-graphics.md. Per format: image-ads.md · carousel.md · animated.md · pitch-deck.md. Carousel rhythm: library/jad-carousel.md. After Effects: core/finish-layer/after-effects/.

## How this engine thinks
Graphics lead the board: the layout, type and motion are the work. Motion design **never invents a photo**: every person, lifestyle shot or clip is ordered by ticket from the engine whose look it needs (phone-real → ce-realism, styled campaign → ce-cinematic, product on a tile → Asset Studio). Text is set in code or the editor, never generated. Every move has a job: show the product or reveal information. Silent-first: it must work with the sound off; sound (UI clicks, whooshes, coin chimes, swipes) makes it land when it's on.

## Formats
| Format | File | Lead | Clock |
|---|---|---|---|
| Static image ad | image-ads.md | Graphics | one frame per ratio |
| Static carousel | carousel.md | Graphics | slides |
| Live carousel (looping video slides, one song) | carousel.md | Graphics + Beat | slides × bars |
| Animated ad / product loop / hyper-motion graphic | animated.md | Graphics | seconds |
| Kinetic type / data / explainer graphics | animated.md | Graphics | seconds, on the beat |
| Logo sting | animated.md §Logo | Graphics + Sound | ≤ 3 s |
| Interactive ad (hover, tap, swipe states) | animated.md §Interactive | Graphics | states |
| App UI motion (from real screenshots or code) | animated.md §App UI | Graphics | seconds |
| Pitch / concept deck | pitch-deck.md | Beat | slides |

## Step 1 · Prepare
ce-core intake + intake.md. Brand tokens from the bible: hex palette with one role per color, type scale, logo files, motion words (3 adjectives for speed and feel), clearspace. Asset Studio: real packshots (transparent PNG), vector logo, product cutouts. Load local font files before anything renders.

## Step 2 · Research
ce-core research: 5 best-in-niche ads or carousels: hook, layout, motion, length. Match / beat, one line each.

## Step 3 · Ideate (gate: pick 1 of 3)
Three directions, safe → bold, each one key frame at the main ratio: TAME clean packshot + type · NEW DIRECTION editorial/lifestyle layout · SPECTACULAR in-motion composite or hyper-motion.

## Step 4 · Map (gate: approve board + tickets)
- Concept matrix (one row per piece): angle × product × ratio, with hook, headline, subline, CTA.
- Board on six tracks; Graphics leads. For video: a beat sheet in seconds (0–2 s hook, proof beats, CTA, end card); between beats a SEAM (an in-frame event carries the change, not a cut). For carousels: one row per slide.
- **Exact copy list**: every on-screen string quoted; "nothing else appears".
- Motion spec (from motion words): easing, one lead move + small supporting staggers, overshoot (≤ 6% UI, ≤ 13% headlines, none on numbers; none for luxury), blur only while moving, holds long enough to read.
- Sound track designed (sound.md).
- Tickets: every photo/person/clip ordered from a supplier engine with its look, size, text space and locks; code/layout pieces as free tickets. Credits quoted.

## Step 5 · Build pieces
Supplier pieces arrive by ticket and are checked on receipt. Here: layouts, type, motion, composites. Routes per format file: Canva (templated text + resize), code (HTML + GSAP/Three.js rendered by a frame recorder; HyperFrames or Remotion), After Effects (tracking, logo stings, layered comps, editable project), Higgsfield Ads Studio or Marketing Studio presets (fast concepts, run only on a yes, checked like anything else). Products placed on a measured surface line with a contact shadow and matching light; never floating.

## Step 6 · Assemble
Every ratio laid out natively (never squeezed): 1:1, 4:5, 9:16, 16:9 from the export table. Soundtrack is the master clock for anything timed: measure its beats, then cut. Captions only where speech exists.

## Step 7 · Audit + deliver
- Frame sheet every 0.25 s (video) or every slide: label matches the real packshot letter by letter; product on its surface; logo clearspace; text in safe zones and under ~20% of an ad image; hex sampled; fonts are the real files.
- Motion QA: easing matches the motion words; loop seam invisible; no flicker; no flashing above 3/s; no judder.
- Sound-off test; phone-size legibility test (cover readable at 200 px wide); −14 LUFS for social.
- EXACT: fresh pass + gauntlet.
- Deliver: every ratio, clean masters, editable source (Canva link, code, or AE project), contact sheet, file names per core/naming.md. Ledger line, WAKE-UP.

## Rules (this engine)
- Motion design never generates a person or a lifestyle photo itself; it orders one.
- Real brand text in code or the editor; exact copy list on every piece.
- Brand palette and fonts only; local font files.
- One lead move at a time; nothing moves while it's being read.
- Silent-first, sound-ready.

## Extra failures (shared ones in ce-core §8)
| Problem | Fix |
|---|---|
| Looks templated / generic | Real product photos and real brand worlds; one strong idea per piece; cut decoration. |
| Text unreadable on phone | Fewer words, bigger type, 4 sizes max; test at real size. |
| Motion feels busy | One lead move; slow the easing; remove secondary motion. |
| Ratio looks squeezed | Re-lay out natively per ratio. |
| Supplier photo doesn't fit the layout | Back with ticket ID + failing field (text space, crop, light). |
| Loop jumps | Whole bars per slide; last frame = first frame; verify numerically. |
