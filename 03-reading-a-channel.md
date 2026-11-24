# 03 — Reading a channel or a film

Updated 24 November 2026. Two layers: the older nine measurements, and today's fuller teardown.

## The nine measurements (19 Nov, still in force)

Sample frames at 2, 18, 35, 52, 68, 84 and 95% plus the transcript: plate dwell · cuts a minute · caption rate · caption length · text presence
· chapter cadence · words a minute · plate classes · colour drift. Two channels share a format only when all nine are within tolerance.

## The full teardown (24 Nov)

Ambi named five films and asked for "every aspect": thumbnails, exact times, text, and the 90/70/50 follow-up pattern. Each film is cut into
shots, then measured: holds, zooms and pans, palette per scene, words on screen by OCR, voice timing, sound by Earshot, quote structures,
thumbnails, and the channel's hits and what followed them.

| Film | Channel | Views on 24 Nov | Length |
|---|---|---|---|
| AI's Strange Obsession with Enlightenment | hands | 1,253,761 | 24:30 |
| Would You Board a Ship to Another Star? | Orange Scarf | 782,501 | 19:32 |
| Something Is Strange About Where We Live in the Milky Way | Milky Stellar | 330,470 | 38:01 |
| The Ancient Test of a True Friend | The Ancient Logos | 159,863 | 11:21 |
| The Grand Canyon Wasn't There in 1540?? | Ink Of The Past | 51,018 | 9:10 |

Findings so far: [11-juju/teardowns.md](11-juju/teardowns.md). Pictures: library section "Teardowns". The job is running.

What Ambi wants taken from them, in his words: "the way he does quotes is just so awesome"; half of the AI film's images are stills that show
the drawing process in sixteen frames, moved only with "some squiggles and wiggles and a slight zoom"; type, palettes and theming, "how they map up
with each other, and how we extract that off of a video".

## The absorber

`crates/juju-absorb` does this in code. Speech decides the sound mode once, for life. Code measures; a model only labels each shot from a closed
list; a shot no type fits becomes a request for a new stage type. A profile must predict three unseen films of the channel before it is used.
Ambi's two spiritual-look rules: exactly four of the 24 ready-made looks are spiritual, and an absorbed spiritual film leans toward one of the four.

## Corrections to older numbers (Measured 24 Nov)

@Ethos-j7t's median is **12,000** views (best 185,000), not the 2.0M the brief states. Server History's median is 291,500 (best 3.1M). Jacopist's is
248,500 (best 2.0M); the 19 Nov scan said 424,000 on a different sample. A ratio is only as good as its median.
