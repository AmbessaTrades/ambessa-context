# The film engine: stage experiment 1 and engine round 2

As of 13:10 EAT, 24 Nov 2026. Source: workflow runs a workflow (reference study, engine build, three cheap-model fills, judges) and a workflow (round 2: diagnosis and picture supply).

> **Read with this:** the nine worlds and the picture-supply law are in `engine-worlds.md`. Worlds have been drawn since (gallery, "Juju — engine", rounds 1 to 6). No judge has scored them yet.

## In short

- **Tried.** Cheap models filled the stage form for one script of 198 words, about 84 s at 142 words a minute. Three fills were checked, healed, rendered and judged. Each film came out 85 s long.
- **Worked.** The engine's check, heal and render ran on all three fills. Fill 2 passed all three gates. The hand-directed proof rendered from JSON alone, at 85.17 s, and passed its gates.
- **Failed.** The fills kept the house look but lost the pictures. Nine judgments gave 3 to 5 out of 10, mean about 4.1. Critics found empty picture frames, long stretches of text on bare brown, one bowl image reused, and no audio track.
- **Round 2 diagnosis.** The spoken words were the picture. The form allowed empty frames. The supply was too thin (4.9 pictures a minute in test). The gates rewarded movement, not quality.
- **Open.** The nine worlds and the picture-supply rule are named in ENGINE-2.md, which is not in this input. Several engine faults are unfixed, and speed and memory are over the brief's limits.

## What was done

**Reference study.** Two reference films were read as stills: 007 (25:06) and 008 (16:16), both with one cockpit world held for 6 of 8 sampled frames. Two orrery films, 009 (26:10) and 010 (24:25), returned to one diagram world with a date that only rises. The study turned these into laws: a held world, one monotonic clock, a fixed stamp corner, one caption slot, and no face before the end.

**Engine build.** A new crate, `crates/juju-stage`, was added to the workspace. About 1,300 lines in 11 files, with 28 tests passing (7 unit, 21 law tests written before the code). It has five commands: `check` (validates the form and reports laws), `heal` (fills gaps without a model), `render` (1920x1080, 24 fps, h264), `gates` (progression, variety and safe-box tests), and `schema` (generates the JSON Schema, so it is never hand-written). It has nine stage types: object table, dial, curve, road, rule card, panels, chapter title, footage and quote canvas. Words are laid out by code from a word clock.

**Proof.** The 85 s hand-directed proof was re-rendered from JSON only, with the original voice muxed in. The maker reports it as "as good, not better" than the hand version. Differences: every spoken word is captioned by code, and cuts are hard.

**Stage experiment 1.** Three cheap-model fills (fill 1, 2, 3) were written against the same script. Each was checked, re-asked, healed, rendered and gated. Judges then scored the films.

**Round 2.** A diagnosis (ENGINE-2.md) was written from the measured clips. A picture crate, `crates/juju-reliquary`, was built to gather public-domain or open-licence pictures. Its 26 tests pass against saved archive answers.

## Breakthroughs

- **The proof renders from JSON alone.** The 85.17 s film (1920x1080, 32 MB) came from the form, with the voice muxed in. Its gates passed: longest stretch with no local change 1.5 s (limit 7). Evidence: render output and gates.json. The maker reports the look matches the hand version. One judge's text cites the proof as 7 of 10. That citation is the only score for the proof.
- **The gates catch deliberate faults.** Controls were made to fail on purpose. A zoom over one still failed progression (19.75 s with no local change). Cream bars at the edge failed the safe box. A 50 s loop failed variety (0% new). Evidence: the maker's control runs.
- **112 licensed pictures on disk, all large enough.** Every picture is 1600 px or more on the long side. The licence gate accepts only public domain, CC0 or CC BY. `juju-reliquary check` reports 0 bad files. Evidence: counts in the Numbers table.
- **The diagnosis shows a measurable gap.** Real painting films leave at most 8% of seconds with under 35% of the frame drawn. The fills leave 64 to 72%. Evidence: the maker's frame meter (its script is not in the repo).

## What critics found

1. **Empty picture frames drawn on screen.** Fill 1 at 1:08 to 1:20. Fill 2 at 0:54 to 0:59, extracted frame at 57.5 s. Fill 3 at 54 to 64 s. How shown: judges read contact sheets and frame extracts. Fixed? Open. The proposed fix is to refuse empty slots.
2. **Text alone on bare brown.** Fill 1 about 23 s (0:10 to 0:19 and 0:50 to 1:04). Fill 3 11.8 s (0:34 to 0:45). How shown: scene lists and judges. Fixed? Open.
3. **Pictures reused.** Fill 1 bowl in about 9 of 18 tiles. Fill 3 bowl in 4 scenes. Fill 2 the opening object is also the closing stage, 32% of the film. Fixed? Open.
4. **Safe-box failure shipped.** Fill 1 render.json: safe_box pass false, 185,260 glyph pixels in the outer 5% margin. The gate also showed ink in the margin for 3 s at 72 s (339 px). Fixed? Open. Fill 2's gate reported 0 stray marks.
5. **No audio.** Render.json reads `audio: null` while also saying `sound: narrated`. The mp4s have a video stream only. Judges could not judge timing. Fixed? Open.
6. **Gates reward handwriting.** Fill 2 passed all three gates and judges gave it 4 and 5. Fills 1 and 3 failed gates and were judged anyway. The movement meter gave fills 66 to 73 of 85 s moving, against 29 of 65 s for real films. Fixed? Open. The diagnosis calls this its point 7.
7. **Heal and variety gate disagree.** On fill 3, heal reports valid, yet the variety gate measured 0.0 new seconds (need 0.3). A likely cause is that heal dropped 11 of 21 scenes, so the tail reuses earlier material. Fixed? Open.
8. **Empty answer can never pass.** A blank start-word answer is rejected even when the check lists it as the only allowed value, so re-asks cannot succeed. Reported as a possible engine bug by the fill 1 run. Fixed? Unknown.
9. **Form written for a longer script.** Fill 1 scenes 7 to 17 quote words not in this 198-word script. Fill 2 scenes 8 to 17 do the same. The fill agent calls this an input pairing error. Fixed? Open. The diagnosis lists "the longer script" as a cause.
10. **Words do not match pictures.** A clock stands for "clock hits lunch", a bowl for "drink water". Judges said the pictures decorate but do not show the idea. Fixed? Open.
11. **Type cut mid-glyph.** Frames show "Day thre", "HOUR 1" clipped, and labels "HOU", "HC". Fixed? Open.
12. **Dial reused with no change.** Fill 3 uses one dial 4 times in 85 s, with the hand at the same angle. Fixed? Open.
13. **Speed and memory over limits.** The proof peaks at 637 MB, against 580 MB per act in the brief. Gates take about 30 s for an 85 s film; the brief asks under 0.8 s. Fixed? Open. The zoom search is brute force.

## Numbers

| Measure | Value | Basis |
|---|---|---|
| Script | 198 words, about 84 s at 142 wpm (83.7 s) | Measured |
| First-try check errors | fill 1: 11; fill 2: 11; fill 3: 12 | Measured |
| Re-asks used | fill 1: 22; fill 2: 21; fill 3: 23 | Measured |
| Fallback scenes | fill 1: 12; fill 2: 10; fill 3: 11 | Measured |
| Heal changes | fill 1: at least 12; fill 2: 11; fill 3: 14 | Measured |
| Variety, 60 to 86 s | fill 1: 0.15 (need 0.30); fill 2: 0.42 (need 0.30); fill 3: 0.0 (need 0.3) | Measured |
| Longest no-change stretch | fill 1: 5.25 s; fill 2: 5.5 s; fill 3: 1.5 s (limit 7 s) | Measured |
| Judge scores | fill 1: 3, 3, 4; fill 2: 4, 5, 4; fill 3: 4, 5, 5 (mean 4.1 of 9) | Judged |
| Hand-directed proof | 85.17 s; judge citation 7 | Measured; Judged |
| Proof render | 143 s, peak 637 MB | Measured |
| Gate run time | about 30 s for 85 s of film (brief: under 0.8 s) | Measured |
| Seconds under 35% drawn | fills 64, 64, 72%; strong-hand form 31%; real painting films 8%; 18 of 30 real films 0% (530 frames) | Measured |
| Movement meter | fills 66 to 73 of 85 s; real painting films 29 of 65 s | Measured |
| Type on plain ground | fills 37, 12, 16%; real painting films about 10% | Measured (fills); Estimated (real, by eye) |
| Picture changes, real painting films | about 15 a minute (13 clips) | Estimated |
| Picture supply in test | 4.9 a minute | Measured |
| Mark events after heal | 11 of 18, 7 of 20, 8 of 23; strong form 8 of 37 | Measured |
| Tests | juju-stage 28 pass; juju-reliquary 26 pass | Measured |
| Pictures gathered and kept | 184 gathered, 112 kept; 70 removed on first look, 2 on second; 14 refused for size | Measured; Judged (look) |
| Kept by source | Cleveland 57, Wellcome 27, Chicago 20, Getty 8; Met, Library of Congress, Biodiversity Heritage Library, NASA: 0 | Measured |
| Licences | CC0 64, Public Domain Mark 26, public domain 21, CC BY 1 | Measured |
| Size | all 112 at least 1600 px long side; 85 at least 1920 px wide | Measured |
| Disk | 336 MB pictures, 29 MB cache | Measured |
| Tiled-pattern score | highest 0.22 against reject line 0.45 | Measured |
| Wants with few pictures | 10 of 70 with 0; 22 with 1 | Measured |
| Pictures needed for 50 min film | 375 kept, 1,125 pulled | Estimated (pull time not measured) |

## Still open

- **The nine worlds.** The diagnosis says ENGINE-2.md lists nine worlds with slots, movement and picture need, plus a build order. That document is not in this input, so the worlds cannot be described here.
- **Fallback counts disagree.** The fill reports give 10 to 12 fallbacks each. The diagnosis says these films had no fallback scenes and heal made only small changes (3 marks, 1 flip, 1 split). Which is right is unknown.
- **No weak-model re-ask loop yet.** The check reports paths and allowed values. A loop that asks a model again is not built. First-time-right odds for a weak model are unknown, since no weak-model fill was run on the proof pack.
- **Pictures in the Met gap.** Nine Met objects named in research could not be fetched, because the image host blocks automated downloads. Library of Congress and Biodiversity Heritage Library answered with blocks.
- **Footage.** The Prelinger adapter is tested on a real answer, but no clip was fetched. Cutting one shot from a film is not built.
- **Wants with no pictures.** Ten wants still have no picture, including the Greek armour and the Bede page.
- **The judge cross-check.** The judges' full notes are not on disk; only a commit line ("about 4 of 10") remains. The strong-hand form has a measurement but no verdict. The advisor was rate-limited, so the diagnosis had no second reviewer.
- **Who pays for planning.** One strong planning call per film is proposed. Its cost is not known, and no world has been built or timed.
