# Juju now

As of 10:27 EAT, Wed 25 Nov 2026. Written every two hours by claude-haiku-5-5 (medium) from facts collected by code and the lead agent's own messages. Reports are not proof.

## Changed since the last sheet
- Covers 08:23 to 10:27 EAT, Wed 25 Nov 2026.
- Paid calls: 6,029 calls, $8.0822 in the ledger (was 5,825, $6.0073).
- Mac load (1, 5, 15 min): 14, 14, 17 (was 89, 84, 75). 0 agent transcripts written in the last 10 minutes.
- Ambi ruled: Juju only; the old Loop and Milarepa threads are out (10:02 log). He ordered single-builder mode, no swarms (09:47 log).
- Lead stopped otto-chron-3 himself at 08:32. Line 2 was cut before "of the Roman empire", which made it false. It is back at Outline.
- Finished runs: strip-japan DONE 08:34 (60 s, 0.008751 US). Whole-film runs on disk: 4 DONE, 4 FAILED, 23 HOLD.
- Newest runs: proof12c FAILED 09:47 (stopped at Render and mix); proof12 HOLD 09:16; proof75b HOLD 09:06; proof75a HOLD 08:59 (Publish kit); strip-planets HOLD 08:41; strip-pluto HOLD 08:40.
- Juju commits on this Mac's main: newest 04788e9 (10:12), then cbbffcb (09:46). The builder reports the work is committed here but not on GitHub.
- Rooms drawn: 20 (was 19). Rust: 33,969 lines in 14 crates (was 32,716).
- Logged attempts: 241 kept, 35 reverted, 47 inconclusive.
- Finish check: still 2 of 23 clauses true.

## What worked and what failed
**Worked** (as reported; no one has judged any of it good)
- otto-chron-2: DONE, silent, Juju's own lines, -14.9 LUFS, 0.0019 US (lead, 08:32).
- strip-japan: DONE (facts, 08:34). No judgement of its look is reported.
- First voiced 75 s film, proof75a: voice bought, 0.015 US, 4.6 minutes machine time (builder, 09:00). It stopped at the thumbnail check (0.69 against a 0.68 limit).
- The builder's first 60 s of the new Ottoman strip, reviewed by a video model: verdict "fix". Worst fault: about 10 s with nothing new on Constantinople (builder, 10:12). Still stillness went from 6.2 s to 2.2 s (builder, 10:02).
- Script quote check: 148 sentences each matched to an exact quote in a source (builder, 09:46).
- Date and map position alone found the event for 23 of 26 beats (builder, 10:06).

**Failed**
- proof12 (voiced, 12 min requested): first draft 1,483 words, cut to 800 by Juju's own checks. Spent 0.46 US and 353 s on one attempt (read-only audit by Mungura, 09:28, from the job files).
- Mungura's comparison: VerseBatch wrote 10 scripts averaging 6,905 words in 55 minutes (10 Oct). Juju wrote 0 usable scripts. This is Mungura's reading, not judged by Ambi.
- proof75b: the renderer's laws refused it (builder, 09:06). proof12c FAILED at Render and mix (facts, 09:47).
- Ambi on a sound run, 08:44: interrupted before any fix landed. Three sound asks remain open.

## App engine and films
- **Ottoman Empire, 9.5 min, 26 events, voiced:** the builder says the full film was drawn and rendered. No run for it appears in FACTS. The builder has not watched it whole. The builder reports it ends in 1908. A longer script with an ending is being written (10:12).
- **Voice:** the builder moved from the cheap "flash" voice to the real TTS-2. Two samples await Ambi's choice. Delivery was called flat by the video model.
- **Limits:** the builder removed the 0.30 US voice gate. No ruling by Ambi is recorded. The builder also says a test clip no longer blocks a real film's thumbnail.
- **Story skills:** 52 skills exist. `juju make` does not link to them. The 10:02 diagnosis says no fix was applied. Crossroads Chain is not tested on a real film.
- **Render speed:** about 2.3 machine seconds per film second while the Mac was busy (builder, 10:12). Target 1.0 not met.
- **Picture:** the engine draws 12 of the 40 picture moves in the 60 reference films (study, 03:39). The builder is adding painting cutaways (10:12). Not in the film yet.
- **Harvest:** 11 of 12 films have notes. The rest is not reported.
- **Day log, undated:** a draw check found 3 wrong of 100 in two subjects. Rules fixed. Fresh draws 0 wrong (judged).

## Web app and rooms
- Pressed 24 Nov 01:22: 61 screens. Gate, Altar, Crossroads, Cauldron, Pact, Conjuring, Spell Strip and Publish Kit work on the main path. The five cards are placeholders. Mirror Bend and Feed Sight show broken or empty pictures.
- "Make a film" still makes practice clips (log, 08:44). A builder is wiring the film path into the 10, 20, 30 and 50 minute choices (09:43). Not reported done.
- An earlier worker's rooms in the film path never landed (10:01).
- Census (24 Nov 20:00): 573 controls; 112 real, 160 sample, 131 dead.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone.
- Phone job: an emulator run had 19 checks pass and 3 fail (lead, 24 Nov 23:14). Paused. Needs the Galaxy plugged in.
- Mac app: no release build reported. Not tested.

## Agents running now
- Live agent page did not answer. Running agents: unknown.
- Last reported, not confirmed live:
  - builder (10:12): three helpers, one per lane: app press-to-film path, a music bed, and painting cutaways. No film renders.
  - builder (10:15): auditioning space beds, then a `watch.py` fix.
  - a library test fails (lead, 08:37); no later report.
- Reviewers: all finished, last at 08:03.

## Money spent on services
- Ledger: $8.0822 over 6,029 calls. DeepSeek $2.1902, OpenRouter $4.3318, Google $0.834, Inworld $0.4198, WaveSpeed $0.171, unsettled $0.1355.
- Answered calls: DeepSeek 2,898 (13 refused); OpenRouter 2,949 (45); Google 14 (7); Inworld 87 (1); WaveSpeed 5 (0).
- Builder (10:12): 7.52 of 9.50 US spent. Lead: film lane 0.482 of 0.50 (08:32). Working limit 10.00 US (lead, earlier). The ledger is the record.

## Broken, blocked or open
- **GitHub billing blocks the merge** of seven pull requests (21 to 27 open). Nothing merged (lead, 08:16; no later report).
- **PR 26, sound:** the watcher reserves 0.000336 per call; main prices it at 0.001344; main refuses the call. Not reported fixed. Ambi said not to push to PR 26 (08:44).
- **PR 26** still holds two test frames pushed by mistake; they are Juju's own map film.
- **Two older tests fail** in files the builder has not touched (10:01).
- **Missing prices:** two models have no price in main; PRs 24 and 25 refuse their calls (07:49). Not rechecked.
- **Sound:** the 1.28 s hush rule on silent films awaits a ruling.
- **Vault:** LINE-RULE items 7 to 20 await countersign. No film made from a slot.
- **Pacing:** the Ottoman film is not watched whole. Its stillness and cutaway gaps are not yet measured after the cutaways.
- **Ending:** the Ottoman script stops at 1908; the longer ending is not written yet.
- **Not proven:** a voiced film over ten minutes; Crossroads Chain on any film; anything on a phone.

## Waiting on Ambi
1. **Fix GitHub billing** so the lead can merge the seven pull requests.
2. **Choose the voice:** say "Graham" or "Winston". Without an answer the builder uses Graham (10:03).
3. **Watch the first 100 seconds** of the Ottoman strip (10:01), then the full film when it is ready. Name the worst thing in it.
4. **Answer four questions** the builder put (scope, who writes, what may stop a film, pictures). Each has the builder's proposed "yes". No ruling by Ambi is recorded (Mungura, 09:28).
5. **Sound:** rule on the 1.28 s hush, and say whether the three sound fixes wait for the watcher fix.
6. **Plug in the Galaxy** for the phone job.
7. **Personal check-in:** a worker asked Ambi a personal question at 09:28 and 09:31. No reply is recorded.

## Counted by code

- Pull requests: 7 open, 19 merged, 1 closed
- Paid calls in the test ledger: 6029, $8.0822 in all {deepseek: 2.1902, openrouter: 4.3318, google: 0.834, inworld: 0.4198, unsettled: 0.1355, lead-test: 0.0, wavespeed: 0.171}
- Paid services answering: deepseek 2898 ok, 13 refused or failed, last ok 25 Nov 10:27 EAT; openrouter 2949 ok, 45 refused or failed, last ok 25 Nov 10:22 EAT; google 14 ok, 7 refused or failed, last ok 25 Nov 10:01 EAT; inworld 87 ok, 1 refused or failed, last ok 25 Nov 10:02 EAT; unsettled 0 ok, 7 refused or failed, last ok None; lead-test 0 ok, 3 refused or failed, last ok None; wavespeed 5 ok, 0 refused or failed, last ok 25 Nov 00:37 EAT
- Rust: 33,969 lines in 14 crates. Skills: 52. Rooms drawn: 20. Decisions: 19. APK files built: 0
- Design-system libraries on disk: camera_motion.json, fonts, house, kits, looks, palettes.json, proof, proto, work-camera_motion, work-palettes, work-quotes, work-surfaces_light, work-typography
- Finish check: 2 of 23 clauses true, so not done
- Whole-film runs of `juju make` on disk: 4 DONE, 4 FAILED, 23 HOLD
- Newest film runs: proof12c FAILED 25 Nov 09:47 (stopped at Render and mix); proof12 HOLD 25 Nov 09:16 (stopped at Script and heal); proof75b HOLD 25 Nov 09:06 (stopped at Render and mix); proof75a HOLD 25 Nov 08:59 (stopped at Publish kit); strip-planets HOLD 25 Nov 08:41 (stopped at Deal and package); strip-pluto HOLD 25 Nov 08:40 (stopped at Render and mix); 20261125-083722-131d HOLD 25 Nov 08:37 (stopped at Deal and package); strip-japan DONE 25 Nov 08:34 (60 s, 0.008751 US); strip-bulgaria HOLD 25 Nov 08:11 (stopped at Deal and package); strip-austria HOLD 25 Nov 08:11 (stopped at Deal and package); strip-manchuria HOLD 25 Nov 08:11 (stopped at Deal and package); thru-mughal HOLD 25 Nov 08:06 (stopped at Pictures and form)
- Agent transcripts written to in the last 10 minutes (all Claude work on this Mac, mostly Juju): 0
- Logged attempts: 241 kept, 35 reverted, 47 inconclusive
- Mac load (1, 5, 15 min): [14, 14, 17]
- The live agent page did not answer, so running agents are unknown
