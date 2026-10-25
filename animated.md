# Animated ads, motion graphics, logo stings, interactive, app UI (ce-motion)
Spine and gates: SKILL.md. Defaults: library/motion-graphics.md.

## Types
Product loop (hero pack with light and depth) · hyper-motion graphic ad (parts assemble, callouts, packed final shot) · kinetic type / data · logo + sound sting · stylized / mixed media · real pack over a generated environment loop · 3D turntable (Three.js, real label renders on the real silhouette) · interactive ad · app UI motion.
Footage of people, a cinematic world, or any generated plate is a supplier ticket (SKILL.md §How this engine thinks); this engine adds the graphics over it.

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
- **A · Presets**: Sume presets (product commercial, logo motion, wall-of-text, slideshow) or, only if asked, Higgsfield Marketing Studio; real product and logo as inputs; run on a yes. Concept or draft unless they pass label + frame check.
- **B · Plate + composite**: a video plate ordered by ticket from ce-cinematic (start frame = end frame for a loop), then composite the real pack and logo with tracking so they stay locked to the surface (code, Higgsedit or AE).
- **C · Code-built**: HTML + GSAP / Three.js, deterministic frame recorder, ffmpeg; or HyperFrames / Remotion; or Higgsedit. For kinetic type, data, 3D turntables, scroll-style reveals, app UI motion.
  - Before motion: one key still per beat → animatic (static cuts, real timings, text in place) → legibility check at phone size in every ratio. Frame recorder: seek per frame, local fonts, base64-embedded textures, ffmpeg encode.
- **D · After Effects**: ExtendScript through the app, aerender. For logo stings, tracking, precise text, compositing, editable projects. Route order: core/finish-layer/after-effects/AE-route.md.
  - Flow: brief > Firefly stills (cutouts via Remove background / Creative Production, real alpha) > board approval > build in AE > editable project + linked assets + render. Soundtrack is the master clock: measure beats, cut on them, place boundaries in absolute musical time so frame rounding doesn't add up. Tracking marks computed from the animated transforms, never placed by hand. Native text, shape layers, named layers, precomps. Check the real render for clipping, detached marks, overlaps, flicker, missing footage, beat sync.
- **E · Scale**: native re-layout per ratio; Ad Multiplier for variants from one approved 4–30 s source.

## Data and type
Count-up 800–900 ms ease-out, tabular numbers, no overshoot on numbers; bars fill with the count; badge pops after the bar settles; source line on data cards. Never move text while it's read; hold ≥ max(0.8 s, 0.3 s per word). Words may act out their meaning.

## Logo sting
Real logo file animated; sting per core/tools/routing.md "audio" row (sound.md); ≤ 3 s; reused across the set.

## Brand end card (shared block; ce-cinematic and ce-realism order it by ticket)
- Last 2.5–5 s of a video ad: the real product hero (packshot or approved still, label to camera) + the logo, centered about 35–45% down a 9:16 frame, about 40% of frame width, white or brand color.
- Logo fades in over 8–12 frames on the beat; no bounce, no spin. Optional one line of copy (≤ 4 words) only if the brief has approved copy.
- Out: 3–4-frame white flash or a cut to black. Built in code or After Effects from the vector logo; never generated.
- Safe zones per core/export-table.md for the placement.

## Interactive
States designed on the board (rest, hover, tap, swiped, done). Built in code over finished assets. Each state has a reason (reveal info, show product, confirm action). Delivered as a web piece; for a site, handed to ce-web as a component ticket.

## App UI motion
From real screenshots or real app code only; never model-drawn UI. Exact UI text. Device and lifestyle shots ordered from ce-realism or ce-cinematic.
- HUD stays flat on screen, never in the 3D world. Button micro-physics in numbers ("3 cm button travels 4 mm, firm click"). Screen demo: camera tight on the screen, no scrolling.
- AE dashboard prompt: style + elements + one named AE effect each (counter = Numbers, chart = Linear Wipe, cards = stagger) + idle drift + "all editable layers".
