<!-- copied from the Juju repo: runs/harvest/SCORE.md, last changed 03:30 EAT, 25 Nov 2026. Private lines removed. Do not edit here. -->
# How well each tool sees a film

25 Nov 2026. Hand truth against rea-video (fc69e19), our older tools, and snapshots. Every time below is a second of the film. Labels: Measured, Judged, Estimated.

## Verdict

- rea-video is right about **hard cuts on paper**, whole-frame pushes and long standing captions. Trust its shot list there, and nothing inside a code-drawn shot without the extra eyes below.
- Inside code-drawn shots it owned **10 of 35** drawn events (Measured; pure luck gives 3.4). Paper 8 of 12, void 2 of 14, silent map 0 of 9.
- An arrival map plus a frame difference found **35 of 35** on the same windows, at 183 answers for 35 events; luck 11.8 (Measured, same windows it was built on: no held-out proof yet; C uses the arrival map alone, because frame difference on its coded grain adds 28 wrong).
- Snapshots every 2 s show that 32 of 35 happened and place 2 of them within 0.1 s: they are for meaning, never for timing (Estimated, a perfect eye).

## Windows and how the truth was made

| | Film and seconds | Kind | Drawn events | Words | Cuts | Camera moves | Sound landings |
|---|---|---|---|---|---|---|---|
| A | J0wWNytEXS4 169.00 to 209.00 | hero, paper | 12 | 6 | 3 | 1 | 1 |
| B | J0wWNytEXS4 211.00 to 251.00 | hero, void and depth | 14 | 5 (4 scored) | 3 (2 scored) | 3 | 2 |
| C | 3KkQGTa1YjM 432.00 to 472.00 | silent map, 30 fps | 9 | 5 | 0 | 0 | 0 |

- Every frame of every change was looked at; a frame-difference list only said where to look, so it can be kind to frame difference. Point tracks gave the camera curves.
- `runs/harvest/truth/*.json`, hashes and times in `truth/SEALED`. It was sealed before any `breakdown.json` existed for these windows. B was amended after the first seal (each re-seal is written there), still before any answer for it: the star push is layered (211.09, 247.12), and the slide at 228.23 is an object moving, not the camera.
- Before the seal I had read the first lines of no log of these windows; right after it, A's log ("detected 4 shots"). And 0.08 s of clip B is the old shot (B's cut at 211.085 sits two frames in, so it is left out of the cut score).
- A second hand: another worker's hero notes (`runs/scriptlab/hero/part-1.json`), made apart from mine: same events, start times 0.04 s apart (median, A and B). 17 of 26 within 0.1 s one to one; their notes join two of my events in some rows. Measured.
- Sound was read off spectrograms, not heard. Judged: no designed effect sits above voice and music in A and B, none above the beat in C. The three "landings" are music notes near a picture event (189.72, 211.13, 217.66).

## Cuts (within 0.1 s)

| | rea-video | juju-absorb 10 a second | juju-absorb 30 a second | snapshots 2 s |
|---|---|---|---|---|
| A (3) | 3 of 3, 0 wrong, error 0.000 s | 3 of 3, 2 wrong, 0.077 s | 3 of 3, 3 wrong, 0.025 s | 0 of 3 (0.5 s off or more) |
| B (2 countable) | 1 of 2 (247.12), 1 wrong | 1 of 2, 1 wrong | 2 of 2, 1 wrong | 1 of 2, by luck of the grid |
| C (0) | 0 wrong | 1 wrong (441.85) | 1 wrong (441.85) | 0 |

- rea-video's wrong one: the cut at 235.94 (the depth box) is put at 236.15, five frames late, where the zoom smear ends. The 211.085 cut is not found (two frames in).
- Transitions: truth has none. rea-video calls the cuts at 171.13 and 186.65 "blur" over 0.71 s and 0.25 s: they are hard cuts with an element drawing itself in after. Judged wrong, 2 of 2.
- absorb's wrong cuts are big element entrances and leaves inside a shot (map 173.4, number 189.7, 192.9); at 441.85 a caption swap.

## Drawn events inside a shot (start within 0.5 s, box overlap, one answer owns one event)

| | Found | within 0.1 s | said | wrong | start error | act named right |
|---|---|---|---|---|---|---|
| rea-video A | 8 of 12 | 5 | 15 (6 events, 9 stickers) | 5 | 0.07 s | 3 of 8 |
| rea-video B | 2 of 14 | 1 | 2 | 0 | 0.06 s | 1 of 2 |
| rea-video C | 0 of 9 | 0 | 1 (sticker) | 1 | none | 0 |
| **rea-video all** | **10 of 35** | **6** | **18** | **6** | | **4** |
| juju-absorb | 0 of 35 (it makes no such record) | | 0 | | | |
| snapshots 2 s | 32 of 35 noticed | 2 | 32 | 0 | 0.4 to 0.8 s | eye |
| rea-video's own motion code, cut at the true shots | 14 of 35 | 8 | 16 | 0 | 0.04 to 0.8 s | 7 |
| the same, in 4 s pieces | 15 of 35 | 13 | 26 | 0 | 0.02 to 0.07 s | 7 |
| arrival map, merged | 33 of 35 | 23 | 164 | 2 | 0.00 to 0.13 s | not named |
| arrival map + frame difference | 35 of 35 | 25 | 183 | 6 | 0.00 to 0.13 s | not named |

"Wrong" means it touches no truth event and no word. "Said" includes pieces of one event (median 4 pieces an event for the arrival map, 1 for rea-video).

## Words (text alike, then in and out)

| | Found | said | in within 0.1 s | out within 0.1 s | how it enters named right |
|---|---|---|---|---|---|
| A | 5 of 6 (missed "The Republic" 199.57) | 6, one a fragment | 1 of 4 | 2 of 5 | 2 |
| B | 4 of 4 (the two-frame word of the old shot is not counted) | 4 | 1 of 4 | 1 of 2 | 0 of 4: the one that scales in with its land (230.61) is called hard in, two that are cut in are called pop |
| C | 4 of 5 (missed "THE KINGDOM OF HEAVEN" 436.57, read as pieces) | 52 | 0 of 2 | 1 of 2 | 0 |

- C in full: 52 tracks = 9 of the five truths, 19 names printed on the map, 18 pieces of one line, 6 misreadings ("MORTR", "HOROS"). Useful for "what does it say", not for "when".
- The typed number (189.69 to 191.94) is cut in two, typed-on is seen, its start is 1.2 s early in one part and 2.8 s late in the other. "30,000" is read as "30.000".
- juju-absorb (OCR on the middle frame of a shot): right on standing words, no timing; 30 a second: in and out right in A 2 of 5 and 2 of 5, B 3 of 4 and 2 of 2.

## Camera

| | named | measured rate |
|---|---|---|
| A push 177.68 (truth 1.000 to 1.269 in 8.93 s = 0.0301 a second) | 1 of 1, `planar_zoom_pan` | 0.0295 against 0.0301 |
| B star push 211.09 and 230.90 | 0 of 2, says `static` | but its scene numbers say 0.0037 and 0.0033 against 0.0032 and 0.0028: it measured what it called still |
| B push in two layers 247.12 | 0 of 1, says `static` | 0.0041 against 0.0033 |
| our point tracks | 3 of 3 pushes, 247.12 marked "in layers" | 0.0270, 0.0031, 0.0033 (within 11, 4 and 1 percent) |
| juju-absorb | A 1 of 1, plus 1 wrong; B 1 of 3 | 0.0103 against 0.0301 |

## Sound landings

- rea-video A: 0 of 1, 6 said, all wrong. Its effects track held no event at all (0); the 6 are guesses pinned to a "sticker" or a text start (173.4 to 189.1). Run without its splitter on B (3 said) and C (6 said): all wrong. Judged.
- Nothing here can prove it can hear a designed effect: the truth has none. A window with real effects is still to do.

## What it cannot see inside a code-drawn shot

1. **Below 180 px and 12 levels.** It looks at 180 px, 15 times a second, cells of 4 px; an event under 0.2 percent of the frame is thrown away. Lost: the dashed line 171.84 (8 frames), the ruler 189.65, 32 gold dots 213.84 to 215.0, lines 217.26 to 218.59.
2. **Two things at once.** Grid 186.65, star specks 187.10 and blue slab 187.15 came back as one event of 17.71 to 18.38 s. A thing that arrives while another moves is joined to it.
3. **One dead shot.** A 25 s run of four changes with no cut is one shot (211.09 to 235.94). Inside it, the picture moves all the time (the star push), so every change reads as background: 0 of its 8 events (a sticker happens to land on the colour turn at 222.60, which the table counts). Cutting the same code into 4 s pieces gives 5 of 14 for all of B, against 2.
4. **A wrong label switches the eye off.** C was called `ai_video`, so it made no events and no scenes at all. A seeing answer of `code_render` (done here: `truth/rea/C-seen`) gives one scene of 40 s with no event inside. Its motion code called by hand on C gives 5 answers, 3 of 9 right.
5. **Slow or fading change.** Flag fade 436.47 (57 frames), labels, sea colour 460.33, white dot 463.83: each step is under its line. Also a front (land taken 449.10 to 464.37) has no edge it can call an element.

## The five biggest blind spots, and the cheapest way to see each

| # | Blind spot (films and seconds) | Cheapest eye | Measured here | Not done |
|---|---|---|---|---|
| 1 | Small and thin: dots, lines, a ruler (213.84, 217.26, 189.65) | frame difference at 480 px, every frame, threshold 14, 6 px cells | fd alone: A 8 of 12, B 6 of 14, 13 of those 14 inside 0.1 s; 47 s a window at load 180 | none |
| 2 | Fills, fades, fronts, things taken in turn (C 440 to 465; 221.93, 187.15, 198.66) | arrival map: for each point the frame of its lasting colour step, joined by colour and time (`tools/see_at2.py`) | 12 of 12, 12 of 14, 9 of 9 | naming enter, leave, change; merging pieces (3 to 4 an event) |
| 3 | Layers that move apart: stars push, territory stands (211.09, 247.12) | point tracks, then a second fit on what the first left over | three pushes, rates within 1 to 11 percent, one marked "in layers" | which thing belongs to which layer |
| 4 | Elements hidden in a moving picture (208 to 422 of A; 211 to 235) | take the first fit out of each frame, then difference. A dense flow map does the same | not run: `see_at2` skips a moving shot | dense flow |
| 5 | Words on busy maps and typed words (189.69, C) | the typed word is in the frame difference (a growing box); then OCR only on the boxes that change, one reading a word, pieces joined by place and time | frame difference saw 189.69 to 191.94 to the frame | not built |
| + | Shot boundary late by a smear (235.94) | a hard cut is the first frame where most cells are new, not the last of the blur | 1 case, not built | |

Colour layers (k-means, area per colour) alone: 26 of 35, 78 answers, 0 wrong, start 0.08 to 0.20 s, but it names a colour change well and cannot place a thing. Edge tracks alone: 15 of 35 and 234 wrong: text and map edges flicker. A 1 s baseline difference alone: 14 of 35.

## Cost (load 100 to 190; Measured)

| | Wall | Processor |
|---|---|---|
| rea-video A, 40 s, everything, plain | 58.9 min | 1,977 s |
| rea-video B, scripts/harvest, no sound split | 10.0 min | 94 s |
| rea-video C, no sound split, plain | 16.9 min | 410 s |
| juju-absorb, 40 s | 44 s | 16 s |
| frame difference / arrival map, 40 s | 47 s / 100 s | one thread or less, not timed alone |

## Rerun

`scripts/harvest` or `runs/harvest/rea.sh` into `truth/rea/<W>`; `truth/absorb.zsh`; `/usr/local/bin/python3 truth/tools/see.py W`, `see_pt.py W`, `see_at2.py W`; then `python3 truth/tools/score.py` (writes `truth/score.json`). `score.py` prints luck: the same answer shifted in time.

## Open

1. Held out: every eye above was built on these windows. Score it on a window of a third film (a war map, a photo essay) before it goes into `scripts/harvest`.
2. Sound: a window with real designed effects.
3. `survey` (looking) was skipped; it may repair the 235.94 cut and the wrong label of C. Not measured.
