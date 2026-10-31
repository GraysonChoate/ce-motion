---
name: ce-motion
description: The motion design flavor on top of ce-core v5. Carousels (static and live), image ads, animated ads, kinetic type, product loops, logo stings, interactive ads, app UI motion, pitch decks. Lays out and animates; never invents a photo: every person, scene or clip is ordered from the engine whose look it needs. Adds to each core skill; removes none.
version: 5.1.0
---
> Load ce-core first (its SKILL.md, then the user's playbook). Core's three floor rules hold: show before build, price before spend, see it. This file only adds the motion-design way of doing each step.

# CE-MOTION v5 — flavor

## How this engine thinks
Graphics lead: the layout, type and motion are the work. Motion design never invents a photo: every person, lifestyle shot or generated scene is ordered from the engine whose look it needs (phone-real → ce-realism; styled → ce-cinematic; packshot cutouts → core asset-studio). Text is set in code or the editor, never generated. Every move has a job: show the product or reveal information. Silent-first: it works with the sound off; sound (UI clicks, whooshes, swipes) makes it land when it's on.

## Formats (playbooks in library/formats/, read at storyboard)
| Format | File | Clock |
|---|---|---|
| Static image ad | image-ads.md · static-image-ad.md | one frame per ratio |
| Static carousel | carousel.md · instagram-carousel.md | slides |
| Live carousel (looping video slides, one song) | carousel.md · animated-carousel.md · library/jad-carousel.md | slides × bars |
| Animated ad / product loop / hyper-motion graphic | animated.md · story-ad.md | seconds |
| Kinetic type / data | animated.md | seconds, on the beat |
| Logo sting | animated.md §Logo | ≤ 3 s |
| Interactive ad | animated.md §Interactive | states |
| App UI motion | animated.md §App UI | seconds |
| Pitch / concept deck | pitch-deck.md | slides |
Explainers go to ce-cinematic. Two formats in one job: one set of three directions, one board per format. Motion can supply finished loops, stings and components to ce-web.

## What motion adds to each core skill
**brief** — Brand tokens from the bible: hex palette with one role per color, type scale, logo files, three motion words (speed and feel), clearspace. Real packshots as transparent PNGs, vector logo. Local font files loaded before anything renders.

**reference** — Five best-in-niche ads or carousels: hook, layout, motion, length; match or beat, one line each. For hyper-motion graphics, the physics reference is still real footage of the thing moving.

**storyboard** — Concept matrix, one row per piece: angle × product × ratio with hook, headline, subline, CTA. Board with graphics leading; video gets a beat sheet in seconds (0–2 s hook, proof beats, CTA, end card) with a SEAM between beats (an in-frame event carries the change, not a cut); carousels get one row per slide. **Exact copy list**: every on-screen string quoted, "nothing else appears". Motion spec from the motion words: easing, one lead move plus small staggers, overshoot ≤ 6 % UI, ≤ 13 % headlines, none on numbers, none for luxury; blur only while moving; holds long enough to read. Sound track designed (sound.md). Three directions: clean packshot + type · editorial layout · in-motion composite or hyper-motion. Recurring characters or worlds (an explainer series, a mascot, an episodic social show) reuse the same locks across every piece (core storyboard §8).

**physics** — library/motion-graphics.md: products sit on a measured surface line with a contact shadow and matching light; a hyper-motion graphic obeys the same mass and cause rules as a filmed one.

**image-prompting / video-prompting** — Only via tickets to the supplier engines, with the look, size, text space and locks named. Tool presets (one-click ad templates): concept drafts only; a final only if it passes the label and frame checks.

**sound** — sound.md: UI sounds on the event frame, a swipe per slide change, the soundtrack as the master clock for anything timed (measure its beats, then cut).

**audit** — Frame sheet every 0.25 s or every slide: label letter-perfect against the real packshot; product on its surface; logo clearspace; text in safe zones; hex sampled; fonts are the real files. Motion QA: easing matches the words; loop seam invisible; no flicker; no flashing above 3/s. Sound-off test; phone-size legibility (cover readable at 200 px wide).

**finish** — Every ratio the placements need laid out natively, never squeezed. Routes per format file: templated tools for text and resize; code (HTML + animation libraries rendered by a frame recorder) for exact type and motion; After Effects for tracking, stings and editable layered comps (core finish-layer/after-effects/). Captions only where speech exists.

## Rules (this engine)
Text in code, never generated · never a floating product · one lead move per beat · silent-first · generated footage = a supplier ticket, never made here.
