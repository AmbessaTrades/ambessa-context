> **State of 24 Nov, 13:10.** Later facts win: [worked-and-failed](worked-and-failed.md), [../10-now/now.md](../10-now/now.md).

# Juju: ability coverage, three skeptic attacks, and the round-1 room review

As of 13:10 EAT, 24 Nov 2026. Source: workflow outputs a workflow (ability map, merge and three attacks) and a workflow (five room reviews).

> **Read with this:** written from the morning's raw results. Two things moved since. (1) The merged table counts **262** abilities (95 kept, 57 kept better, 77 missing, 14 unclear, 19 dropped); the 342 below are the raw rows before duplicates were merged. (2) The attack on "almost nothing exists" described three crates; by 13:10 there were eight, about 11,700 lines of Rust (`02-the-software.md`). An attack finding stays open until a check or a real run closes it.

## In short

- The studied app was mapped into 342 raw ability rows over three passes. Juju keeps or improves 198 (58%), marks 16 unclear and misses 101 (30%). Some recur across passes; I did not dedupe. The task named 262, which the file does not reproduce.
- Three skeptic attacks say the plan would fail before a film ships: the platform's originality rule, a weak model's output passing every gate, and a render and phone plan the code cannot yet run. They raised 21 breaks, 10 marked as killers.
- Five room reviews (round 1) logged 40 findings, 9 of them blockers. The file marks none as fixed.
- Still open: the count gap, why the room loop stopped, and whether any fix was made.

## What was done

- **Ability map.** Three passes read the studied app's screens and Juju's prototype rooms. Each ability got a row with a verdict (kept, kept better, unclear, missing, dropped on purpose), the Juju room that covers it, and the frames it was seen in. Pass sizes were 95, 119 and 128 rows. A merge pass picked the ten most important gaps.
- **Attack 1, platform rule.** A critic read the platform's originality policy (fetched 24 Nov) against the plan.
- **Attack 2, weak model.** A critic ran the Rust heal command on a junk model reply. The linter was tested with a Python stand-in, not the Rust linter.
- **Attack 3, engine reality.** A critic measured the code tree, frame timings and peak memory on the Mac, and read the older engines' source.
- **Room review, round 1.** Five reviewers (crossroads, gate, mirror-bend, altar, vessel) each wrote a first impression, the strongest part, and findings with severity and a fix.

### Coverage of the studied app

Verdicts over the 342 rows: kept 135, kept better 63, unclear 16, missing 101, dropped on purpose 27. Dropped rows are mostly named faults (AI avatars, share-percent sliders, timeline controls) and public-service features (plans, billing, seats) that the brief rules out.

Juju does better where it swaps a control for proof: outlier ratios, cost in dollars, licence tickets on each relic. Missing rows cluster in three places. In the first pass, about 20 of the 50 are voice-library and voice-design items (library, favourites, search, provider and tier, cloning). Script tools (history, copy, new script, read before voice) and the mention menu (Drive, audio, folders, clip playback) are also missing. In the other passes, the gaps are channel management, per-film voice, A-roll rules, the film's ending and timeline-style edits.

The most important missing abilities. Rows 1 to 10 follow the merge's ranking; rows 11 to 15 come from the map passes.

| # | Ability | Where in the studied app | Juju status in the file |
|---|---|---|---|
| 1 | Read the AI script before voice is paid | Script stage | Pact promises it; Conjuring runs Script straight into Voice |
| 2 | Clone a voice from a recording or file | Voice Studio | Missing; Record and Own-file buttons do nothing |
| 3 | Thumbnail reference from a link or uploaded picture | Thumbnail picker | Missing; both inputs have no handler (Mirror Bend) |
| 4 | Cut a scene out | Editor | Missing; no removal action |
| 5 | Replace a scene picture with own file | Editor | Missing; "My own file" shows a toast only |
| 6 | Upload files to the library from the device | Media library | Missing; the "From this device" option matches no click branch |
| 7 | Swap the film's music | Editor | Missing; no room changes a film's music |
| 8 | Place a sound effect at a moment | Editor | Missing; the Sound room only keeps or drops sounds |
| 9 | Set how the film ends | Pre-flight | Missing; no room shows the ending before paying |
| 10 | Change the voice for one film only | Pre-flight | Missing; only speed works, and the link changes the channel voice |
| 11 | Turn off overlays and captions | Channel settings | Missing; no words-off switch |
| 12 | Turn off visual effects | Channel settings | Missing; no effects switch |
| 13 | Save a look as the channel default | Look picker | Missing; a look lasts one film |
| 14 | Rename, default, or delete a channel | Channel More sheets | Dead buttons |
| 15 | Redo a change | Editor | Missing; undo is a 7-second toast only |

## Breakthroughs

None. The file shows no end-to-end result. One measured number is a speed fact about existing encoders, not a Juju result, so it sits in Numbers only. The 85-second proof film exists, but its shots are hand-coded and its audio is silent.

## What critics found

Status is "open" unless the file says otherwise. The file records no fixes.

### Attack 1: platform originality rule

- **No human creative input (kills).** A model writes the film and a person approves 75 s of it (0:00-0:40, a 15 s middle span and the last 20 s). That is 4.2% of a 30-minute film. The policy covers mass-produced content without the creator's original perspective. Fix: each film needs a thesis and one claim written by an operator. Open.
- **Fixed story spines (kills).** Twelve title equations and a closed set of stage types give form variety but no substance variety. Fix: each film must add a new thing for its channel, checked by a blind swap test. Open.
- **Sequels and graft phase (costs quality).** A 90% similarity rule and 85% of early cards built from other channels' outliers make the first 12 uploads and their sequels close to interchangeable. Fix: a sequel must answer what the first film left open. Open.
- **Silent text films (costs quality).** At $0.12-0.15 for a 30-minute film, silent text with archive pictures risks the "scrolling text" clause. Fix: silent mode only for real stories. Open.
- **Titles (minor).** A first-person verb is used where no one did the act. Open.
- **Framing (costs time).** The brief treats the risk as rendering and misses the creator-perspective clause. Fix: a written law for operator input. Open.

### Attack 2: weak model

- **Junk output passes (kills).** The reply "sorry I cannot" was healed into a 9-scene film marked valid: 20 changes, 6 quote-canvas scenes, 2 rule cards, 1 chapter title. The pixel gates and renderer are stubs. Fix: stop above about 10% fallback scenes, and gate on real pixels. Open.
- **Nobody judges the story (kills).** No skill names the story law. The causal-share gate (0.72) reads link labels the model writes itself. In the sample script, stations 2 to 9 have empty lines. The experiment covers only the first three minutes. Open.
- **Wrong facts pass (kills).** The number law compares spoken and written numbers, not truth. An invented Seneca quote hit 0 rows in the Python stand-in. The proof film's sources are the channel's own old videos, on a health topic. Fix: a claim ledger with exact passages. Open.
- **Linter misses AI tells (costs quality).** Five sample lines with usual AI tells got 0 hits. The bracket rule flags TTS tags such as [breath]. Open.
- **Skills contradict each other (costs quality).** Four pairs of orders clash, including a main tension due within 22 s against a frame-wide-first rule, and a retention slot against a banned topic. Fix: one ranked rule list per pack. Open.
- **Numbers do not add up (costs time).** Nine clashes, for example a 900-1,500 ms silence against a 500 ms cap, and 3,500-4,300 words at 142 wpm (24.6-30.3 min) against a 14-minute price. Open.
- **Human checks the wrong thing (costs quality).** The human watches 75 s and never reads the script. The critic's proposed review takes about 14 min per film. Open.

### Attack 3: engine reality

- **Almost nothing exists (kills).** Three crates exist (127, 52 and 773 lines). Render, draw, stages and gates are stubs. The 18 tests cover check and heal only. Open.
- **Render speed (kills).** The brief claims 4x-8x realtime. The full 2,045 frames ran at 6.1 fps (335 s for an 85.2 s film). The GPU path does not exist. Open.
- **Memory ceiling broken on the Mac (kills).** The brief's 580 MB phone ceiling is already exceeded on the desktop: 432 MB for the render alone, about 1.03 GB with software encode. Open.
- **Phone path (kills).** Every engine calls the desktop ffmpeg, Python or OpenCV. No Android encode code exists. Earshot, the sound engine, is estimated at 11-16 days to port to the phone and has never run on Android. Open.
- **No APK, no phone (costs time).** No APK has been built and no phone is connected. Every phone claim is untested. Open.
- **Proof film (costs quality).** The 85.2 s film is silent (-91 dB), with 11 hand-written shots and three lossy encodes. The old pipeline's last full film cost $104.93 and was not uploaded. Open.
- **Day-2 smoke gate (costs time).** No juju binary exists, and several brief claims describe the old tools wrongly. Open.

### Room review, round 1

Forty findings: 9 blockers, 30 important, 1 nit. All are open.

- **Crossroads (2 blockers).** The donor's finished thumbnail fills the card above our title, so it reads as ours. The donor's multiple sits under our title with no owner. Taking a card loses it: the card id is not passed on.
- **Gate (no blockers).** The PIN strip reads as characters, not digits. ENTER looks ready with 0 or 3 digits. A first-run user has no way in, and a forgotten PIN has no way back.
- **Mirror Bend (4 blockers).** The right plate shows the donor's words with one noun changed, hard-coded. Paint never leaves the empty state. The link and picture inputs do nothing. "Same place" is shown for 49 of 63 outliers that were never measured (only 14 are).
- **Altar (1 blocker).** "Film ready" with a 25.3-minute length appears where only a script exists.
- **Vessel (2 blockers).** Two of six style plates are other channels' real thumbnails with their multiples, shown as the channel's own. Version history ("Pacing v3", "Go back to version 2") is invented.

The file holds only round-1 entries and no round 2. It gives no reason the loop stopped. Status: unknown.

## Numbers

| Metric | Value | Mark |
|---|---|---|
| Ability rows (raw) | 342; the task named 262 | Measured |
| Kept / kept better | 135 / 63 | Measured |
| Missing | 101 (19, 32, 50 by pass) | Measured |
| Unclear / dropped on purpose | 16 / 27 | Measured |
| Attack breaks | 21 (10 kill, 6 costs quality, 4 costs time, 1 minor) | Measured |
| Human span per film | 75 s of 1,478-1,817 s (4.1-5.1%) | Estimated |
| Heal test output | 9 scenes, marked valid | Measured |
| Crates and lines | 3; 127, 52, 773 | Measured |
| Frame rate, loaded machine | 12 fps (120 frames, load 22) | Measured |
| Frame rate, full film | 6.1 fps; 335 s for 85.2 s | Measured |
| 25-minute film at 6.1 fps | about 98 min | Estimated |
| Encode, 120 frames | 1.92 s hardware, 7.52 s software | Measured |
| Peak RAM, render | 432 MB; about 1.03 GB with software encode | Measured |
| Proof film | 85.2 s, silent at -91 dB | Measured |
| Old pipeline film spend | $104.93; 7 of 22 parts passing | Measured |
| Earshot phone port | 11-16 working days | Estimated |
| Mirror Bend outliers measured | 14 of 63 | Measured |
| Borrowed style plates | 2 of 6 | Measured |
| Room findings | 40 (9 blockers, 30 important, 1 nit) | Judged |

## Still open

- The 262 count against 342 raw rows, and the source of 262.
- Why the round-1 room loop stopped, and whether a round 2 was planned.
- Whether any attack or room finding was fixed. The file records none.
- Render speed and phone memory were measured once on a loaded machine; no re-measurement exists.
- Per-film voice, A-roll rules, the closing takeaway and channel management are missing in the prototype.
- The 16 unclear rows need an owner's decision.
