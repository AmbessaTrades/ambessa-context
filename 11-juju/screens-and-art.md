> **State of 24 Nov, 13:10.** Later facts win: [worked-and-failed](worked-and-failed.md), [../10-now/now.md](../10-now/now.md).

# Juju screens and art: three directions, quiet copy, round-2 rooms, and the Library of Tehuti variety

As of 13:10 EAT, 24 Nov 2026. Source: design jobs a workflow (art directions), a workflow (quiet copy and parts sheet), a workflow (round-2 base, rooms and variety).

> **Read with this:** carved ink won 17 of 30 and was refined; the rooms in the gallery are the round-2 rooms that followed. Ambi's words on art are in `what-ambi-said.md`.

## In short

- Three art directions were built, each on its own kit: struck-metal panels, carved stone, and lit lanterns on a night ledge. Each was judged on craft, world and cold reading. Every judge score was 5 or 6.
- The quiet rule (names and verbs only, with word caps) went into the shot checker. The parts sheet fell from 728 interface words to 186 at 1440 px, with zero faults.
- Round 2 built a shared base and three rooms (Offering, Reliquary, Canopy) across 41 states. The default Canopy state passes its check. The all-state check did not finish.
- The Library of Tehuti variety design (10 film kinds, 10 variety rules, a 28-day calendar) passes its own checker. A solver found that a daily schedule under every rule needs 9 kinds. Today's worlds give 5.
- Open: no art direction is chosen, the voice model is unset, the extra worlds are unbuilt, and the listening and thumbnail tests are designed but not run.

## What was done

**Art directions.** Three makers drew the same screens: an altar (the vessel shelf), a tank (money and keys) and an art sheet that shows every object in every state. Each library drew working, many-channel , locked and sample states. Render rounds: about 9 for panels, 8 for nightlit, about 11 for carved. The shot checker reported zero faults on altar and tank at both widths for all three. Only carved got a refinement pass after the judges (5 more rounds). The file records no refinement for panels or nightlit.

**Judging.** Each direction got three reads: craft (does it look made), world (is it one hand and one place) and logic (can a cold reader name each object in about three seconds).

**Quiet work.** The copy list covers 19 rooms: 55 status words, 134 verbs, and one action per flow state. The worst counted screen is the Tank at 25 words on desktop (cap 30) and 23 on phone (cap 24). Then the parts sheet was cut to names and state words. Explanatory lines, plate sentences and demo prices went. Catalogue words (looks, voices, donor names) are marked as data, which the checker excludes. The repair pass added a large seal badge for the Done jar, removed the tree's state words, moved the padlocks beside the wallets, and moved the "use these parts" bar to the end of the sheet so it no longer covered the wallet jars.

**Round 2.** The base uses kit2.css, kit2.js, light.js and art.js. Objects are lit from the upper left, with shadow and engraved lines. Build scripts bake them into 91 light maps (light.js, 2.2 MB), so the four skins (Nocturne, Codex, Atelier, Daylight) all switch on the same maps. The art sheet took 11 rounds and shows zero faults at both widths. Rooms: Offering (11 states, 6 rounds), Reliquary (15 states, 5 rounds) and Canopy (15 states, 4 rounds, one short of the five asked for). There are three doors only. The Tank is a fixed chip at the right end of the head in every room.

**Variety.** Ten film kinds: Crossing, Trial, Clock, Reach, Root, Ladder, Mirror, Works, Trail and Witness. Each has its own question, its own way of arguing, a list of material that must be on disk first, and a rule for what it may not share with yesterday. The design also has ten variety rules (V1 to V10), the brief's rules H1 to H4 and H6, three thumbnail and colour rules, 11 thumbnail families, and seven title equations kept (five cut, each with a reason). A solver built a 28-day calendar with day 1 fixed to the first film. A separate checker that read only the files found zero faults.

## Breakthroughs

1. **The state-on-the-mouth vessel system.** Judged. In each direction the judges named the central object as the best element: the coin with a lamp (panels), the amphora whose mouth carries the state (carved), and the lone gold lantern among dark ones (nightlit). The many-channel wall stays readable because the gold "needs you" items stand out. Evidence is judge text, not a timed test.
2. **The colour rule is measured.** Measured. Across 62 outlier plates, bright turquoise covers more than 1 percent of the frame in only 4. Red, gold and blue each do so in 26 to 28. The umbrella colour rule (turquoise means on record) rests on this count.
3. **The quiet parts sheet passes its checks.** Measured. Interface words fell from 728 to 186 at 1440 and 184 at 390. QUIET faults fell from 46 per width to 0.

No judge scored any direction above 6, and none is called finished.

## What critics found

- **Old fasting-walkthrough title on the altar.** Brief law 8 bans it. The carved world judge, and the nightlit logic and world judges, found it in every altar state. Carved: fixed. It now shows an empty plate, because the sample film file does not exist yet. Nightlit: open, since it was not refined. Panels: the file does not say.
- **Jade means both "working or locked" and "press me".** A panels judge found the bright jade "Make a film" and "Lock spending" beat the gold action that actually waits on you. Open. Nothing in the file changes it.
- **A full jade test fuse read as money ready to spend.** A carved logic judge found it. The refinement draws the limit in hollow slate and never in jade. Fixed per the maker. Not re-judged.
- **Empty wallets read as drained, not never funded.** A panels logic judge found the six solid tubes labelled "$0 left" looked like money had run out. The carved refinement draws empty glass as a clean dry floor, labelled as never funded. Fixed per the maker. Not re-judged.
- **Room marks misread.** A carved logic judge read crossroads as a snowflake or gear, the tank as a bar chart, and the cauldron as a teacup. The Tank now has a rail and phone-bar entry (fixed). The marks themselves were not redrawn in the file (open).
- **Padlock and gold selection.** A nightlit logic judge found the open padlock looked shut, and the gold lantern read as "selected" rather than "needs you". Open.
- **Moon in the wrong place.** The nightlit rule places the moon in the gap between the first two glasses. In the sample state it sat above glass two. Open.
- **Phone tank detail under the fixed bar.** A carved world judge found it covered the detail panel. The refinement moves the wallet detail into a sheet. Fixed per the maker. The free-services row still sits under the bar at first view, which the maker notes (partly open).
- **Desk-view overlap.** A cold reader found the "use these parts" bar covering the wallet jars. Fixed by moving the bar to the end of the sheet.
- **Second card row overflows at 390 px.** A cold reader saw it run off the right edge. Unknown. The repair list does not mention it.
- **Tree labels do not match branches.** The repair removed the state words and moved each bough's name under its own bough. The maker reports this; no reader re-checked it. Partly fixed.
- **A daily calendar needs 9 kinds.** A solver found that 4, 7 and 8 kinds fail every rule and 9 pass. Today's worlds allow 5 kinds and only 11 of the 28 days. Open. Building archive footage, a lineage tree and an instrument view would give the extra kinds.
- **A title frame repeats.** EQ_08 lands on 6 of 28 days (conflict C8). Open.
- **Two films too close in story.** A checker found day 26 put a Gilgamesh film six days after a flood-story film, which the rules had missed. The maker fixed it by hand and extended rule V7 to check the story each film is built on. Fixed.
- **Canopy not fully checked.** The default state passes the truth check with zero hits. The all-state check was still queued when the work stopped. Open.
- **Reliquary sources sheet.** Opened on load, it goes over the 24-word phone cap, because the page behind it is counted too. The maker calls this a flaw in the check, not the room. Open.

## Numbers

| Measure | Value | Basis |
|---|---|---|
| Judge scores, panels (craft / world / logic) | 6 / 5 / 6 | Judged |
| Judge scores, carved | 6 / 6 / 5 | Judged |
| Judge scores, nightlit | 6 / 6 / 5 | Judged |
| Cold read, panels | about 7 of 11 objects right | Judged |
| Cold read, carved | about 6 of 17 meanings; 7 partly; 4 missed | Judged |
| Cold read, nightlit | 8 of 17 right; 5 partly; 4 wrong | Judged |
| Cold reader, quiet desk view | sure of 16 of 40 objects | Judged |
| Render rounds: panels / nightlit / carved | about 9 / 8 / about 11, plus 5 refine | Measured |
| Shot-checker faults, altar and tank, both widths | 0 in all three directions | Measured |
| Outlier plates with turquoise over 1% of frame | 4 of 62 (red, gold, blue: 26 to 28) | Measured |
| Turquoise contrast on dark ground | 9.29 to 1 | Measured |
| Counted copy screen, Tank | 25 words desktop (cap 30); 23 phone (cap 24) | Measured |
| Copy list | 19 rooms; 55 status words; 134 verbs | Measured |
| Interface words, parts sheet | 728, then 206 / 204, then 186 / 184 (1440 / 390) | Measured |
| QUIET faults per width, parts sheet | 46, then 0 | Measured |
| Light maps and light.js size | 91 maps; 2.2 MB | Measured |
| Round-2 states | 41 (Offering 11, Reliquary 15, Canopy 15) | Measured |
| Round-2 render rounds | Offering 6, Reliquary 5, Canopy 4, sheet 11 | Measured |
| Film kinds, variety rules, thumbnail families | 10; 10 (V1 to V10); 11 | Measured |
| Thumbnail layout threshold | 0.42 against yesterday; 0.55 against last 15 (from 1,840 pairs) | Measured |
| Kinds needed for a daily schedule | 9 pass; 4, 7 and 8 fail | Measured |
| Days possible with today's 5 kinds | 11 of 28 | Measured |
| Neighbouring-day difference | at least 13 of 14 traits; at least 7 within 15 days | Measured |
| Title frame EQ_08 repeats | 6 of 28 days | Measured |
| Open conflicts in the variety file | 10 (C1 to C10) | Measured |
| Weekly pictures kept | about 2,000 to 2,600 | Estimated |
| Overnight rendering per week | 12 to 23 hours | Estimated |
| Weekly cost | about $14 | Estimated |
| Effort per film (quick / crafted / masterwork) | $1.74 / $2.00 / $2.81, from ADR 0006 | Estimated |

## Still open

- **Direction choice.** No art direction is decided, and Ambi has not approved one. The file does not say which direction round 2 builds on.
- **Judged craft.** Judges called all three clean but generic. Panels, carved and nightlit each still need extra depth, and the judges asked for a hand-made illustration per room.
- **Voice model.** The variety file leaves the voice empty. ADR 0005 names TTS-2, but the model name, speed and temperature from the older setup are unconfirmed.
- **Daily output.** Either build three new worlds for 9 kinds, or run 5 kinds with the pair rule loosened. This is the owner's decision.
- **Upload start.** uploads=0 starts the channel in a graft phase, where 85 percent of ideas come from outside outliers. The brief's section 19.2 says to bloom at once. The two conflict; the file does not resolve it.
- **Tests not run.** The listening test (masked ABX on three pairs, pass at 7 of 8 with two controls) and the thumbnail test (describe, then find among 7 lures) are designed, not run.
- **Estimates.** Effort costs and receipt totals are estimates with no measurement. Keeping or dropping them is the owner's call.
- **Unchecked content.** Subject seeds in the calendar have not been verified. The Held 35% dial has no clear meaning to a new reader.
- **Motion.** Flame, steam, press and seal were checked only as still frames.
- **Canvas.** The push script inlines only kit.css, so round-2 rooms cannot yet go onto the canvas.
- **Round-2 finishing.** Canopy's all-state check and the Reliquary check flaw are open. Canopy's tree on phone is busy and its growing, hit and flop states were seen only on desktop, or not at all.
