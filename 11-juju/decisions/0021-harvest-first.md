# ADR 0021: harvest first, then cheap models execute

Decided 24 Nov 2026, about 23:55 (Ambi): "use Opus 5.5 high ultracode or Fable 5.2 high ultracode to do the reverse engineering of 9 to 12 key videos, extract their systems ... a bunch of layers of different systems, visually verified, that we can map prompts to, then build design systems around them, colour palette, structures, 3D ... then give it to the lesser models so they don't have to think that much, they just execute, mixing and matching ... even if a YouTube video is put into our app and the brand profile has to make that for that channel, it uses an amalgamation of design systems similar to that, or reverse engineers that video ... so DeepSeek does it without Anthropic ... the rest of the night just focus on this, this is the gold." And: "you're stuck on 10 second, 20 second clips. You're not making a full 20 minute, a full 15 minute video. You don't understand pacing, you don't have the script skeletons."

1. Strong models once, offline: 12 key films taken apart whole (picture, motion, words, pacing, sound, packaging) into packs of data. Proven by a blind rebuild: a builder who never saw the film rebuilds a stretch from the pack alone.
2. Layers, each checked by looking: pack (one film) -> grammar (rules with counts) -> system (tokens, materials, operators, timing laws) -> recipe (a 20 to 60 s movement with slots that compiles to an engine form) -> film plan (a 10, 20, 30 or 50 minute order of recipes with its script skeleton, pacing curve and sound).
3. A recipe ships only when it was drawn on three unrelated subjects and eyes calibrated on AMBI-EYE.md passed all three.
4. Cheap models execute: they choose from closed menus and fill slots. Target: 95 percent legal at the first answer with DeepSeek Flash, and no strong model in a film.
5. A pasted link: Juju measures the film, finds the nearest systems and blends them by named traits, or harvests it into a new pack with its own models. A blend says what it took from where.
6. The unit of proof is a whole film of 10 minutes or more with a voice, never a clip.

Models: the harvest lane may use Opus 5.5 or Fable 5.2 at high (Ambi named both); everything else stays at medium or below.

## Added 25 Nov 01:00 (Ambi): "f*** safety aggressively rea video. make it a high quality skill juju, true to exactly how its done, and add a few things designed for us and our workflows that make it faster and reliable"

7. No audit step and no sandbox work for rea-video. What stays, because it costs nothing: its process starts with an empty environment, so no key is in it. The money gate, the cap and the rights rules are unchanged.
8. One command, `scripts/harvest`, upstream order exactly; speed only where the answers stay the same (decode once in hardware, Apple Vision text, CoreML sound splitting in windows, captions as speech, receipts, resume, two films at once).
9. One skill, `film-harvest` (crates/juju-skills/packs), faithful to upstream's skill and references, with ours marked as ours.
