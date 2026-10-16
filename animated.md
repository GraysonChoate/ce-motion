# Animated ads, motion graphics, logo stings, interactive, app UI (ce-motion)
Spine and gates: SKILL.md. Defaults: library/motion-graphics.md.

## Types
Product loop (hero pack with light and depth) · hyper-motion graphic ad (parts assemble, callouts, packed final shot) · kinetic type / data · logo + sound sting · stylized / mixed media · real pack over a generated environment loop · 3D turntable (Three.js, real label renders on the real silhouette) · interactive ad · app UI motion.
If the piece needs footage of people or a cinematic world, that footage is a ticket to ce-realism or ce-cinematic; this engine adds the graphics over it.

## Brief (written at step 4; one line per part)
1. FORMAT: length, ratio, fps (60 for code-built graphics), silent or not.
2. PALETTE: locked hex, one role per color.
3. LOCKS: hero and what persists (the pack never changes; a stack only grows).
4. CAMERA: allowed / forbidden moves.
5. MOTION RULES: easing; blur only while moving; one lead move; overshoot limits.
6. BEAT SHEET: seconds; seams between beats.
7. EXACT COPY: every string quoted; nothing else appears.
8. AUDIO: soundscape, music BPM, SFX cues with times.
9. HOLD + END STATE: last beat held; end card exact.

## Routes
- **A · Presets**: Marketing Studio motion presets (hyper-motion, 2D motion, mixed media, SaaS motion); real product and logo as inputs; run only on a yes; check like any route.
- **B · Generated plate + composite**: a video plate (start frame = end frame for a loop), then composite the real pack and logo with tracking so they stay locked to the surface (code, Higgsedit or AE).
- **C · Code-built**: HTML + GSAP / Three.js, deterministic frame recorder, ffmpeg; or HyperFrames / Remotion; or Higgsedit. For kinetic type, data, 3D turntables, scroll-style reveals, app UI motion.
- **D · After Effects**: ExtendScript through the app, aerender. For logo stings, tracking, precise text, compositing, editable projects. Route order: core/finish-layer/after-effects/AE-route.md.
- **E · Scale**: native re-layout per ratio; Ad Multiplier for variants from one approved 4–30 s source.

## Data and type
Count-up 800–900 ms ease-out, tabular numbers, no overshoot on numbers; bars fill with the count; badge pops after the bar settles; source line on data cards. Never move text while it's read; hold ≥ max(0.8 s, 0.3 s per word). Words may act out their meaning.

## Logo sting
Real logo file animated; sound sting from generate_audio; ≤ 3 s; reused across the set.

## Interactive
States designed on the board (rest, hover, tap, swiped, done). Built in code over finished assets. Each state has a reason (reveal info, show product, confirm action). Delivered as a web piece; for a site, handed to ce-web as a component ticket.

## App UI motion
From real screenshots or real app code only; never model-drawn UI. Exact UI text. Device and lifestyle shots ordered from ce-realism or ce-cinematic.
