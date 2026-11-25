<!-- copied from the Juju repo: runs/harvest/LANGUAGE.md, last changed 05:11 EAT, 25 Nov 2026. Private lines removed. Do not edit here. -->
# The film language

> Working document. Candidate. The fields are code: `tools/make_schema.py` makes `language.schema.json`, the only list of them, and beside each field who may say it (`x-by`). This page says what they mean.

One film, written so that a stranger can build it and a cheap model can fill it. Frames count from 0 at `t0_s`. Boxes are shares of the frame, x0 y0 x1 y1.
Prose has no place to live. Open strings: the name of a thing (60 signs, what it is and never how it moves), the printed text, the spoken sentence, the spoken word in `cause.ref`. Everything else is a closed word, a number or an id. Evidence is written `film second`; H is J0wWNytEXS4, S is 3KkQGTa1YjM, Z is ZgpMtombn9A.
Donor words, names, drawings, clips, music and whole colour sets stay on this Mac in `language/`; a system takes the numbers and the closed words from here.

## Pick your branch

- **You take a film apart:** `scripts/heavy /usr/local/bin/python3 runs/harvest/tools/measure.py see FILM OUT --from S --to S --words CAPTIONS.json3` (up to 60 s at a time). It writes `measure.json` and a draft `language.json` with only what was measured. You name the things, join pieces of one thing, set `idea`, `cause`, `say`, `relations`. `measure.py valid` must print VALID.
- **You build from it:** read the orders (section 10) and nothing else. `measure.py orders FILE` prints them.
- **You make a recipe or fill one:** section 11.
- **You pace a whole film:** `measure.py pace FILM OUT --words CAPTIONS.json3`, section 9.

## 1. The ten layers of a moment, back to front

| Layer | Holds | Say | Measured by |
|---|---|---|---|
| lens | camera, and which layer rides with it | `move`, per layer `rate_per_f`, `scale`, `dx dy`, `fixed`, `depth` | measure.track (rate error median 5 percent on 3 pushes) |
| ground | paper, void, sea: says what kind of claim is made | one thing, its colour, the shots it stands under | measure.colour not built; eye. Ground change: measure.cut |
| field | stars, grid, room, map under the subject | kind, count, pitch, line width | eye; count only as "about" |
| actors | things with identity: a territory, a network, a solid | one id for its whole life, through every look | arrival map gives place and time; identity by eye |
| marks | lines, arrows, rulers, outlines, flags | from what to what, width, dashed | measure.diff (dots and lines 10 of 11) |
| words | string, role, cap height, how it comes and goes | `role` name number unit clock caption list source title | measure.words (11 of 11 found, 13 of 15 in and out times within 0.1 s) |
| light and material | lit side, shadow, smoke, paint, points | `material`, `side`, scene3d | eye |
| edge and grain | rim, vignette, softness, grain | `edge`, `edge_px` | eye or a pixel patch; hero: edge shade none to 760 px from the centre, 0.55 to 0.70 in the corner, grain 0 (H 530, 639) |
| cut | the first frame of the new picture, flip or not | `f`, `kind`, `flip`, `smear_f` | measure.cut |
| sound | voice, note, hit, silence and what it lands on | `what`, `lands_on`, `lag_ms`, `db` | loudness and captions; never split tonight, so kind and landing are Judged |

Two things of one colour at one place are two things if one can stay when the other leaves. That test settles identity.

## 2. The life of a thing

Six acts and no others: **enter, hold, change, move, leave, return**. Each is one event with `f0` (first frame that differs), `f1` (last), `box`, `way`, `curve`, `cause`.

- **enter, leave:** `way.how`. **change:** `props` with from, to, and `via` when a third colour is passed. **move:** `props` x, y, scale or rotate with from and to. **hold:** only when it does something (a drift, a live clip) or runs over the edge of the window (`before`, `after`). **return:** the same id again; a return under a new meaning also gets a `same_but` tie.
- `cause`: word, pause, beat, note, event, cut or clock, with `ref` and `lead_ms` (minus is picture first). The word is Judged, the time Measured.
- `stays` names what does not go when the event takes something away. It is the argument of every subtraction (H 221.93: the fill goes, the lines stay).
- A part that starts apart is a `lead` (H 187.145: the shadow comes one frame before its slab) or a `part` with its own frames.

### Ways, with what they look like in numbers

| `how` | The eye sees | Numbers found |
|---|---|---|
| pop | whole on one frame | names and units, H 187.896, 189.856 |
| fade | all points together, over many frames | 8 frames and fast first, H 171.838; 57 frames in steps of 2 to 3, S 436.467 |
| wipe | each point at once, points in turn; `circle`, `arc`, `line`, `brush`, and `start` | 24 frames to the far edge, H 173.465; 27 to 29 frames, H 187.145, 198.657; leaving takes 9 to 21, H 206.79, 221.93 |
| draw, grow, shrink | a line gets its length; `start`, `end`, `ends` | ruler 29 frames from its middle both ways, H 189.648; 32 frames as a wave, H 217.258 |
| scale | from a point, with blur, past its size and back | peak at 7 frames and 8 percent over, rest at 14 to 17, H 186.645, 230.605; hero median 105 to 113 percent |
| type | one sign at a time | 2 to 3 frames a sign, H 189.689; 0.12 to 0.25 s a sign, H 359.65, 368.99, 382.88 |
| front | an edge that travels for seconds, pale ahead of the colour | 458 frames, stepped 11.25 times a second, S 449.1 |
| tint | whole thing changes colour where it stands | 22 to 44 frames by way of pale, S 457.233, 459.533 |
| uncover, carried, cut, slide, turn, burst, swap by swell | shown because another leaves; rides with its parent; comes with the shot; moves in; turns like a coin; opens from one point; swells 3 frames and is gone in 4 to 6 | H 206.831; 230.605; 235.944; 228.228; 305.639; 282.41; 243.66 to 244.661 |

`order` is how a group comes: `unit` (item, char, segment, region), `by` (together, one_by_one, wave), `each_f`, `gap_f`, `total_f`, `start`, `end`. 32 dots at one frame each in 29 frames, H 213.838.
`curve.ease`: cut, linear, in, out, in_out, overshoot (`over.f`, `over.pct`, `settle_f`), swell (`swell_f`), step (`step_f` or `step_range`, `step_hz`), spring, unknown. Give `keys` when three points were read. An unknown curve stays unknown.

## 3. Relations

`causes leads follows uncovers replaces same_as same_but stands_for behind tied_to contrasts eye_goes_to`, each between two ids, `lag_f` where timed.
**Reuse:** count pictures, not shots: about 12 pictures carry 45 shots (H 0 to 270, Judged); one outline lives ten lives in 144 s at 0.94 to 0.995 overlap (Measured). Every `same_but` says what differs: ground, place, meaning, dress, count, size.
**Eye:** `shot.eye` is the ordered list of ids looked at. One new thing at a time: median gap between changes 0.44 to 1.3 s in A, B, C (Measured).

## 4. Idea operators: what a change means

Closed: 31, and `idea.move` is closed to the 39 move names. Tagged on all 161 hero rows, none left over (`language/ops_tag.py`, Judged by one reader). `moves` are names of `runs/scriptlab/storyboard/moves.json`; every one of its 39 has a home here.

| Operator | What the change says | Carried by | Hero rows, seconds | Seen at |
|---|---|---|---|---|
| full_to_empty | the picture is withheld so the question stands alone | bare_ground | 7, 29 | H 0, 278.5, 393.3 |
| centre_to_whole | a thing introduces itself from its own centre | grow_from_centre | 2, 8 | H 2.4, 352.2 |
| accepted_to_doubted | what everyone accepts is shown whole, then accused | official_map, come_back | 6, 39 | H 12.4, 263.8 |
| land_to_claim | a claim spreads over what was there | paint_over | 2, 11 | H 6.3; S 449.1 |
| surface_to_bones | a layer is lifted, what held it stays | lift_paint, night_lights | 7, 46 | H 10.2, 117.6, 222.0 |
| rule_to_exception | one step where the rule stops | cross_the_line, test_directions | 4, 20 | H 18.9, 22.9 |
| flat_to_deep | a missing direction is added | tip_to_depth, stand_up | 6, 40 | H 67.6, 186.6, 235.9 |
| deep_to_flat | a direction is thrown away | lined_up | 4, 14 | H 55.0, 97.8 |
| many_to_one | several become one, or fewer | one_left | 3, 15 | H 446.1, 618.7 |
| one_to_many | one thing repeats until the count is felt | draw_back, crowd_of_same | 2, 13 | H 293.2 |
| case_to_habit | many hands, one picture | crowd_of_same | 23, 35 | H 58.2, 335.1 |
| area_to_points | a fill is swapped for what it stood for | count_is_things | 4, 28 | H 211.1, 243.7 |
| points_to_area | separate things drown in one colour | paint_over | 2, 13 | H 102.9, 488.3 |
| whole_to_part | divided, and one part ringed or weighed | share_of_one, point_at | 7, 46 | H 368.8, 382.9 |
| part_to_whole | pieces join into a system | named_in_turn, lined_up | 7, 32 | H 465.8, 543.9 |
| outside_to_inside | go in, find parts in the part | sink_in, level_below | 8, 69 | H 83.7, 646.9 |
| inside_to_outside | step back, the subject is one of many | draw_back | 1, 5 | H 388.3 |
| near_to_far | the gap to the next thing, true size | true_gap | 2, 12 | H 77.4 |
| then_to_now | two dates of one thing, or a clock | then_now, how_far_by_day | 3, 11 | 7prMGQnO8n4 4 to 24; H thin |
| name_to_number | a word becomes a figure | number_alone, number_on_table | 3, 13 | H 189.6, 359.6; Z 60 |
| number_to_thing | a figure becomes things, or true size | draw_it_true, count_is_things | 2, 13 | H 283.7 |
| name_to_thing | each item shown as it is said | list_answered, named_in_turn | 4, 16 | H 124.9 |
| picture_to_opposite | same picture, other ground or meaning | ground_flip, come_back | 4, 33 | H 112.0, 247.1; Z 136, 1086 |
| this_beside_that | two states in one frame | side_by_side, then_now, night_lights | 3, 13 | H 280.2, 314.3 |
| places_to_ties | what holds it is the ways between | ties | 3, 15 | H 133.1, 458.9 |
| line_to_reason | an edge followed, or laid on what made it | trace_the_edge, lies_on_nature | 2, 14 | H 165.8, 177.7 |
| drawing_to_real | the diagram gives way to a real place, page, clip | open_to_real, exhibit, page_lit, words_on_painting | 28, 112 | H 129.2, 695.7 |
| fits_to_overflows | past the frame, or too much to read | wider_than_frame | 6, 49 | H 408.0, 567.7 |
| cause_to_effect | one is moved, what is tied follows | paint_over, ties, how_far_by_day | 2, 20 | H 579.9; S 449.1 to 464.4 |
| said_to_struck | one or two words alone, answered or struck | word_alone | 2, 8 | H 396.6, 642.4 |
| all_to_one_left | everything else goes | one_left | 2, 11 | H 206.8, 437.7 |

`idea.from` and `idea.to` are ids on screen. A shot whose operator has no from and no to is decoration: write `idea: null` and let a reviewer see it.

## 5. Cut and ground

A cut is the first frame where the old picture is gone, not the last frame of a smear (H 235.944; rea-video put it 5 frames late). A picture that changes inside a fixed frame on paper is a cut of that clip, not of the shot (H 667.79).
`flip` is a cut that also changes the ground: 12 in 270 s (H 263.8 to 492.2, Measured), one frame, never softened, on the turn of an idea. A ground has one job for the whole film.
Run against hold: 12 pictures at exactly 15 frames each, then 3.5 s (H 335.1 to 342.6).

## 6. Density and rest

Density is starts of events and words in 10 s: 5.0 A, 5.2 B, 3.0 C (Measured on hand truth). Rest is a stretch with nothing new but a drift: longest 8.97 s A, 7.72 B, 8.13 C; hero 16.7 s once (H 247.1).
`shot.rest`: none, part (a drift runs), full. Rest is earned by the event before it. Held pictures drift linearly, 0.3 to 2.9 percent a second (H 67.6, 177.7), with no ease at either end, or are locked at scale 1.0000.

## 7. Depth and 3D

- **Layered** (two rates, no 3D): the far layer and the near layer each get a row in `lens.layers`. Stars 0.0031 a second under still things (H 211.085); stars 0.0031 against the shapes' 0.0088 (H 247.121, Measured by measure.track). The same star push runs behind a still room at H 235.944 to 247.1: neither the truth nor the hero notes hold it; two frames laid together show it (Judged).
- **Solid**: `scene3d` with camera keys (eye, at, frame), projection, lights (kind, direction, power, shadow), materials (base, side, roughness, thickness). Side walls at 1 to 16 percent of the light of the top, no gradient between (H 331.0).
- Camera keys of a 3D shot are Judged until a rebuild overlays (`compare`); no tool here solves a camera.

## 8. Sound

`kind` music, voice, effect, room, silence; `what` is closed; `lands_on` names the event or cut. Not split and not heard tonight, so every row is Judged and says so in `limits`.
Known of the hero: no designed effect found at 117 cuts (runs/atlas/grammar, Measured by level, not heard); notes near picture events at H 189.72, 211.13, 217.66 (Judged from spectrograms); bed about 15 dB under the voice.

## 9. Pacing of the whole film

`pacing` holds `movements` (t0, t1, job, ground, heat 0 to 5; `skeleton` and `beat` point into `runs/scriptlab/skeletons`), `turns` (t, operator, pause before, flip), `questions` (opens, closes, by word or picture), `words_a_minute`, `silences`, `loudness`, `cuts_a_minute`, `events_a_10s`, `rests`.

Hero, 780 s (Measured by measure.pace, words from captions):

| Minute | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| cuts | 13 | 13 | 6 | 3 | 7 | 23 | 10 | 13 | 4 | 7 | 15 | 15 | 4 |
| words | 179 | 173 | 176 | 167 | 164 | 173 | 166 | 174 | 193 | 181 | 176 | 187 | 137 |
| quiet gaps of 0.5 s or more | 10 | 19 | 15 | 3 | 17 | 12 | 7 | 15 | 16 | 14 | 15 | 15 | 15 |
| loudness dB, mean | -23.3 | -23.6 | -24.6 | -23.3 | -23.6 | -23.8 | -24.5 | -23.7 | -24.2 | -24.1 | -24.4 | -25.0 | -27.4 |

The words run flat (164 to 193), the cuts do not (3 to 23): pace is in the picture. Minute 3 is one long build with 3 cuts, minute 5 is a crowd with 23. Gaps: median 0.6 s, 100 s in all; only three over 1.1 s (102.1, 766.6, 769.2 to the end).
A silent film has no words row: its pace is `events_a_10s`, its turns the date and the caption (S: 1 cut in 541 s, Measured; 3.0 changes in 10 s in 432 to 472).

Lead and air: the picture stands before its spoken word: median 278 ms over 87 pairs (H 0 to 270), 203 ms over 67 (H 520 to 770); after a heard pause 33 of 35 changes come before the voice, median 295 ms; a pictured noun is said a median of 1.8 to 2.2 s after its picture is up (Measured times, Judged pairs). A typed number begins 30 ms after its word and ends with it (H 189.72).
Before a turn: 0.96 to 0.99 s of quiet (H 618.8, 632.5), 2.36 s before the last words (H 769.0); bare ground 1.71 to 3.2 s (H 278.5, 393.3).

## 10. The prompt form: orders

One order a line, the same data as the JSON, both ways without loss (`measure.py orders`, `orders --back`; `fit` proves it on 64 truth rows).

```
FILM film="..." t0_s=211.002 fps=23.976 frames=960 size=[1920,1080] limits=["sound_not_split"]
THING id=ties layer=actors kind=lines name="lines between the places" colours=["gold"] label=Judged
SHOT id=s2 f0=2 f1=597 cut=c1 ground=void lens=["l1"] things=["fill","ties"] say="..." idea.op=surface_to_bones idea.from=fill idea.to=ties idea.move=lift_paint
CUT id=c1 f=2 kind=hard flip=true label=Measured by=["measure.cut"]
LENS id=l1 f0=2 f1=412 move=push layers=[{"who":["stars"],"rate_per_f":0.000134,"ease":"linear"}] fixed=["fill","ties"] depth=true
ENTER id=e1 thing=ties f0=150 f1=182 box=[0.3,0.2,0.7,0.9] way.how=grow way.shape=path order.unit=item order.by=wave order.start=first order.end=all_sides cause.kind=word cause.ref="joined" cause.lead_ms=-230
LEAVE id=e2 thing=fill f0=262 f1=283 box=[0.3,0.2,0.7,0.95] way.how=wipe way.shape=arc way.start=left way.end=right stays=["ties"]
SOUND id=n1 f=159.7 kind=music what=high_tone lands_on=e1
TIE a=e2 rel=uncovers b=ties
```

(An example: frames and rates are H 211 to 251, the word, its lead and the names are made up. A real one: `language/truth-B.orders.txt`, 62 lines for 40 s.)

Every order answers five things: **what** (`thing`), **where** (`box`, layer, z), **when** (`f0 f1`), **how** (`way`, `order`, `curve`, `blur`, `stays`), **why then** (`cause`, `idea`). A builder who lacks one of the five asks the pack, never the film.
`cause` left out means unknown, `null` means looked for and not found. A key that is absent is the engine's default.

## 11. For a cheap model: what it fills, what it never touches

A recipe is a stretch of orders with three kinds of value.

| Kind | Fields | Who sets it |
|---|---|---|
| law | `way`, `order`, `curve`, `blur`, rates, leads, rests, `stays`, ties | the recipe; from the numbers above, with a trace `film second, kept or bent` |
| slot | `name`, `text.string`, `count`, the subject's data id, `colours` as a role, `cause.ref` (which spoken word) | the cheap model, from a closed menu of ids code made, or words that stand in the script |
| code | `f0 f1` (from the word clock and `lead_ms`), `box` (from the slot's shape), `size`, ids | code |

Steps for one stretch, each a small call: 1. choose `idea.op` from the operators the skeleton beat allows; 2. choose a `move` the engine can draw today (`drawable_today` in moves.json); 3. choose the data id for each slot; 4. choose the word the change lands on. Code writes the frames, runs `measure.py valid`, and drops the row it refuses.

## 12. Which tool for which field

| Field | Tool | Right on hand truth | When to look yourself |
|---|---|---|---|
| cut `f` | measure.cut | 5 of 5 in A and B, none invented in C; hero whole: 108 of 113 noted, 133 said, 8 of them wrong by looking (`language/cut-look.json`, Judged) | a cut inside a clip box, a soft cut |
| event `f0 f1 box` | measure.arrive, measure.diff | 32 of 35, 25 within 0.1 s, 134 said, 4 wrong; held out 36 of 36 and 30 within 0.1 s, 271 said | two things that touch while both move (H 243.7 to 244.7) |
| `act` | colour against the ground | 17 of 32 | always for change against move |
| `way` `shape` `start` `ease` | order of the pixels' own steps | way 10 of 32, start 4 of 8 (`language/ways.py`): a first guess, no more | always; a fit over 0.9 did come in turn 7 of 8 times |
| layers, rates | measure.track | 3 of 3 pushes said in layers, the one-layer push not | fewer than 60 points |
| words | measure.words (Apple Vision, then ink by frame) | 11 of 11, 5 misread pieces | type under 2 percent of the height, posters |
| identity, parts, z, material, idea, ties, `eye`, movements, turns, questions, scene3d | eye | | always |
| density, rests | measure.see (`pacing.events_a_10s`, `rests`) | counts pieces, so it reads high | join pieces first |
| ground, `flip`, sound | not built | | eye; sound from level and spectrogram, not heard, not split |
| cause word | captions, nearest word | time Measured, word Judged | always |
| loudness, words and cuts a minute, silence | measure.pace | | captions stretch words over pauses |
| rea-video | hard cuts, whole frame pushes, standing captions, the storyboard | SCORE.md | nothing else inside code-drawn shots |

## 13. Proof and how far it goes

`scripts/heavy /usr/local/bin/python3 runs/harvest/tools/measure.py check`

25 Nov 2026, 05:15. Measured unless said.

| Proof | Result |
|---|---|
| every row of the sealed truth said in the schema, prose taken apart phrase by phrase | 64 of 64 rows, 300 phrases, 0 words left over; every number and direction in a phrase is checked against its field; orders and back the same |
| planted faults (free prose, a lost clause, a how hidden in a name, a changed number, a turned direction, a moved frame ...) | 18 of 18 refused, each for its own reason |
| phrases that rest on a thing's name alone | 29 of 300, all from what it is, none from how it moves |
| the whole hero's pacing in the schema, through orders and back | valid, the same |
| 1 small and thin | 10 of 11, 8 within 0.1 s (luck 2.2); best rea-video answer 5, 3 |
| 2 fills, fades, fronts | 13 of 13, 10 (luck 3.0); rea 5, 3 |
| 3 layers that move apart | 3 of 3 said in layers, rate error 5 percent; rea 0 of 3, 36 percent |
| 4 hidden in a moving picture | 6 of 7, 4 (luck 1.6); rea 5, 4: **not won** (exact starts are equal) |
| 5 words | 11 of 11, 13 times within 0.1 s, 5 misread of 25 said; rea 9, 4, 12 of 58 |
| share of wrong answers | 0.03 against 0.10 to 0.33 |

Best rea-video answer = the better of run alone, run and reviewed by a fresh seeing agent, each with and without its scene borders, taken window by window; `spots.json` was written before measure.py. Same windows the eyes were tuned on.
Held out, notes made apart by other workers (`language/heldout.py`), found net of luck (the same answer shifted in time):

| | noted | said | within 0.5 s | net of luck | within 0.1 s | net of luck |
|---|---|---|---|---|---|---|
| H 280 to 320, measure.py | 19 | 126 | 19 | 7.6 | 17 | 11.8 |
| rea's motion code, shots given | 19 | 11 | 6 | 4.2 | 5 | 3.8 |
| H 632 to 672, measure.py | 17 | 145 | 17 | 5.4 | 13 | 7.8 |
| rea's motion code, shots given | 17 | 20 | 12 | **10.4** | 6 | 6.0 |

So measure.py misses nothing and places starts better; it also says seven to nine pieces for a thing, and at half a second rea's few answers on big plain graphics are the better guess (H 642 to 654). You join the pieces.

Not won, not done: spot 4; every held-out second is of one film. One reader tagged the ideas; curve and way names are not scored; footage inside a frame is one live thing; no sound was heard; no blind rebuild from these orders has been drawn.
