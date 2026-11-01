# Viral type techniques (graphics over a talking person)
Read at storyboard (step 3) for any talking-head reel, creator ad or explainer that carries graphics. Studied from high-performing creator reels, Oct 2026; no creator names kept. Each technique: what it is · why it spreads · how to build it. Pick 2–4 per piece, never all; one technique per line of script. Graphics stay generic and on-brand; text is set in code or After Effects, never generated (SKILL.md Rules).

## Techniques
| # | Technique | What it is | Why it spreads | Build notes |
|---|---|---|---|---|
| T1 | Type placed in the room | words stand in the 3D space of the shot (beside the head, on a wall, on the floor), appearing word by word, top third | reads as part of the world, not a sticker; the eye stays near the face | track or match the camera (AE 3D camera tracker, or a locked shot + a fixed 3D layer); perspective, light and a soft contact shadow match the room; word on the spoken word (rule C2) |
| T2 | Phone UI as an object | a notification, DM or payment card appears in the scene as a real object, then is flicked or thrown out | everyone knows the UI at a glance; a familiar card = instant context and a little dopamine | build the card in code at real UI size (rounded corners, system font, real-looking but generic app); give it mass: a throw has an arc, spin and motion blur; one SFX on arrive and exit (T8) |
| T3 | New camera angle per line | each script line cuts to a new angle of the same talk | constant visual change holds attention without B-roll | one locked master, then re-angles by timestamp (ce-realism SKILL.md video-prompting); punch-ins and zooms in post; cut on the line, never mid-word |
| T4 | Shrink to card | the video shrinks into a rounded UI card (a post, a window, a phone screen) that then moves aside for the next graphic | turns the speaker into "content" and frames the next point; feels like an app | scale 100 → 40–60% with ease-in-out 0.4–0.6 s, corner radius grows as it shrinks, drop shadow appears; the card keeps playing |
| T5 | Hand out of the phone | a hand (or object) reaches out of a phone screen into the room | breaks the frame; the "how did they do that" pause drives rewatches | phone screen = masked layer; the hand is a separate plate or cut-out composited over the screen edge; matched light and shadow on the room side |
| T6 | Text on or through the lens | type sits on the glass (smudge, reflection) or the person reaches through or wipes it away | the viewer feels addressed directly; interaction = surprise | the person's hand is rotoscoped to pass in front of or behind the type layer; a faint glass reflection on the type sells it |
| T7 | Ghost or duplicate self | a second, semi-transparent or full copy of the speaker reacts, disagrees or finishes the line | a two-voice argument in one person is fast, funny and easy to follow | locked-off camera, two passes of the same set (or one master + a re-performed segment); split mask or opacity 40–70% for a ghost; eyelines meet |
| T8 | SFX on every graphic beat | each graphic event has its own sound: buzz (notification), whoosh (move), chime (reveal), cash register (money), pop (word) | sound makes a silent-first edit land when sound is on; the beat feels tight | one sound per event, on its frame (sound.md); whoosh leads the hit by ~20 ms; max one cue per second; 8 dB+ under the voice |
| T9 | Kinetic type worlds | full-screen type scenes between talking parts: words build a room, a code-typing look, a terminal, a document filling in | resets attention and makes an abstract idea visual | built in code (one beats file drives picture and sound: code-ads.md); a typing look = character by character with a caret, real-looking but generic syntax; 1–3 s per world |

## Caption rules (with any technique)
- Busy background = captions in solid black boxes (white type), so they read on any frame. Clean background = plain type with a shadow.
- Text appears a hair after the spoken word (1–3 frames late), never before it: early text reads as a teleprompter.
- One idea per screen. Clear the screen before the next idea; never stack two thoughts.
- Never over eyes, mouth or a label; inside the platform safe zone (core/export-table.md).

## Picking
- Talking head with no B-roll: T3 + T1 + T8 is the safe base. Add T2 when the line names a message, a sale or a notification.
- One "how did they do that" moment per piece max (T5, T6 or T7), placed at the turn, not the hook.
- Every technique is a supplier ticket when it needs new footage (re-angles, a second pass, a hand plate): ce-realism or ce-cinematic.
