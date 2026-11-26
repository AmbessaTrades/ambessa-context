# Juju now

As of 22:39 EAT, Thu 26 Nov 2026. Written every two hours by claude-haiku-5-5 (medium) from facts collected by code and the lead agent's own messages. Reports are not proof.

## Changed since the last sheet
- Covers 20:08 to 22:39 EAT, Thu 26 Nov 2026. Facts as of 22:39.
- Main: last commit 446e356e (21:35, 0.4.2). Five commits since 20:08.
- Phone: 0.3.8 and 0.3.9 (20:33, engine c1f4591c), then 0.4.0 (21:10), 0.4.1 (21:25), 0.4.2 (21:39). Current phone build: 0.4.2.
- Web: 0.4.2 live at 21:39.
- Mac app: 0.4.2, restarted 21:39.
- Door: 410c250a (20:33), 5ca8b342 with the learn route (21:10), 0ff5cb31 with the export chain (21:39). Door tests 63 of 63 pass at 21:39.
- Money ledger: 10,632 calls, $36.11 in all. Up about one cent since 20:08.
- Pull requests: 8 open, 19 merged, 1 closed (unchanged). PR 28, "High Juju: two modes", is open with a failing check.
- Rust: 37,524 lines (was 37,404).
- Film runs on disk: 4 DONE, 4 FAILED, 24 HOLD (unchanged). The worker reports an 11-minute test film, zz-len11, held at room 4. It is not in the disk count.

## What worked and what failed
**Worked (as reported)**
- Length: 11 minutes asked gave 44 stops and a 9.4-minute film (worker, 20:40; TEHUTI, 20:33). Mac build only, held (see below).
- Confirm sheet before a film shows length, time, money and first download. Checked on the live web at phone size (TEHUTI, 20:33).
- Gris-gris and High Juju switch works on the live web (TEHUTI, 20:08).
- Learn from a film: Door watch of Ambi's USA maps link. 55 s, $0.20, 19 shots, 10 rules, 6 topics (worker, 21:10). In a test space, link to lesson to rules on the channel ran end to end.
- Absorb: the same handle twice opens the first channel; a video link is redirected; a bad link is refused (live web, 21:25).
- Delete a channel: 422 without the word DELETE, 200 with it (live web, 21:25).
- Upload chain: DeepSeek's real step-90 idea was "Does Your Province Have These? (15 Maps)" (worker, 21:39).
- Live sweep: nine GET routes answered; five rooms load with no script errors. Mac: nine routes answer 200 while signed in (worker, 21:38).

**Failed or refused**
- The 11-minute test was held at room 4. Twenty coloured countries had no name, and Russia and Australia shake a few pixels between frames (worker, 20:40). The last three short money films (14 stops each) were held the same way, so the fault is older than today.
- Phone films are not held by room 4, because the check is not built on the phone.
- Ambi (17:40, as quoted by the lead): "we're here to fix juju, not ... the specific video."
- Ambi refused Deep Time ("ugly") and said "forget Neon if expensive" (last sheet). Parked. The learn route uses gemini-4-neon (21:10). This is not reconciled.
- Five test runs locked Ambi's PIN for 15 minutes (19:39). The Door no longer signs in as him in tests.

## App engine and films
- juju-core and timemap.py take the film length. Each stop is 13 seconds. Stops are no longer capped at 18.
- The steer line reaches every words call (TEHUTI, 20:33).
- Learned rules go into every words call as "STYLE TO FOLLOW" (TEHUTI, 21:10). No phone film has used them yet.
- Room 4 fix (proposed by the worker): give every coloured country its name, and stop names shaking. It goes in the shared map code, so Mac and phone both get it. The worker estimates 1 to 2 hours plus a test film. Not started. It waits on Ambi's reply.
- Export 720p or 1080p redraws the film at the new size and reuses the paid script and voice (worker, 21:39). Not run on a real phone.
- The Mac sends its Claude plan reading to the Door (21:22). The last reading seen was 1% left (19:39).
- High Juju sends writing and storyboard roles to Claude Opus 5.5 (last sheet). No real film on the phone has used it.
- The debt film has not been redrawn on the fixed code. Ambi's rehearsal showed Jordan, Sudan and Congo for "biggest economies" (fixed in code, not drawn).

## Web app and rooms
- Live at 0.4.2. Five rooms load clean: Altar, New Vessel, Crossroads, Cauldron, Shelf.
- New since 20:08: the DELETE sheet on every channel card; absorb studies the best film; Learn from a film; the upload kit opens (it said "Not built yet"); "Uploaded? paste the link" in Cauldron and Shelf; Crossroads marks chain ideas "Follows your hit · 90%"; export buttons in the Cauldron.
- Still wrong: five High Juju looks (Duppy Day, City Towers, Contagion Pulse, Crude Ledger, Engraved Atlas) have no films or colours (19:39).
- Mend (fix a film) answers only on the Mac.
- Rooms missing since the last sheet, not re-reported: Bend, Fill the week, the composer, Conjuring receipt.

## Mac app and APK
- Mac app: 0.4.2. Signs in to the Door with its own key, learns from films through it, sends the Claude plan reading, and reports its version (21:22).
- Phone: 0.4.2 released (21:39). Only one APK file is on disk (FACTS).
- Phone on a real device: not tested. The one emulator run used earlier builds.
- DMG for the Mac: still next time (19:28).

## Agents running now
- Worker (TEHUTI): last message 21:39 (0.4.2 shipped). Session end logged 22:18.
- Lead: last message 18:05 (credits ran out).
- Agent transcripts written in the last 10 minutes: 0.
- The live agent page did not answer, so running agents are unknown.
- Mac load (1, 5, 15 min): 14, 15, 17.

## Money spent on services
- Ledger at 22:39: 10,632 calls, $36.11 in all. DeepSeek 11.11, OpenRouter 12.27, Google 8.39, Inworld 3.92, unsettled 0.14, WaveSpeed 0.29.
- The $35 cap was passed at the last sheet. No ruling since.
- Door cap: 5 US (lead, 15:04). No change reported.
- Learn from a film: $0.20 for the USA lesson, and about 3 cents for the first test watch (worker, 20:58). The Gemini watch is not in the ledger figures above; Google stays at $8.39.
- Claude API: one count_tokens check per hour, free. One real Opus call under 1 cent (19:39). Claude is not a ledger line.

## Broken, blocked or open
- Room 4 label fix: not started.
- Five High Juju looks: no colours or films (last report 19:39).
- juju-core high_on does not read lean.api (20:08).
- Not run: export on a real phone; the upload chain on a real upload; a phone film using learned rules; the learn route on Ambi's own account.
- Phone: no real-device test; first sign-in on a physical phone not checked.
- Door sync needs Ambi's Gate sign-in. Not done.
- PR 28 has a failing check.
- Not proven: a voiced film over 10 minutes; a film on 0.4.2; the 95 of 100 taste bar; that a cheap model fills recipes at 95% legal first answers.

## Waiting on Ambi
1. Reply "go labels" to start the room 4 label fix (worker, 20:40).
2. Install 0.4.2. Open a finished film in the Cauldron, tap 720p, and check the phone's Movies folder when it says done (worker, 21:39).
3. On the phone, paste the USA maps link under Learn from a film and wait for "Learned 10 rules" (worker, 21:10).
4. Remove the two extra channels added by accident: tap the bin, type DELETE, tap Delete (worker, 21:25).
5. Say whether the $35 cap still holds.
6. Rule on "forget Neon if expensive" against the learn route, which uses gemini-4-neon.
7. Say whether to build colours and films for the five High Juju looks now.
8. Plug in a real Galaxy. Phone tests have run on an emulator only.
9. Rule on night on two grounds: parked, no ruling.

## Counted by code

- Pull requests: 8 open, 19 merged, 1 closed
- Paid calls in the test ledger: 10632, $36.1077 in all {deepseek: 11.1059, openrouter: 12.269, google: 8.3851, inworld: 3.9231, unsettled: 0.1365, lead-test: 0.0, wavespeed: 0.288}
- Paid services answering: deepseek 6537 ok, 23 refused or failed, last ok 26 Nov 20:27 EAT; openrouter 3411 ok, 47 refused or failed, last ok 26 Nov 16:38 EAT; google 119 ok, 16 refused or failed, last ok 26 Nov 13:59 EAT; inworld 458 ok, 1 refused or failed, last ok 26 Nov 10:54 EAT; unsettled 0 ok, 9 refused or failed, last ok None; lead-test 0 ok, 3 refused or failed, last ok None; wavespeed 6 ok, 2 refused or failed, last ok 25 Nov 11:24 EAT
- Rust: 37,524 lines in 15 crates. Skills: 59. Rooms drawn: 22. Decisions: 27. APK files built: 1
- Design-system libraries on disk: camera_motion.json, fonts, house, kits, looks, palettes.json, proof, proto, work-camera_motion, work-palettes, work-quotes, work-surfaces_light, work-typography
- Finish check: 1 of 23 clauses true, so not done
- Whole-film runs of `juju make` on disk: 4 DONE, 4 FAILED, 24 HOLD
- Newest film runs: ottoman12f HOLD 25 Nov 11:25 (stopped at Pictures and form); proof12c FAILED 25 Nov 09:47 (stopped at Render and mix); proof12 HOLD 25 Nov 09:16 (stopped at Script and heal); proof75b HOLD 25 Nov 09:06 (stopped at Render and mix); proof75a HOLD 25 Nov 08:59 (stopped at Publish kit); strip-planets HOLD 25 Nov 08:41 (stopped at Deal and package); strip-pluto HOLD 25 Nov 08:40 (stopped at Render and mix); 20261125-083722-131d HOLD 25 Nov 08:37 (stopped at Deal and package); strip-japan DONE 25 Nov 08:34 (60 s, 0.008751 US); strip-bulgaria HOLD 25 Nov 08:11 (stopped at Deal and package); strip-austria HOLD 25 Nov 08:11 (stopped at Deal and package); strip-manchuria HOLD 25 Nov 08:11 (stopped at Deal and package)
- Agent transcripts written to in the last 10 minutes (all Claude work on this Mac, mostly Juju): 0
- Logged attempts: 433 kept, 63 reverted, 52 inconclusive
- Mac load (1, 5, 15 min): [14, 15, 17]
- The live agent page did not answer, so running agents are unknown
