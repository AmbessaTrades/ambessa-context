# Juju page map: the 19 rooms

As of 13:10 EAT, 24 Nov 2026. Source: flow specs in `mockups/flow` (journeys.json, order.json) and the walk, repair and board-judge jobs of the same pass.

> **Read with this:** the rooms themselves have been rebuilt since (gallery, "Juju — rooms"). Every number of seconds below is an estimate by the lead.

## In short

- Juju's app was specified as 19 rooms, each with a flow file. Three walk jobs traced real journeys through them and found 42 breaks. A board judge found 10 more.
- The repair pass patched the specs. Nothing was built, run on a phone, or timed.
- The walks found the worst breaks in money and keys: a new install starts in Practice, a paid film cannot be finished on a test budget, and a key pasted on one device is not seen by the Mac.
- Still open: the time budget (three films take 1,045 s hand-published, against a 900 s target), no look is ready, and sound-mode ownership.

## What was done

- 19 room files, one `order.json` with 218 leaving actions, and a `journeys.json` with 193 timed steps across four journeys.
- A board of 658 frames (19 rooms, 329 states, phone and desktop), 218 arrows, and a canvas with 7,886 wired clicks.
- Journeys: "a first film" (63 steps: 37 person, 26 agent), "a new channel on the phone" (70 steps: 49 person, 21 agent), "things go wrong" (46 steps: 31 person, 15 agent), and "after day 30" (14 steps, not timed). The last was added in the repair pass.
- Speed law: a new skill, asase-velocity, with seven steps and a budget table. It is linked into the skill folders (34 skills). Its Rust count test was not run because the crate could not resolve offline.

## Breakthroughs

None. Nothing was built, run or timed. The counts above are file counts.

## What critics found

Walk jobs: 42 findings. Kinds: dead end 14, missing agent step 6, too slow 5, phone gap 5, missing option 4, untrue 4, duplicate option 3, unclear 1. Board judge: 10 findings (dead end 3, unclear 3, phone gap 2, untrue 2). Each finding below names the walk that showed it.

1. **New install cannot pay for a film.** Shown by the new-channel walk and the first-film walk. Every install starts in Practice. Real mode is Ambi-only and is not shown on the second operator's phone. The 75 cent test fuse stops a 50 minute film, whose voice alone is about $0.81 (estimate). Status: fixed in spec for the phone path (shared mode line, Ask Ambi button). Open: who may open Real, and whether test money resets.
2. **A key on the wrong device.** Shown by the things-go-wrong walk. A key pasted on the phone is not read by the Mac, so the film fails on the Mac with a missing key. The loop ends only when Ambi opens the Mac. Status: fixed in spec (check the key on the device that makes the film; one Ask Ambi button; no key travels between devices).
3. **Two states for one fact.** Shown by the things-go-wrong walk. With no key, one state lights Incant for a free run and another dims it. Status: fixed in spec (mode decides first, one rule in pact, voice and conjuring).
4. **Nothing to deal on a new channel.** Shown by the new-channel walk. The deal reads only saved scans, and a new channel has none. Status: fixed in spec (new-vessel writes the first saved scan from the films it reads).
5. **Failed fact check loops.** Shown by the things-go-wrong walk. Try again reruns the same check on an unchanged script, so the second try gives the same answer. Unsourced lines are cut without a limit. Status: fixed in spec (failed sentences go back to the writer with their passage; a gather-passages step is added). Open: the 10 percent stop threshold is a candidate, untested.
6. **Render stops silently.** Shown by the things-go-wrong walk. A render has no heartbeat, so a stuck film can show "about 1 hour left" all night and block the next films in the queue. Status: fixed in spec (a watch on frames, one restart, the queue moves past a stuck film). Unbuilt.
7. **Thumbnails fail the phone-size check.** Shown by the things-go-wrong walk. Three paid pictures can all fail, and the only route back is a loop to paid painting. Status: fixed in spec (a "make it simpler" state, at most two paid rounds). Unbuilt.
8. **Approve cannot finish.** Shown by the first-film and things-go-wrong walks. Approve waits for two fresh reviewers, and the strip has no way to ask them again. Status: fixed in spec (ask again, or approve marked "not reviewed" after 180 s). Open: whether the three lamps stay required.
9. **Upload check reads a stale answer.** Shown by the first-film walk. The link check needs a YouTube channel link that is never asked for, and it can say "It is live" for a film nobody can see. Status: fixed in spec (fresh public read, states for not public and scheduled).
10. **Subtitles and sound.** Shown by the new-channel walk. A silent channel's controls talk about spoken words, and the captions file would print the subtitles twice. Sound mode can be changed in four rooms. Status: captions fixed in spec. Open: sound mode ownership, which the brief and the stage rules disagree on.
11. **The board is hard to read.** Shown by the board judge. Desktop frames are empty boxes. Phone frames are paragraphs with code chips, and the board-wide image is unreadable at phone width. Arrows land on a room's first state, so Watch on a ready film opens "no film". Journey steps repeat button names. Status: unknown. No repair of the board is reported. Three things are present in the files: `lands_on` in order.json, the after-day-30 journey, and journeys that end back at the altar.

## Numbers

| Measure | Value | Status | Source |
|---|---|---|---|
| Rooms | 19 | Measured | order.json |
| Leaving actions | 218 | Measured | order.json |
| Board frames | 658 for 329 states | Measured | board job |
| Canvas clicks wired | 7,886 | Measured | board job |
| Steps: first film / new channel / things go wrong / after day 30 | 63 / 70 / 46 / 14 | Measured | journeys.json |
| Person seconds: first film | 418 (53 once only) | Estimated | journeys.json |
| Person seconds: new channel | 439 (19 once only) | Estimated | journeys.json |
| Person seconds: things go wrong | 155 | Estimated | journeys.json |
| Three films, made and queued to approve | 595 s | Estimated | journeys.json |
| Three films, published, Juju uploads unlisted | 730 s | Estimated | journeys.json |
| Three films, published by hand in Studio | 1,045 s against 900 | Estimated | journeys.json |
| First-film walk before repair | 347 s a film, 1,033 s for three | Estimated | walk job |
| Render speed, measured | 0.42x realtime on a busy Mac | Measured | speed skill, open risks |
| Render speed, brief target | 4x to 8x realtime | Estimated | speed skill (target only) |
| Frame drawer | 12 fps at load 22; 6.1 fps on full proof | Measured | open risks, quoted in speed skill |
| Encode, one clip | 1.92 s with hardware, 7.52 s in software | Measured | open risks, quoted in speed skill |
| 50 minute film, frames | 72,000 | Estimated | arithmetic at 24 fps |
| 50 minute film, render | about 100 min to 3.3 h | Estimated | from measured rate |
| 50 minute film, drawing in spec | 7,200 s | Estimated | conjuring spec |
| Voice cost, 50 minute film | about $0.81 against $0.75 test fuse | Estimated | pact spec |
| Reading clock, 12 word card | about 4.25 s | Estimated | spec rule |
| Graft read, one dated video | about 10 s | Measured | crossroads walk, busy Mac |
| Lamps, share of 50 minute film | 75 s, 2.5 percent | Estimated | spell-strip spec |
| Walk findings | 42 | Judged | walk jobs |
| Board findings | 10 | Judged | board judge |

## The speed law

The asase-velocity skill sets the budget. The brief target is taps under 900 s for three films, about 300 s a film (inferred). Machine work before render starts must be under 90 s (brief target, not measured). Renders are targeted at 4x to 8x realtime, but the measured rate is 0.42x, so a 50 minute film needs overnight Mac time. The rules are: no required human take (ADR 0002), a film is scenes in acts, a screen never waits (slow work runs as a background job), and every speed claim is re-timed on an idle Mac.

The skill and the repaired specs conflict. The skill says one fix re-renders its act chunk. The repaired specs say only the changed scene is redrawn. Neither is built, because the renderer has no scene-level segments. The skill also lists three conflicts it did not settle: the required watch in brief 3.2 against ADR 0002, the 4x to 8x and 90 s figures against open risks, and brief 16.2 against ADR 0004.

## The 19 rooms

Purpose and action come from the journey rows and the order.json labels, because ROOMS.md is not among the inputs. "Action" is the room's main forward step. Where it leads comes from order.json.

- **gate**: Lock screen and person switch. Action: enter the PIN. Leads to the altar.
- **altar**: Home shelf; each channel shows its one need. Action: Make a film. Leads to crossroads.
- **new-vessel**: Reads a reference link and learns its sound, shape and point of view. Action: Absorb. Leads to the vessel once read.
- **vessel**: A channel's own settings: story, voice, sound, thumbnails, sources. Action: Make a film. Leads to crossroads.
- **crossroads**: The deal of seven cards from the saved scan. Action: Take this card. Leads to the pact.
- **mirror-bend**: Paints the thumbnail in three versions. Action: Keep this version. Leads to feed-sight.
- **feed-sight**: Tests the thumbnail at phone size. Action: Use it. Leads to the pact.
- **cauldron**: The pot of ideas for the next film. Action: Review the pact. Leads to the pact.
- **arcana**: Chooses the film's look. Action: Wear this look. Leads to conjuring for the film being made.
- **pact**: The receipt, a sealed contract for one film. Action: Incant. Leads to conjuring.
- **conjuring**: The making of the film; acts draw one by one. Action: Leave it working. Leads to the altar.
- **spell-strip**: Scene-by-scene fixing and approval. Action: Approve the film. Leads to publish-kit.
- **publish-kit**: Title, description, thumbnail, upload and pinned comment. Action: Copy the title. Leads to the altar. ROOMS.md says "Copy everything", and no control carries that name.
- **canopy**: Results tree and the day 30 numbers. Action: Save the day 30 numbers. Leads to the offering or to the cauldron.
- **offering**: Product mention for a channel. Action: Start the product work. Leads to the canopy or the shelf.
- **sound**: The channel's set of music and sounds. Action: Hear the set and keep what is good. Leads to the vessel.
- **voice**: Choice of voice for a film. Action: Use this voice and carry on. Leads to conjuring.
- **reliquary**: Holds sources and pictures a film may use. Action: Use it and carry on. Leads to conjuring.
- **tank**: Money, keys and the test fuse. Action: paste a service key. Leads back to the room the person came from.

The crossroads main button changes with state (Deal seven, Take this card, Paint three), while ROOMS.md names one action per room.

## Journeys

- **A first film** (11 rooms): setup once (key, test film, voice), then one film from the crossroads through pact, conjuring, spell-strip and publish-kit. 418 person seconds, 53 of them once only, 2 steps untimed. Three films take 365 s for the first and 340 s for each next one.
- **A new channel on the phone**: the same path, starting at a reference. 439 person seconds, 19 once only, 4 steps untimed. The reference read needs the Mac today.
- **Things go wrong**: seven failures walked, each with both branches. 155 person seconds, 2 steps untimed.
- **After day 30**: canopy, offering and cauldron, after a film is 30 days old. Nothing timed (10 untimed steps), so no person total exists.

## Still open

- Nothing is timed. One walk on a Mac and one on a real Android phone are needed before any estimate is quoted.
- No look is Ready, so Make a film cannot light for the first channel until two looks and their proofs exist.
- Sound mode: set once for the channel (the repair's choice), or changed per film (the brief). For Ambi.
- Health lines: written out by default, or held for a named person's sign-off. ADR 0002 says no sign-off is required. For Ambi.
- Whether the three lamps and the two reviewers stay required. For Ambi.
- Who may open Spend for real, and whether the 75 cent test money ever resets.
- Where music beds come from. No music model is used.
- Phone features are specified but unbuilt: YouTube reads, drawing, sound making, offline queues and upload. No APK exists.
- Gaps: ROOMS.md was not in the inputs. Per-room state counts are not derived here, and only the total (329) is reported.
