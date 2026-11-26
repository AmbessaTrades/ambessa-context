<!-- copied from the Juju repo: docs/ENGINE-2.md, last changed 19:24 EAT, 26 Nov 2026. Private lines removed. Do not edit here. -->
# Engine 2: worlds, not text layouts

> **Retired for map films 25 Nov 2026 (ADR 0022):** the Map theatre row is now Juju Maps (`docs/STACK-MOVE.md`). The other worlds wait with their niches.

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.
> Candidate design, 24 Nov 2026. "Measured" was run on this Mac today. "Candidate" is a guess to be tested. `lot-r01` is retired (ADR 0004): the next test uses new material.

## Why the films scored 3 to 5, worst damage first

| # | Cause | Evidence |
|---|---|---|
| 1 | **The spoken words were the picture, and the form let the rest of the frame stay empty.** Seven of nine stages are words or a small object on a plain ground; every stage prints the speech, word by word. Pictures were optional in four stages. | Measured: share of seconds with under 35% of the frame drawn: fills 64, 64, 72%. Same engine and same pictures with a strong hand's form: 31%. Three real painting and archive films (016, 018): 8%. Real clips of 30 films: 18 at 0%; only black space, dark drawn and chat films go past 11%. |
| 2 | **No stage is a place.** Nothing is held, deep or lit; a scene starts bare and builds; frames 5 s apart show half words ("Day thre"). Every scene is the same brown or red ground, so the whole film looks like one screen. | Picture filling the frame: 10, 10, 17% of the time (strong form 31%), from the scene lists. In 007 to 015 the cockpit, map or street is there from the first frame and one number, border or light moves in it. |
| 3 | **Too few pictures, no spares.** Five stills and two clips for 85 s: 4.9 a minute. The bowl came back in every fill. | Counted by eye in 13 short clips of two painting films (65 s): 16 plate changes, about 15 a minute. |
| 4 | **The judged films were silent** (`"audio": null` in all three), so the printed words had to be the narrator. | `render.json`. How much of the score this cost is unknown: the judges' notes are not on disk. |
| 5 | **The picture did not say what the voice said.** A clock under "No medals at the end", a feast under "Your belly gets a drink". Red highlighter was the event of choice. | `mark` is 11 of 18, 7 of 20 and 8 of 23 events. The strong form used 19 kinds of event; 8 of its 37 were `mark`. |
| 6 | **Empty slots drawn as empty boxes** for about 10 s, because a panel exists before its words are said. | Fill 1 at 1:10 and 1:15, fill 2 at 0:55 and 1:00; even the strong form at 1:00. |
| 7 | **The gates reward the wrong thing.** Handwriting counts as movement; a left to right flip counts as variety; a film that fails is still shown. | Measured: the fills move in 66 to 73 of 85 s; the two real painting films in 29 of 65 s. Fill 2 passed all three gates. Fills 1 and 3 failed and were judged anyway. |
| 8 | **Heal's floor is a text film** (OPEN-RISKS, weak model 1). In this run it did less than we thought: 3 added `mark`s, 1 flip, 1 split, no fallback scene. | `heal.json`. The text came from the model's own choices. |
| 9 | **The longer script.** It dropped 11, 10 and 11 scenes and ate 64 of 66 re-asks. It did not change what is seen in the 85 s. | Outside the missing words the three models made 0, 1 and 1 form errors. Filling the form is not the hard part; choosing is. |

The order is my reading. One test separates the causes: strong and weak filler, thin and full supply, with voice, on new material (four 60 s cuts).

## The stages become worlds

A world is a place that is whole in its first frame, stays 20 to 200 s, and has a **state table** (place, number, date or light against the clock). Code moves between rows, so something always advances. Speech is never drawn by default: it is heard, with at most a caption lane. Each world is one Rust type behind one trait; nothing in it names a channel; every look comes from the pack.

| World (seen in) | Slots | What moves | Needs a picture |
|---|---|---|---|
| **Map theatre** (009, 011, 012, 013, 015) | base map and date range, sides, border rows by date, units, places, counter | borders flow, units travel, date ticks, camera goes where it happens, counter runs | Base: no, real map data. 1 real photo, flag or portrait per named event or leader |
| **Route chart** (009, 010, 015) | bodies or stops with true positions, craft, start, end, date, arrival count | bodies orbit, trail draws, scale zooms out, arrival count falls | Chart: no. 1 real surface map or craft model per body visited |
| **Instrument view** (007, 008, 014, 015) | window (cockpit, street, room), outside scene, 2 to 5 gauges fed from one number table, milestones | outside view never stops, gauges count, light and colour shift, next milestone counts down | No. Needs a built 3D scene: the dearest to make, the cheapest to run |
| **Timeline or lineage tree** (band in 013; the brief's UsefulCharts, not looked at here) | nodes (name, date, parent), path, bands, places | camera travels the branch, new branches grow, bands slide, ancestors stay lit | 1 real face or object per 2 named nodes, or it is a chart of words |
| **Layered painting** (016, 018) | picture, focus, light side, weather, caption | 3 to 5 cut layers slide apart, light crosses, mist or dust, dissolve into the next | Always. The hungriest world |
| **Document and quote canvas** (016, 018) | scan of the real page, exact line on it, author, source line | page rises from dark, the spoken line lights on the page itself, page turns, author's face | Always: the real page and the author. No page found, no quote scene |
| **Archive footage** (016, 018) | clips, place and date stamp, credit | real motion, cut on the words; a still is held 6 s at most (candidate) | Always, a real file with a licence |
| **Group chat** (015) | cast (name, face), room, messages, time jumps, pinned pictures | typing dots, bubbles, scroll, people join and leave | 1 face per speaker. Only for a chat channel whose cast want things and fight |
| **Ladder or scale flight** (012, 013, 014) | quantity, unit, rungs (value, plain comparison), camera path | camera passes each rung, number climbs, surroundings change, "next in 25 s" counts | 1 real photo per 4 rungs (012 shows Valdivia 1960) |

To retire (candidate): `rule_card`, `quote_canvas` on bare ground, `panels`, `dial`, `object_table` and `curve` as full scenes. Their motions (ink, sweep, grow, light) live on as parts inside a world. `chapter_title` is a beat inside the world on screen.
Build order (candidate): layered painting and document canvas, then map theatre, then timeline. One film needs two or three worlds, not nine.
A world ships only when a strong hand's 60 s of it, with voice, beats the old engine and stands beside the real clips to fresh eyes.

## Picture supply law (candidate numbers)

1. A film may not start until every picture slot in its plan is filled, plus 20% spare. Empty slot: the film waits. Nothing is drawn as a box.
2. Ready pictures for each minute of that world on screen: painting 12, archive 10, document 4 (pages and faces), chat 1 face per speaker, ladder 2, timeline 4, map 3, route 1, instrument 0. Pull at least 3 real candidates for each one kept (so 36 a minute for painting).
3. "Ready" means: real file on the Mac, source and licence written, wide enough after its crop (1920 px full frame), a one line "what it shows" written from looking at it, and a fit of 2 or 3 on the 0 to 3 scale against the very words it sits under. A fit of 0 or 1 is empty.
4. A picture may come back once, in a new crop, at least 90 s later. Code refuses the third use.
5. What this costs: 50 minutes that is half painting (25) and half map (25) needs 375 kept and about 1,125 pulled. How long that takes is not measured. Held worlds are what make 50 minutes affordable; a pack's mix of worlds is its picture bill.

## Text law (candidate numbers)

| Measure (row 1 fills: scene lists; row 2: pixels) | Fills | Real painting films | Candidate limit |
|---|---|---|---|
| Type on a plain ground | 37, 12, 16% | about 10%, runs seen of 2 to 2.5 s | 6% of the film (stricter than theirs on purpose), 4 s a run, 20 s apart |
| Seconds with under 35% of the frame drawn | 64, 64, 72% | 8% | 10%; space worlds and chat have their own meter |
| `mark` (highlighter) events | 61, 35, 35% | not measured | 15% of events (strong form: 22%) |
| Speech printed word by word | 100% | 0: whole short lines that fade | 0%. Captions only if the pack says so: 2 lines, one lane, whole lines, never half a word |

A chat pack is exempt from the first row only if its cast is in conflict and it has sound. Silent type over archive: OPEN-RISKS (YouTube 5) proposes a ban; keep it.
New gates: the world is drawn within 0.5 s of a cut; the state table really advances on screen; one opening never repeats within 10 minutes.
**Calibrate first:** any gate that ranks these three fills above the real clips is thrown out. A failed film is never shown as a result.

## What a pack must say, so two channels in one niche look different

1. **Its stance:** what it believes, its source shelf, what it refuses to say (ADR 0002). Two channels with the same stance are one channel.
2. **Home world and shares:** one home world for at least half the film, one or two others, in minutes.
3. **Home object:** the exact cockpit, map projection and base, tree shape, or chat room. Built for this pack, not recoloured.
4. **Its furniture:** which number or date is always on screen, where, in what type, and what sits in the caption lane (or nothing).
5. **Its pictures:** which archives, century and kind (oil, engraving, press photo, satellite), and how they are cut and lit.
6. **Its cut:** seconds a plate stays, dissolve or hard cut or burn, when the camera may move. **Its sound:** one mode, for life.
7. **The neighbour list:** the two nearest channels and three things each does that this one will not.

Test (candidate): 12 frames from each of two packs, words and names masked; a fresh judge sorts at least 22 of 24. Turning the hue does not count as a difference (OPEN-RISKS, YouTube 2). Difference is owned openly, never used to hide that channels are related.

## What the cheap model must never decide

Which world, or how long it stays · whether a slot gets a picture · whether a picture fits · any fact, number, date, place or quote (it picks a row from the claim ledger) · time, size, colour, position, camera or layout · whether words go on screen · what replaces a failed answer · whether a film starts, passes or ships · the idea, the turn, or anything in the pack.

**It may:** match each stretch of script to a row of a plan already made; choose between two or three pictures already judged fit; name which change in the state table happens on which words. The aim: every choice is between good answers, so the worst film it can make is still a real film. Unproven.
The plan (about 25 to 40 scenes for 50 minutes) is made once per film by the strongest model the router allows, or by code. Who pays is open.
Heal may fix spelling and spans. It may not add a scene, an event or a layout. A scene that fails twice goes up one model with its script around it; if that fails the film stops and says which line. Limit on fallback scenes: 0.

## Not known

- The judges' notes, the effect of sound, and whether the strong-hand form itself would score above 5: none is on disk. No world here is built or timed.
- The old engine drew these at about 0.6 to 1.0 times real time (load 18), so 50 minutes is about 1 to 1.5 hours; layered worlds will be slower.
- The real clips are 5 or 6 s each and small; 007 to 018 are frames, not films. The frame meter: 1 frame a second at 320x180 grey, 16x9 blocks, a block counts as drawn when its spread passes 6; the 35% line is mine.
