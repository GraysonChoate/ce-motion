# Code-built ads — the proven pipeline (route C, in depth)

Learned on the Grounded Labs ad program (Oct 2026: Gravity, The Mess, Spark, Overnight Shift, Every PDF, 700 Tickets, Sphere). Brand-agnostic: swap fonts, colors and logo per brand. $0: code + owned tools, no generated images, video or stock.

## When to use it
One pain → one fix, said with type, shapes, UI, data or 3D that code can draw exactly. Exact brand type and logos. Many variants for testing (a piece is a template: swap hook, industry, numbers, words).
Not for: real people, real places, liquids (order those from ce-realism / ce-cinematic).

## Story spine (the "mom test")
WHO (a recognisable owner) → PROBLEM (what piles up) → COST (hours, money, missed moments) → FIX (what the system does) → RESULT (the human payoff) → CTA (a concrete free offer). Pain hook in the first 0.5–2 s. If someone's mom can't say what the business does after one watch, rewrite.
Words: plain job-site language ("hours back", "missed calls caught", "paid faster", "one system"). Never lead with jargon ("AI-powered", "transform", "revolutionize", "leverage").

## Format defaults (defaults, not rules — test lengths per platform)
- 9:16 1080×1920 master, 60 fps; cut 16:9 / 1:1 natively when needed.
- Sound-off first: every key line is on-screen text. Text holds ≥ max(1.0 s, 0.3 s per word).
- Safe area: ≥90 px sides; clear of the top ~200 px and bottom ~300 px (platform UI).
- Frame 0 already shows motion or content — never black or empty.
- ONE ground per piece (all dark or all light); mixing reads as two ads.
- Encode: H.264 -preset veryfast -crf 18, yuv420p, AAC 48 kHz.

## Build pipeline
1. **Beats file = one clock.** A single beats/timing file drives picture, captions and sound, so they never drift.
2. **Deterministic render(t).** The scene is a pure function of time; a Playwright frame-stepper seeks each frame and saves PNGs; ffmpeg encodes. Canvas 2D or Three.js (vendored locally; CDNs may be blocked).
3. **Crash guard.** Frames go to disk; on a crash the renderer relaunches and resumes from the last saved frame. A watchdog checks long renders every ~2 min and restarts stalls.
4. **Sound** is synthesized from the same beats file: ≤ ~1 lead cue per second, layered SFX (tick, whoosh, thud), peak ≈ −1 dBFS; quiet beats on purpose (e.g. −20 dB for a punchline).
5. **Logo** from the brand's official SVG paths only (never redrawn); the 3D or animated version must match the SVG silhouette at the lock frame.

## Process (fast loop)
- Design with preview stills and contact sheets (8–12 key moments), not full renders. Check mid-transition frames, text collisions, safe area.
- Prove the build with a short test (~60 frames), then run the full render as a background job.
- Fix by pointing at frames ("frames 253–255: no blur on contact"), one version per round, logged in the brief.

## Render cost (measured)
Canvas 2D ≈ 2–3 min per 15 s; Three.js with motion blur ≈ 10–30 min. Fast 2D styles suit high-volume testing; save 3D for hero pieces.

## Lessons (from the version logs)
- Big objects make physics hit harder; small builds look like UI, not events.
- Overcorrecting (darker, emptier) is common after a fix round: lift light, keep the end frame full.
- Chaos scenes must overwhelm (fill the frame); the "order" beat earns its relief from that contrast.
- Frame rate can tell the story: chaos at 12 fps (stop-motion jitter) → order at 60 fps.
- Glow: an orange-only ramp with cream cores; avoid white/pink blowout.
- Count-ups: 800–900 ms ease-out, tabular numbers, no overshoot, hold each stat ≥ 1.2 s.
- End card: lockup ~70–75% width, one CTA line, URL in a mono face.
- Never name real clients on screen unless approved.
