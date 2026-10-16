# Carousels (ce-motion)
Spine and gates: SKILL.md. Rhythm method: library/jad-carousel.md.

## Static carousel
- 4:5 1080×1350 (or 1:1), up to 10 slides (20 allowed; 10 is the default).
- Slide 1 is the hook; the profile grid crops to 3:4, so the title sits centered.
- Each slide readable in 3 s: headline ≤ 8 words, 3–5 chunks, one accent color, 4 type sizes max. Cover readable at 200 px wide.
- Story across slides: hook > problem > turn > proof (product) > payoff > CTA on the last slide. Story check runs on slides.
- Photos and people ordered by ticket; flat images rebuilt in layers first.
- Built in code (HTML) or Canva; text always live.

## Live carousel (looping video slides, one song)
- Every slide a looping video; one song runs across all slides; each slide takes the next bars of the song.
- Fixed BPM (default 120 = 0.5 s per beat). Every slide a whole number of bars (3–4 bars = 6–8 s). Last frame = first frame. Hits, flips and bounces land on beats.
- Design silent-first; the song is the bonus.
- Built in code: HTML + GSAP rendered frame by frame (deterministic recorder, local fonts) + ffmpeg. One MP4 per slide + a preview page.
- Rebuild slide 1 at 9:16 to reuse as a Reel.

## Sound
Per sound.md: one song for live carousels; UI SFX optional on reel cutdowns.
