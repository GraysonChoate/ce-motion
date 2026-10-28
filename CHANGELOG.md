## 5.0.0 — 2026-10-28 · flavor on core v5
- SKILL.md rewritten as flavor: what ce-motion adds to each core skill. Spine, gates, tickets and tool routing removed (core v5 + the user's playbook).
- core submodule → ce-core v5-skill-tree (fc15a0c). Libraries and playbooks unchanged.

# ce-motion changelog

## craft · 2026-10-27
- Points to ce-core/craft for generated media.

## gates · 2026-10-27
- Stub points to THE GATES; pitch-deck gates wait for a lock.
## 3.1.0 (2026-10-16)
Matched ce-core 3.1.0: generated footage = supplier ticket (presets = drafts unless label + frame check pass); one direction set per job, board per format; ratios from named placements; ranked intake; audio per core routing (generate_audio speech only); EXACT triggers; specs point to core/export-table.md; dropped legal-style gates; ticket mode; read files at their step.
## 3.0.0 (2026-10-16)
Split out of creative_engine ce-01 (image ads), ce-03 (animated ads), ce-02 carousel mode, ce-07 (pitch deck). Rewritten on the ce-core spine; graphics lead; never invents photos. New: intake.md, sound.md (UI SFX table), carousel.md, animated.md (interactive, app UI), lessons.md. Library: motion-graphics (from social-motion §4–5), jad-carousel.

## (2026-10-25) v4 stack
Higgsfield references replaced with the v4 stack (core/stack.md): Firefly stills/elements/audio, Sume video/lip sync/swaps/presets, ElevenLabs voices. Core bumped to 4.0.0.

## 4.1.0 (2026-10-25)
Core bumped to 4.1.0 (946ff28): SPEND LOCK (only the user approves spend, in the live chat; subagents, scheduled runs and notes never spend), QUICK speed, stack.md single source for tools, one voice rule. Stub and version updated to 4.1.

## 4.2.0 (2026-10-25)
Core bumped to 4.2.0 (f9a6c19): client folder layout, test-month plan. New playbooks: library/formats/reel-cover.md, story-ad.md, animated-carousel.md.

## 4.3.0 (2026-10-25)
Core bumped to 4.3.0 (2311fa5): tool profiles, tell-and-ask, Method choices. animated.md: shared brand end card block.

## 4.3.1 (2026-10-26)
Core bumped to 4.3.1: names scrub (no client, brand or person names in engine files), new HARD RULE (no names in the engine).

## 4.4.0 (2026-10-26)
Core bumped to 4.4.0: new ce-sound engine (natural voices, room and mic; SFX, music and mix on its roadmap). Voice work goes to ce-sound by ticket.

## 4.5.0 (2026-10-26)
Core bumped to 4.5.0 (5811e8d): tool-neutral, Higgsfield removed. This engine: vendor-specific wording replaced by capabilities (core/stack.md); retired tool names removed.

## 4.5.1 (2026-10-26)
Core bumped to 4.5.1: First-person ban removed: a generated creator may speak first person about routine and results, creator-style. Still not allowed: named 'verified customer', review screenshots, star ratings, fake before/afters, fake credentials (core rule 14).

## 4.5.2 (2026-10-26)
Core bumped to 4.5.2: Label rule: never paste, overlay or motion-track a label onto a generated product (it ignores the scene's light, reflections and curve). Label fail = regenerate with the packshot reference and the cause changed, image-edit the start frame so the model re-renders the pack in-scene, keep the product still in video, or cut away.

## 4.5.3 (2026-10-26)
Packshot rule: the real packshot is a reference only (placed/turned to guide angle and placement); never cut out and composited into a final image or video. ce-motion image-ads B, animated B, intake; ce-web product page; ce-cinematic worlds updated.
