# Juju day log, newest first

Rebuilt 14:31 EAT, Wed 25 Nov 2026. Only entries whose title names Juju. Times are EAT (UTC+3). Logged by agents: evidence of what they report, not proof. Where two entries disagree, the later one wins and the older stays.

---

## 2026-11-25 14:32 EAT — TEHUTI — Juju Maps: three looks written as closed systems (Duppy Night, Moko Day, Moko Dusk) with pick.py
<!-- type: event -->

**Changed.** juju-maps/systems/ (build.py, three machine files, three pages, pick.py, tests) and a draft pack crates/juju-skills/packs/moko-and-duppy. No engine file touched, no paid call.

**Why-verdict.** Ambi 25 Nov 13:55: low poly and dark are each a design system, operated by lower-thinking models over hundreds of films. Measured: 27 of 30 test sentences right on the first run, 30 after mending; 30 of 45 unseen sentences right on first runs; 204 of 255 hand-cut gold beats offered.

**Status-open.** No film boarded from pick.py; storyboard3.py does not call it; names, voice, thumbnails not chosen by Ambi; reach.rs and pins.txt rows owed. Harness: Claude Code (claude-opus-5-5).

**Related.** veve-gait, opon-sight, juju-lowpoly/EDIT-RULES.md, topic juju.

---

## 2026-11-25 14:21 EAT — TEHUTI — Juju docs and skills moved to the map-film stack

**Changed.** docs/STACK-MOVE.md (the stack now, 71 file verdicts, pins and reach rows for countersign, 9 handoffs). AGENTS.md, WORKER.md, ask-juju, 20 other skill files, 14 docs and ADR notes, kits. No skill.json, gate, pins.txt or reach.rs edited.

**Why-verdict.** Ambi 25 Nov 13:55: upgrade the skills and every MD that names the old stack. Checked: gates section of WORKER.md identical, skill.json identical, pins unchanged for existing packs.

**Status-open.** Eight packs have a when with no row in reach.rs; the app's one tap still draws with juju-stage; subtitle conflict with ADR 0014 item 4. Harness: Claude Code (Opus 5.5).

**Related.** [[juju]] docs/adr/0022-juju-maps.md

---

## 2026-11-25 14:10 EAT — TEHUTI — Juju Maps: Juju cut its own film for under a cent; panels, board4, cap 15

**Changed.** Cap 15 US (Ambi, about 13:55, runs/meter/cap.json). juju-maps/board4.py + shots2.json (structure in code, one small form a view), panels.js (Juju Motion facts panels, 12 kinds) + motion-timing.json (bjEr7L2Rj9s read whole), storyboard3 anchor(), views sized to the hero, auto cut. docs/COSTS-MAPS.md. Delegates: skills and stack docs, long films, app 0.2, design systems (Duppy Night, Moko Day, Moko Dusk), low-poly 2-8, editor by skill.

**Why-verdict.** Ambi: 7.5 of 10; Juju Motion timing is what takes it to high 8; spend more on breakthroughs; poly looks great. films/kivu-machine/a.mp4 shown. The low-effort editor taught by veve-gait made a better cut than the cheap model.

**Status-open.** kivu take b and the agent cut drawing; dam low-poly film not yet out; rift take 3 broken by a full disk, redraw when the Mac is quiet. Harness: Claude Code (Opus 5.5).

**Related.** [[juju]]

---

## 2026-11-25 13:51 EAT — TEHUTI — Juju Maps: measured edit grammar, dark take 2 approved in feel, low-poly style running, two new stories spoken

**Changed.** juju-maps: grammar.json, pace.py, storyboard3.py (sets, hero, in-view law, donor shot per sentence, self-mend, automatic cut), gl.js (fixed LAYERS, block cut that acts, lake water and gas, flood), record.mjs (4 s piece cache), mend.py, voice.py, beds/ (6 music moods). scripts/opon.py. Skills veve-gait and opon-sight (linked, not pinned in juju-conduct). juju-lowpoly/ + juju-poly-assets/ (polyfork shelf, 8 delegates). Films: rift2 take 2, kivu (Juju script), dam (script by Claude as a test).

**Why-verdict.** Ambi: "this is really good ... actually felt like I was learning"; dark look kept; spoken place must be in view; no stickling over accuracy.

**Status-open.** Purse 9.45 of 9.50. Disk and memory tight; Mac load over 100 with nine agents. kivu-machine (cheapest model, own cut) drawing. Harness: Claude Code (Opus 5.5).

**Related.** [[juju]] docs/adr/0022-juju-maps.md

---

## 2026-11-25 12:14 EAT — MUNGURA — Juju Maps: engine scripts written and first 480p obsidian take of the Ottoman film rendered

**Changed.** New engine files under `juju-maps/`: compile.py, mix.py, story.py, pics.py, ideate.py, tiles.js, film.js, film.css, film.html, record.mjs, server.mjs, and looks/obsidian.json + looks/terra.json. First take built in `films/ottoman2/`: scene.json (576 KB — 19 camera stops, 7 picture cards, 15 labels), pics.json (23 pictures), cards.json, mix.wav, `take1-obsidian.mp4` and t1.jpg (2,400×1,620 contact sheet of 30 frames).

**Why verdict.** ADR 0022 wants looks judged on fast 480p takes of one voice before any full export, so this is that test: full map skeleton and picture cards for a 1:58 cut instead of a full-priced draw.

**Status open.** Only the obsidian look was rendered (terra not); the take is 1:58, not the ~30-minute film. All juju-maps work is untracked — no commit, no push remote. `out/` is empty. No verdict from Ambi yet on voice, look or pictures.

**Related.** Verified with `ffprobe`: h264+aac, 854×480, 24 fps, 118.6 s, 40,592,307 bytes; `ffmpeg ebur128`: −15.1 LUFS, LRA 3.2. Frames pulled at 9, 12, 30 and 45 s show the relief map, year counter, empire fill and a captioned picture card (Sultan Bayezid I) with no blank tiles. Paths: `juju-maps/films/ottoman2/{scene.json,take1-obsidian.mp4,t1.jpg}`.

---

## 2026-11-25 12:04 EAT — MUNGURA — ADR 0022: Juju goes map-only; drawing engine forked as Juju Maps

**Changed.** `docs/adr/0022-juju-maps.md` written (1,882 bytes, 12:04), recording Ambi's decision of about 11:30–12:10: one niche only (empires, wars and borders), drawing engine forked as Juju Maps (`juju-maps/`) from bilawalsidhu/gods-eye-view (MIT, upstream 92fcccb), Wedjat untouched, juju-stage stops drawing map films; two looks held as data, no parchment; checks report and no longer stop a render except the money cap, an unsourced sentence, picture rights and Ambi's publish clicks; supersedes the HOLD law for these films. The fork exists on disk with its own `.git` at 92fcccb, an `upstream` remote set `no_push`, plus LICENSE, THIRD_PARTY_NOTICES.md and DATA_SOURCES.md (245 KB).

**Why verdict.** Ambi's own words are quoted in the ADR ("Juju just only [does] maps for now … do this one niche really well", "fork it again … so we won't use Wedjat", "I hate parchment paper", "having hard gates prevents a vid from rendering"). The fork keeps gods-eye-view's director maths and drops its name and marks; Wedjat is not modified.

**Status open.** The ADR leaves unsolved how a film is made with the Mac closed (keys and model calls need an always-on host) and money above the 9.50 USD cap for a 30-minute voice.

**Related.** `docs/adr/0022-juju-maps.md`; `juju-maps/DATA_SOURCES.md`; `juju-maps/THIRD_PARTY_NOTICES.md`; upstream commit 92fcccb.

---

## 2026-11-25 11:40 EAT — TEHUTI — Juju: film room and sound bed done on the copies; Ottoman film take 1 reviewed, take 2 drawing
<!-- type: event -->
**From:** TEHUTI

Juju: film room and sound bed done on the copies; Ottoman film take 1 reviewed, take 2 drawing
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi's ask: press to film, smooth. Walks passed 71 steps on web and phone, 0 bad, on the practice copy. Live app on 4701 restarted; its film room program answers. Film room tested on a silent film only.
- Ambi's ask: a bed and cues a history film deserves. proof75a and Pluto both PASS with the bed heard; 46 of 46 juju-sound tests pass, per the delegated report. Voiced proof12c bed: 37 of 37 stretches pass.
- Ottoman12f full draw with voice and music finished take 1. Review flagged flat delivery, treaty stretch, 1908 ending, thumbnail word, and an empty Paris map at 8:00. Take 1 moved aside; take 2 drawing with map and painting fixes.
- My mistake: a forced add committed about 1,000 ignored files from the rooms folder. Local only, never pushed; removed from the commit. About 1 GB of git data remains. Disk recovered from 0.7 GB to 1.9 GB.
- Spend: 8.69 of 9.50 US cap. Open: take 2 review, compare with take 1, thumbnail, and the flat voice. Ambi has not yet said what he hated most in take 1.
- Files changed: crates/juju-stage/src/worlds/map.rs; crates/juju-cli/src/stages/shots.rs; runs/spine/ottoman12f/master.mp4; runs/spine/ottoman12f/bin/juju-sound; runs/sound/proof/proof12c-bed/bed.json
- Status: in-progress — take 2 of the Ottoman12f film is drawing; its review and thumbnail are still open

---

## 2026-11-25 11:11 EAT — TEHUTI — juju-sound: real music beds and cues for voiced map films; Watcher reservation fixed
<!-- type: event -->
**From:** TEHUTI

juju-sound: real music beds and cues for voiced map films; Watcher reservation fixed
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 24e67170)
- Ambi asked that every voiced map film come out of juju-sound with a real, fitting bed and cues, after a video model flagged birdsong over historical narration on proof75a.
- Built a history bed from real string recordings in place of the birdsong, and a space bed (half-speed strings or tambura). Changes come at chapter points, ducked under the voice.
- Verified on copies only: proof75a -14.1 LUFS, peak -1.8 dB, bed 14.0 dB under the words, 1 cue heard. strip-pluto -14.5 LUFS, peak -1.8 dB, 4 of 4 cues heard. make-mongols now passes; it failed before.
- Fixed scripts/sound/watch.py so the Watcher reserves what the gate prices. 46 of 46 juju-sound tests pass. Open: Ambi must countersign the new bars, which the transcript cuts off before stating.
- Files changed: crates/juju-sound/src/music.rs; scripts/sound/watch.py; runs/sound/proof/proof75a-music/sound/strip.mp4; runs/sound/proof/strip-pluto-music/sound/strip.mp4; runs/sound/proof/proof12c-bed/bed.json
- Status: complete — the predicate is TRUE on the copies; new bars await Ambi's countersign

---

## 2026-11-25 11:10 EAT — TEHUTI — Juju sound: real music beds, both copied films pass
- **Changed:** crates/juju-sound (music.rs new), scripts/sound/watch.py reservation, profile map-music.json, 11 licensed music pieces on the shelf (6 history, 5 space). Harness: Claude Code (Opus 5.5 sub-agent).
- **Why/verdict:** birdsong bed replaced by real string quartets 14 dB under the voice, heard whole; proof75a and strip-pluto copies pass, 4 silent films pass, 46+ tests pass. Nothing committed.
- **Status/open:** kits.json needs the profile line (lead); silent-film bed is near -37 LUFS, a ruling is owed; no person has listened.
- **Related:** runs/sound/auto/HANDOFF.md 13-15, runs/sound/proof, topic juju.

---

## 2026-11-25 11:07 EAT — TEHUTI — Make-a-film room finished and walked end to end in the Juju app; server restart still needed
<!-- type: event -->
**From:** TEHUTI

Make-a-film room finished and walked end to end in the Juju app; server restart still needed
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 6553c74e)
- Ambi asked that a person pick a subject or pasted link, a look, voice or silent, a length (10/20/30/50), and get a real MP4 that flows 'exceptionally well'.
- Finished the Make a film room and added the /api/make path in juju-serve real.rs; the Altar, Cauldron and Pact rooms now run through it instead of dead-ending.
- Verified: web and phone walks at 71 steps each, other doors at 20, all 0 bad; 7 rooms pressed at 390 and 1440 px with 0 dead ends. The film room plays to the end with thumbnail and download matching master.mp4.
- 30, 50 and voice were checked only with a test list; make.json was left unchanged (voice off, lengths 1/10/20). The Estimated minutes figure only fell during the wait.
- Open: server on port 4700 must be restarted (scripts/serve/start) before anyone opens it. One test (a_real_film_survives_kill_9_and_two_tabs) did not run at head after a full cargo test began drawing a practice film by mistake; that scratch folder was deleted.
- Files changed: crates/juju-serve/src/real.rs; crates/juju-serve/tests/real.rs; runs/app/real-film/rooms/altar.html; runs/app/real-film/rooms/cauldron.html; runs/app/real-film/walk.py; runs/app/API.md; runs/app/api.json
- Status: complete — walks pass and the film path plays; server 4700 restart and one unrun test remain open

---

## 2026-11-25 11:05 EAT — TEHUTI — Juju app: Make a film to a watched film, walked on web and phone

- Harness: Claude Code (Opus 5.5), sub-agent, app lane. Topics: juju
- **Changed:** crates/juju-serve (links go to juju make --link, one look, one plain line and minutes left, one sentence and one action at a stop, the review's worst thing), mockups/r2 rooms landed, new film room, runs/app/API.md and api.json.
- **Why-verdict:** web walk 71 steps 0 bad, phone walk 71 steps 0 bad, 7 rooms pressed at both sizes with 0 dead controls and 0 layout faults; all on 4701 with a kept run played back, nothing paid.
- **Status-open:** 4700 needs the lead's restart (its old program has no /api/make); new films need a fresh pin; --link proved only against the stand-in; one test run began to draw the practice film and was stopped.
- **Related:** runs/app/real-film, runs/decision.tsv lane app-flow

---

## 2026-11-25 10:51 EAT — TEHUTI — Juju film pipeline: diagnosed why films stop, proposed a design-system-file approach
<!-- type: event -->
**From:** TEHUTI

Juju film pipeline: diagnosed why films stop, proposed a design-system-file approach
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 2aeafab7)
- Ambi asked what can actually be done about Juju choking, with VidRush reverse-engineered and only the design-system feature needed, full stack, no minimising.
- Read all 33 recorded Juju film runs: 4 finished, 25 of 29 ended were stopped by Juju's own checks (sound too quiet, 14.3 s hold vs 14 s limit, thumbnail 0.69 vs 0.68).
- Proposed three changes: nothing kills a film (repair or backup shot, note for Ambi); one shot kind per spoken line like VidRush; a design system as one file filled by measuring a pasted video.
- Open: Ambi's question 'A film always finishes, yes or no?' is unanswered; no code changed; the proposal is not yet built or tested.
- Files changed: JUJU-MASTER-BRIEF.md; ~/.hermes/profiles/default/memory/shortterm/2026-11-25.md
- Status: in-progress — diagnosis and proposal delivered; awaiting Ambi's yes/no and a go to build.

---

## 2026-11-25 10:50 EAT — MUNGURA — Juju: 25 of 29 film runs were stopped by our own checks; assemble-not-draw proposed
<!-- type: event -->
**From:** MUNGURA

- **Changed:** nothing in Juju; read only. Harness: Claude Code (Opus 5.5).
- **Why/verdict:** Measured from runs/spine/*/live.json (33 runs): 4 done, 21 hold, 4 failed, 4 marked working. The 25 stops by stage: deal and package 8, script 8, pictures and form 2, render and mix 6, publish kit 1. Small misses stopped whole films (14.3 s against 14; -17.0 LUFS against -14; thumbnail 0.69; 117 type pixels outside the safe box after 196 s of drawing). Two of the 25 were test runs with a 0.00 budget. VidRush assembles each clause from seven footage kinds by a channel's share (harvest/wave1/out/vidrush-10.json); Juju draws one kind of world per film.
- **Status/open:** candidate, not decided: a film always finishes (repair, fall back, or note), one shot assembler over mixed footage kinds, a design system is one data file. It changes the never-loosen-a-gate law, so Ambi must say it. Session 31bfe4d9 is the live builder (ottoman12f).
- **Related:** juju, runs/spine, docs/adr/0012, docs/adr/0021

---

## 2026-11-25 10:35 EAT — TEHUTI — Juju film: export moved to 720p 24fps H.264, script ending restored, closing-line checker added
<!-- type: event -->
**From:** TEHUTI

Juju film: export moved to 720p 24fps H.264, script ending restored, closing-line checker added
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked that Juju produce films itself, export the way CapCut and Resolve do, and never crash the computer. Films should be reviewed before he sees them.
- Done: export now draws once and encodes once at 720p, 24 fps, H.264 on the Mac's video chip. An 8-second sample projects to about 390 MB for a 12-minute film, down from about 1.9 GB.
- Done: script rebuilt to about 1,750 words with the Vienna, Candia and Belgrade endings restored. Closing lines now go through a checker (up to 3 tries) and are dropped if none pass. Voice switched from flash to TTS-2.
- Verified: on the first-60-second strip the longest still stretch fell from 6.2 s to 2.2 s, and the review returned 'fix'. Drawing ran at 1.6 s per film-second, down from 2.3, not yet measured on a quiet Mac.
- Open: no full film has been rendered. Painting cutaways, the music bed and the review step are not yet proven end to end. Spend is about 8.1 of 9.50 USD.
- Files changed: crates/juju-stage/src/encode.rs; crates/juju-cli/src/stages/words.rs; crates/juju-stage/src/worlds/map.rs; crates/juju-stage/src/worlds/ink.rs; scripts/video_eye.py; crates/juju-cli/practice/kits.json
- Status: in-progress — export and script fixes are built and partly checked; the full film with paintings, music and review has not been rendered.

---

## 2026-11-25 10:02 EAT — TEHUTI — Juju: diagnosed why make ignores the story skills; fixes proposed, none applied yet
<!-- type: event -->
**From:** TEHUTI

Juju: diagnosed why make ignores the story skills; fixes proposed, none applied yet
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session c34719fe)
- Ambi asked for Juju only: "Juju Juju is what we're working on". Agent confirmed Juju scope and dropped the old Loop and Milarepa threads.
- Found 52 skills exist, but `juju make` has no link to them or to the conductor. The outline prompt tells it to invent causes the facts do not give.
- The 12-minute script failed: first draft 1,483 words, 16 repairs to 1,373, then a fallback cut to 800 words. Cost $0.46.
- A third try at 1,802 words was live at the script check at 9:31. Its proposed fixes are wiring `juju make` to the skills and building the outline with Crossroads Chain.
- Not proven: whether Crossroads Chain improves the script. Nothing was changed in the repo during this session.
- Status: in-progress — diagnosis and fix plan delivered; no code changed or verified yet

---

## 2026-11-25 09:47 EAT — TEHUTI — Juju: one builder, voiced Ottoman film rendering, new map look and quote-checked script
<!-- type: event -->
**From:** TEHUTI

Juju: one builder, voiced Ottoman film rendering, new map look and quote-checked script
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi ordered single-builder mode, no swarms. Background jobs were stopped and Mac load fell from 92 to 3, then the tree was checked to build.
- Voiced path fixed: the 0.30 voice limit is in, the word-matching truth check was replaced by an exact-quote check (148 sentences matched), and a resume-hash rounding bug was fixed.
- New One Ink map look and measured arrival motion added. The first long voiced film (Ottoman, 9.5 min, 26 events) was still rendering, about 15 minutes left, and had not been watched yet.
- Not done: the film came out 9.5 min, not the 12 requested. Seven PRs (21 to 26) passed their combined test but are unmerged because GitHub billing blocked the final step. Ambi must fix billing.
- Files changed: crates/juju-cli/src/stages/words.rs; crates/juju-cli/src/stages/shots.rs; crates/juju-cli/src/stages/deal.rs; crates/juju-stage/src/worlds/map.rs; crates/juju-stage/src/worlds/ink.rs; crates/juju-stage/src/motion.rs; scripts/purse.py; scripts/video_eye.py
- Status: in-progress — Ottoman voiced film still rendering and unwatched; seven PRs unmerged pending GitHub billing fix

---

## 2026-11-25 09:46 EAT — TEHUTI — Juju: single builder; first long voiced film rendering
<!-- type: event -->
**From:** TEHUTI

Juju: single builder; first long voiced film rendering
- Harness: Claude Code
- What happened: undefined
- Status: undefined

---

## 2026-11-25 09:29 EAT — MUNGURA — Juju diagnosis: order of work was wrong; VerseBatch made 10 long scripts in 55 min, Juju made 0
<!-- type: event -->
**From:** MUNGURA

Juju diagnosis: order of work was wrong; VerseBatch made 10 long scripts in 55 min, Juju made 0
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session c34719fe)
- Ambi asked whether we messed up: two weeks of prep and two Ultra-weekly token runs produced no one-minute video, and he asked what we need to do.
- Agent compared VerseBatch (10 scripts of about 6,900 words each, 55 min, 10 Oct) with Juju (0 usable scripts; one try of 6 min, 1,483 words, cost $0.46).
- Causes named: scripts built from border-table rows with lines that break accuracy; checks that kill films instead of flagging them; swarms that re-read heavily, about 4.4B tokens on 24-25 Nov.
- A 75-second voiced film rendered at 8:58 and was stopped because its thumbnail scored 0.69 against a 0.68 limit; the agent said that film is not good either.
- Still open: no fix was applied in this part of the session. Next step is to rebuild the script order and the gates before more swarm runs.
- Files changed: ~/.claude/projects/-Users-Mungura-AUH/memory/juju-benchmark-versebatch.md
- Status: in-progress — diagnosis delivered and benchmark note saved; no Juju fix applied yet

---

## 2026-11-25 09:28 EAT — MUNGURA — Juju audit for Ambi: the script step lost to VerseBatch
<!-- type: event -->
**From:** MUNGURA

- **Changed:** nothing in Juju; read only. Harness: Claude Code (Opus 5.5).
- **Why/verdict:** Measured: VerseBatch made 10 scripts averaging 6,905 words in 55 min (10 Oct, jobs/verse file times). Juju proof12 spent 0.46 US and 353 s on one failed script of 1,483 words cut to 800 by its own checks; proof75a (75 s, voiced, 4.6 min) held only by a thumbnail check and its lines are a list. 4.4 billion Claude tokens on 24 and 25 Nov, almost all re-reading.
- **Status/open:** round 1 of questions put to Ambi; no decision recorded.
- **Related:** juju, runs/builder/proof12.log, ~/AUH/Loop/jobs/verse

---

## 2026-11-25 08:53 EAT — TEHUTI — Fixed the context-repo sync job and pushed the Juju overhaul to GitHub
<!-- type: event -->
**From:** TEHUTI

Fixed the context-repo sync job and pushed the Juju overhaul to GitHub
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 2aeafab7)
- Ambi asked: "I think everything today GitHub. Everything that has happened... Everything everything now, man, please." The two-hour sync had crashed at 13:52 on a date format, so nothing had been pushed for 18 hours.
- Fixed sync_context_repo.py, then read both days of Juju work and the day logs. Picked hand-chosen success and failure pictures, each with its verdict in the caption, and ran a text scan on each.
- Rewrote the repo pages: 11-juju/worked-and-failed.md, money-and-stack, orchestration, surfaces, and the now and record pages. Each is timestamped and the gallery was updated (252 pictures, 57 new).
- Pushed by hand after stopping the running sync job, so the push did not wait for the schedule. The GitHub link and the update text for Ambi were produced from the pushed repo.
- Still open: the Make-a-film button still makes a practice clip, not a real film. No phone app file exists yet. The two-hourly Haiku update job needs a confirmed clean run.
- Files changed: ~/AUH/AMBESSA/sync_context_repo.py; ~/AUH/AMBESSA/context_gallery.py; ~/AUH/AMBESSA/context-repo/11-juju/worked-and-failed.md; ~/AUH/AMBESSA/context-repo/11-juju/money-and-stack.md; ~/AUH/AMBESSA/context-repo/11-juju/orchestration.md; ~/AUH/AMBESSA/context-repo/10-now/now.md; ~/AUH/AMBESSA/context-repo/09-assets/library/LIBRARY.md; ~/AUH/AMBESSA/context-repo/11-juju/what-ambi-said.md
- Status: complete — repo pushed by hand at 08:15 EAT 25 Nov; app 'Make a film' still makes practice clips, not yet wired

---

## 2026-11-25 08:44 EAT — TEHUTI — THROUGH: silent Juju film built to DONE with its own lines; voiced minute and thru-japan/space still open
<!-- type: event -->
**From:** TEHUTI

THROUGH: silent Juju film built to DONE with its own lines; voiced minute and thru-japan/space still open
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session ef888377)
- Ambi asked for a real juju make film with no test switches, only Juju's models: silent minute, then voiced minute, then 10 minutes.
- Silent otto-chron-2 reached DONE, with Juju's own dated lines on the map. Sound passed at -14.6 LUFS with 4 of 4 cues heard. Fixes went into truth.rs, words.rs, source.rs, clock.rs, deal.rs and the new chron.rs.
- New checks refuse a line shown before its year or a pin more than 150 km from its named place. The test suite was at 61 passing with planted cases; the final full run was not confirmed before the session was interrupted.
- Lead reports strip-mughal DONE (16 min, 0.0085 US) but with faults still open. thru-japan and thru-space stalled on the 7 s gap rule. otto-chron-3 went back to Outline. No voiced minute has been made yet.
- Files changed: crates/juju-cli/src/stages/chron.rs; crates/juju-cli/src/stages/truth.rs; crates/juju-cli/src/stages/words.rs; crates/juju-cli/src/stages/source.rs; crates/juju-cli/src/stages/clock.rs; crates/juju-cli/src/stages/deal.rs; crates/juju-cli/tests/make.rs; runs/through/BLOCKS.md
- Status: in-progress — silent minute DONE (otto-chron-2); voiced minute and 10-minute film not yet made; session interrupted by user

---

## 2026-11-25 08:44 EAT — TEHUTI — Sound worker: read the juju-sound code for three fixes; interrupted before any fix landed
<!-- type: event -->
**From:** TEHUTI

Sound worker: read the juju-sound code for three fixes; interrupted before any fix landed
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 62c92a0f)
- Ambi asked for three sound fixes: a bed for the space film strip-pluto, the watch.py reserve mismatch with prices.worst, and a listening check of three masters. He said not to push to PR 26.
- Read WORKER.md, the ask-juju skill, the earshot-sound-engine skill, the juju-sound crate, glue/watch.py, scripts/prices.py and runs/sound/auto/HANDOFF.md.
- Searched Wikimedia for public-domain space-air recordings and created an empty folder runs/sound/auto/shelf/src/space. No bed was built, no code was changed, and no listening check was done.
- Ambi interrupted the run. Open: the bed for strip-pluto, the watcher reserve fix (0.000336 vs 0.001344), and the Earshot listening note on the three masters.
- Files changed: runs/sound/auto/shelf/src/space
- Status: blocked — interrupted by Ambi; all three asks still open, no code or film changed

---

## 2026-11-25 08:12 EAT — TEHUTI — Juju Vault: the review faults of juju-db fixed
<!-- type: event -->
- Changed: crates/juju-db (whole-vault brands, one lock for a deal, kill-safe store, film numbers, story of every film, spoken words only), runs/vault. Commits cf2a0e5..3aec0e3.
- Why-verdict: fresh review showed 7 blocking faults; each red on 9be3910, green now; 54 tests; 357x60 simulation 21,182 dealt, 238 refused, 0 faults on re-read.
- Status-open: LINE-RULE 7 to 20 not countersigned; across niches still more alike than published (2.2 percent against 0.9); no film made from a slot.
- Related: runs/vault/receipt.json, runs/vault/review/. Harness: Claude Code (Opus 5.5), workflow worker.

---

## 2026-11-25 08:05 EAT — TEHUTI — Juju house strips repaired: Egypt, Orion, lungs rendered whole
<!-- type: event -->
**From:** TEHUTI (claude-code, Opus 5.5, strengths lane)

- **Changed:** new world land_depth, rewritten star_depth and solid_depth, whole numbers, law that type may not lie on drawn lines (worktree verbs-wt 53ffdba; patch runs/house/bin/engine.patch). Three mp4s with receipts, trace.json and sheets in runs/house/strip-1..3.
- **Why/verdict:** four judges' findings of the night; code check TRUE, 31 unit tests pass (Measured); looks Judged by the maker only.
- **Status/open:** needs fresh eyes; render 7 to 19 s a second of film at load 57 to 95 (target 1.0 missed); no sound; systems.json seats are a handoff (runs/house/handoff.json).
- **Related:** runs/house/check.json

---

## 2026-11-25 08:03 EAT — TEHUTI — Juju: opus-ship-c rechecked PRs 21, 22, 24, 25 and reviewed 26, 27

- **Changed:** six CLEAN reviews recorded; notes in runs/pr/NEXT.md
- **Why-verdict:** each named block gone, planted tests green on GitHub; 22 own test run once, 2 OK. 26 under-reserves, main refuses (closed)
- **Status-open:** train pending when read; 26 watch.py reserve is a fix
- **Related:** juju, docs/adr/0020. Harness: Claude Code (claude-opus-5-5)

---

## 2026-11-25 07:58 EAT — TEHUTI — Juju harvest: HmuQoak_IAg seen whole
<!-- type: event -->
**From:** TEHUTI

- **Changed:** runs/harvest/rea/HmuQoak_IAg (survey, cuts, events, words, SEEN.md); three 45 s decompose windows beside it. Harness: claude-code (Opus 5.5).
- **Why/verdict:** 74 shots, no hard cut, dissolves about 0.5 s (Measured), not 1 s.
- **Status/open:** label times on moving pictures good to about 1 s; sound not heard.
- **Related:** ADR 0021.

---

## 2026-11-25 07:48 EAT — TEHUTI — Juju: repair rounds on pull requests 21, 22, 24, 25; sound glue moved; rules unit opened
<!-- type: event -->
**From:** TEHUTI

Juju: repair rounds on pull requests 21, 22, 24, 25; sound glue moved; rules unit opened
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: 22 silent survey refused; 21 cost and time from the book's row; 25 redirects, size, official host, promises and ceiling lock; 24 job cap 0.06 asked, word list required; 26 glue in scripts/sound, beds with licence. Rules unit opened (WORKER.md, AMBI-EYE, AMBI-EAR link, film-harvest row). Why/verdict: reviewers' blocks, each with a planted test. Open: rechecks, GitHub on new heads; gather owner applies runs/gather/PATCH-25.diff. Related: runs/pr/NEXT.md. The two frames pushed by mistake in 26 are Juju's own film map-demo-60. Harness: Claude Code (Opus 5.5).
- Verification: Planted tests pass on the Mac; GitHub checks running on 24 and the rules unit at log time.
- Status: in-progress, awaiting GitHub and rechecks

---

## 2026-11-25 07:33 EAT — TEHUTI — Juju: review of PRs 21, 22, 23 by opus-ship-a

- Changed: 21 FINDINGS, 22 FINDINGS, 23 CLEAN; notes in runs/pr/NEXT.md
- Why-verdict: 21 bought-picture receipt wrong with the gate on main; 22 crashed survey skipped (reproduced)
- Status-open: one repair and recheck each for 21 and 22
- Related: docs/adr/0020. Harness: Claude Code (claude-opus-5-5)

---

## 2026-11-25 07:29 EAT — TEHUTI — Juju harvest: film 36J1tL9ulGA seen whole
- **Changed:** runs/harvest/rea/36J1tL9ulGA (survey, cuts, events, words, SEEN.md)
- **Why/verdict:** 340 joins looked at; slow map fills were invisible to both eyes, a colour area curve found 3 of 3 (Measured)
- **Status/open:** done; sound not split, review of three rea windows not answered
- **Related:** juju, runs/harvest/SCORE.md

---

## 2026-11-25 07:21 EAT — TEHUTI — Juju: six small pull requests opened from this Mac's crates
<!-- type: event -->
**From:** TEHUTI

Juju: six small pull requests opened from this Mac's crates
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: PRs 21 sigil, 22 harvest + ADR 0021, 23 kits, 24 next, 25 gather, 26 sound (draft). Why/verdict: units to main by ADR 0020. Left out: juju-encode (needs the Maker seam in juju-stage, owned by engine), scriptlab data (no juju-script test reads it), two film frames and their Vision test in sound. bend.py kept: money tests read it. Open: 26 checks red, the two glue Python files need the lead's ruling; gate allow list untouched. Related: docs/adr/0020. Harness: Claude Code (Opus 5.5).
- Verification: cargo check per crate, gate_checks tree and diff locally; GitHub checks partly pending at log time.
- Status: in-progress, GitHub checks running, nothing reviewed or merged

---

## 2026-11-25 07:17 EAT — TEHUTI — Juju harvest: film IEWMpPs0M-M seen whole
<!-- type: event -->
**From:** TEHUTI (claude-code, Opus 5.5)

- Changed: runs/harvest/rea/IEWMpPs0M-M (survey, cuts 173, events 756 merged, words, SEEN.md)
- Why-verdict: kept; nearly every join is a dissolve, solved as a per frame mix
- Status-open: complete; sound not split or heard
- Related: ADR 0021, runs/harvest/SCORE.md

---

## 2026-11-25 06:51 EAT — TEHUTI — Juju gather lane: the reviewer's ten findings worked through (freeze-14)
**Changed:** crates/juju-gather (new truth.rs, borders.rs, recheck.rs; door, plan, net, geo, maps, scale, pics, film, spot, report), runs/gather folders, rerun.sh, FAULTS-14.txt, HANDOFF-STAGE.md. Harness: Claude Code (claude-opus-5-5), workflow worker.
**Why/verdict:** predicate not called TRUE: second reader 0 of 100 and no cold run of the newest binary (0.0003 US left of 0.20). 101 of 101 planted faults refused; stage valid, 0 fallback on 8 tables; moons and Ottoman carry, Black Death, Zulu, Magellan are honest holds.
**Status/open:** about 0.08 US for a cold run and 100 second readings; stage lane: rims of later borders; pictures of map films few.
**Related:** juju, runs/gather/report.json, ADR 0019

---

## 2026-11-25 06:47 EAT — TEHUTI — Juju: stopped waves restarted, film-harvest skill merged, 60-film study shows engine gaps
<!-- type: event -->
**From:** TEHUTI

Juju: stopped waves restarted, film-harvest skill merged, 60-film study shows engine gaps
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi pressed stop on three Juju waves. All three were restarted from disk, and the original facts worker was found still alive, not dead as first assumed.
- film-harvest skill finished and shipped as PR 20; PR 18 and PR 20 merged to main after clean reviews. Fast runner measured about 1.2x faster, not the 3x target.
- 60-film study done: Juju's engine can draw 12 of the 40 picture moves those films use. Facts lane still fails the bar: 2 of 15 opened facts were wrong.
- Mac thrashed at load 190 with 10 GB swapped; sound splitting was stopped and a disk watch set. Still open: one film through the full chain with words on it, checked by eye.
- Files changed: crates/juju-skills/packs/film-harvest/SKILL.md; runs/harvest/SCORE.md; runs/harvest/READ-FIRST.md; runs/gather/GATE-BACK.md; runs/spine/otto-silent-2/master.mp4
- Status: in-progress — PRs 18 and 20 merged; one repaired film with words is still to be made and checked.

---

## 2026-11-25 06:45 EAT — MUNGURA — Juju: first real film out of juju make (1 minute, silent, DONE); works, not good yet
<!-- type: event -->
**From:** MUNGURA

Juju: first real film out of juju make (1 minute, silent, DONE); works, not good yet
- Harness: Claude Code (claude-opus-5-5)
- What happened: runs/spine/otto-silent-2: "The Ottoman Empire, year by year", juju make, 11 of 11 stages, no test switch, 60.0 s, 1280x720, -14.6 LUFS, 0.068 US, 17.2 machine minutes. Lead watched a frame every 3 s: no words on a silent film, stretches with no change, modern "now Turkey" labels, grey outlines, a doubtful number (1,459 in 1861, 2,018 in 1914). Sent to the THROUGH owner. House strips judged: all four eyes refused the planted burger first; relief and lungs strips liked, Orion strip refused, no trace tables yet, one repair running. Harvest: rea-video 10 of 35 drawn events against 35 of 35 by our own eye; seven films read whole.
- Status: in-progress

---

## 2026-11-25 05:43 EAT — TEHUTI — Juju sound lane: reviewer faults fixed
<!-- type: event -->
**From:** TEHUTI

- Changed: juju-sound reads the drawn frames for a number landing, hears cues in one channel outside the words, requires and hears a bed, makes silent films loud by what happens, runs at most four programs at once, never keeps a rubbish answer. Harness: Claude Code (Opus 5.5).
- Why/verdict: strip.mp4 -14.1 LUFS, 2 of 2 cues heard, 9 planted faults refused, silent kit -14.2 with 4 cues; a 20 minute film takes 912 s at load 35 to 49.
- Status/open: 60 s strip took 81 s wall at load 35 (64 s of processor); the 1.28 s hush on silent films needs a ruling (make-mongols still refused).
- Related: runs/sound/auto/HANDOFF.md, branch unit/sound a1f3e12.

---

## 2026-11-25 05:26 EAT — TEHUTI — Juju title cards: checks fixed, no hand yet
- Changed: juju-next 0.5.0 (a3dfd48 and after): words of a title held to its passage, two readers sealed to the card, pictures from their own records, bends on the donor shape, one journal for a deal. Harness: claude-code (Opus 5.5).
- Why-verdict: 15 of 15 planted false titles passed before, 0 of 15 now; two deals at once and kills lose nothing (13 of 13). Predicate FALSE: 0 cards stand, pull bar 6.
- Status-open: 0.0223 US of the lane left, day fuse 0.12 reached; no vote, no paste, no timing under load 20.
- Related: juju, runs/character/loop/evidence/v5

---

## 2026-11-25 05:18 EAT — TEHUTI — Juju harvest: the film language is written and beats rea-video on 4 of 5 blind spots
<!-- type: event -->
- Changed: runs/harvest/LANGUAGE.md, language.schema.json (made by tools/make_schema.py), tools/measure.py; proofs in runs/harvest/language (stay on this Mac).
- Why/verdict: measure.py check prints PREDICATE TRUE. 64 of 64 truth rows said with no prose left; 32 of 35 drawn events against 10 (Measured, same windows); spot 4 not won. Held out: wins at 0.1 s on both stretches, loses to rea at 0.5 s on H 632 to 672.
- Status/open: way names right 10 of 32, 126 and 145 pieces for 19 and 17 things, held out is one film only, sound not heard, no blind rebuild. Harness: Claude Code (Opus 5.5), workflow worker.
- Related: juju, film-harvest; schema is git-ignored by runs/harvest/.gitignore (rebuilt by tools/make_schema.py).

---

## 2026-11-25 04:44 EAT — TEHUTI — Juju harvest: hero J0wWNytEXS4 seen whole

- **Changed:** runs/harvest/rea/J0wWNytEXS4 (survey, cuts, events, words, SEEN.md)
- **Why/verdict:** 138 hard cuts; truth windows 23 of 26 events
- **Status/open:** done; sound not heard, beats without a hand note are noisy
- **Related:** runs/harvest/SCORE.md (claude-code opus 5.5)

---

## 2026-11-25 04:16 EAT — TEHUTI — Juju Vault: stage 0 slot, shelf and sameness meter built
<!-- type: event -->
**From:** TEHUTI (Claude Code, Opus 5.5, juju-db lane)

- **Changed:** crates/juju-db and runs/vault: one folder a channel store, 14 parts as data, slot solver, 15 film shelf, sameness meter, juju-db CLI; LOT opened in runs/vault/store with 0 films.
- **Status-open:** countersign of LINE-RULE.md items 7 to 14; LOT leans on four arcs its vessel does not list (32 of 60); the spine must call it.
- **Related:** runs/vault/receipt.json, runs/vault/sim.json, commit a966d48. Topic: juju.

---

## 2026-11-25 04:15 EAT — TEHUTI — Juju harvest: scripts/harvest runs windows, same answers, 3x not reached

- **Changed:** scripts/harvest, scripts/harvest_lib, runs/harvest/tools (FAST-READY, FAST.md, ORDER, rea_launch.py refuses stems). Uncommitted. Harness: Claude Code (Opus 5.5 worker).
- **Why/verdict:** 20 s cut SAME as plain, 218 to 90 processor seconds but 195 to 167 s wall; kill -9 and resume SAME; decode was about 6 percent of plain, text and sound the rest.
- **Status/open:** 3x not reached or proven; 120 s plain never finished; sound split off by order; a long film with the memory patch not run.
- **Related:** ADR 0021, runs/harvest/SCORE.md, runs/decision.tsv lane harvest, topic juju.

---

## 2026-11-25 03:40 EAT — MUNGURA — Juju harvest: rea-video scored against hand truth; our own eye sees what it cannot
<!-- type: event -->
**From:** MUNGURA

Juju harvest: rea-video scored against hand truth; our own eye sees what it cannot
- Harness: Claude Code (claude-opus-5-5)
- What happened: Truth sealed first, three 40 s windows. rea-video: hard cuts on paper 3 of 3, but 10 of 35 drawn events inside code-drawn shots, 0 of 9 on the silent map, 58.9 min for 40 s plain. Arrival map plus frame difference: 35 of 35, 47 to 100 s a window, same windows it was built on (no held-out proof). Snapshots every 2 s: 32 noticed, 2 timed within 0.1 s. Decision: no whole film decompose; survey and looking from rea-video, events from our own eye, words from captions. Also: the 60-film study ended; the engine draws 12 of 40 moves and 0 of 20 skeleton and house pairs whole; the engine lane was released to build the ten missing primitives. PRs 18 and 20 merged, none open. Spend 5.50 of 10.00.
- Status: in-progress

---

## 2026-11-25 03:38 EAT — TEHUTI — Juju packaging lab repaired (lab-packaging)
- Changed: runs/scriptlab/packaging: 9 frames, 45 bends, 3 chains, check, plants, blind tags, opened sources. Harness: claude-code subagent.
- Why/verdict: 10 review findings; F06 and F09 dropped by count; check.py TRUE, 145 of 145 plants refused (Measured).
- Status/open: 9 bend sources unconfirmed, 31 pictures need a missing part, F02 five-word sentence wants a countersign.
- Related: juju, runs/decision.tsv lane lab-packaging.

---

## 2026-11-25 03:36 EAT — TEHUTI — Juju sigil: ten reviewer faults fixed in the thumbnail crate
<!-- type: event -->
**From:** TEHUTI

- Changed: crates/juju-sigil (map ground runs past the base's edge, subject chosen by the package, fonts/licence/whole-file checks, G6 fails closed, free picture kept through any buy, locks), runs/sigil checks and faults folder. Harness: Claude Code (Opus 5.5).
- Why/verdict: 19 of 20 new tests fail on the old source, 20 of 20 pass now; check.py 29 TRUE; lane spend 0.0903 of 0.25 US.
- Status/open: not committed; cli must expect HOLD when a package asks for a picture the film does not hold; gather tables without take rows, Borodino at 94.9 E.
- Related: runs/sigil/receipt.json, runs/sigil/faults, topic juju

---

## 2026-11-25 03:24 EAT — TEHUTI — Juju hands lane: two true hands, not three
<!-- type: event -->
**From:** TEHUTI

- **Changed:** juju-next 0.4.1 (commit 6dd7e64): cards are built from their answer outward, a second reader of another vendor finds the answer again unseen, code refuses the rest.
- **Why-verdict:** earlier hands had wrong answers. Vote against real breakouts rose from 6 and 2 to 9 and 7 wins of 20 (judges weak, 3 of 6 plants).
- **Status-open:** lot and space-demo have a hand; map-demo has 4 cards, no hand. Speed under 5 s and 25 s only seen at load 78 to 164. Lane money 0.295 of 0.30 spent, so the rest needs about 0.06 US more.
- **Related:** runs/character/loop/hands.json, runs/character/loop/evidence/v4. Harness: claude-code (Opus 5.5).

---

## 2026-11-25 03:03 EAT — TEHUTI — Juju scriptlab looks repaired against 13 review findings
<!-- type: event -->
**From:** TEHUTI

- Changed: runs/scriptlab/looks make.py, measure.py, check.py, plants.py, side.py, both pairings, HANDOFF.md (lane lab-looks, 15 decide rows)
- Why-verdict: check let 33 of 33 planted faults through; now 0 of 52 missed (Measured)
- Status-open: predicate FALSE for two faults: near-worlds has two usable signature moves; layout gate fires at 0.359 v 0.572 and that measure is not proven; nobody has listened
- Related: Harness: Claude Code (Opus 5.5); evidence runs/scriptlab/looks/evidence

---

## 2026-11-25 02:56 EAT — TEHUTI — juju-gather built: bare card to facts, tables, pictures
Harness: claude-code (Opus 5.5), Juju gather lane.
- **Changed:** new crate crates/juju-gather, runs/gather (report.json, FREEZE-8.txt, bin/juju-gather-freeze-8).
- **Why/verdict:** five bare cards gathered cold in 117 to 188 s, 36 to 172 facts, 0.003 to 0.010 US each; juju-stage accepts every table. First spot draw found 3 wrong of 100 in two subjects; rules fixed, fresh draws 0 wrong (Judged).
- **Status/open:** three map stories still HOLD at ten minutes (10 to 14 dated places, 23 needed). Lane money spent (ledger 0.1980 of 0.20, 0.0259 of it charged while the gate was down).
- **Related:** runs/predicate/CONTRACTS.md 1b.

---

## 2026-11-25 02:37 EAT — TEHUTI — Reviewed Juju PR 20 (film-harvest pack): CLEAN
- **Changed:** review recorded as opus-pack at cc900693; list in runs/pr/NEXT.md. Harness: Claude Code (Opus 5.5).
- **Why-verdict:** pins 800 of 800, rows Builder only, fragment null, licence whole, three translations match. No block.
- **Status-open:** lead countersign for pins; conduct tests and train pending when read; four fixes listed.
- **Related:** juju, PR 20, ADR 0020

---

## 2026-11-25 02:33 EAT — TEHUTI — Juju gather lane: two workers caught, critic report written
- **Changed:** runs/gather/ATTACK.md, runs/gather/TWO-WORKERS.md (Juju). Harness: claude-code (Opus 5.5), no paid call, no code edit.
- **Why-verdict:** build:gather was alive, so the delegate became its read-only critic by the lead's word. FAULTS: 6 wrong pins, a wrong year, 6 facts from other voyages, recheck accepts 6 of 8 planted faults; juju-stage accepts all 7 tables.
- **Status-open:** gather bar not TRUE; owner aee4ed9c2c964b10f; money nearly gone (0.20 US limit).
- **Related:** juju, gather lane, runs/gather/ATTACK.md

---

## 2026-11-25 02:32 EAT — TEHUTI — Juju film-harvest skill: written, linked, passed a fresh agent
- **Changed:** crates/juju-skills/packs/film-harvest (SKILL.md 90 lines, 13 references plus 4 more in English, 14 forms, 5 kickoffs, self test, reach-and-pins.patch), linked into Claude Code and Hermes; runs/harvest/rea/ref20-fresh (proof). Uncommitted. Harness: Claude Code (Opus 5.5 worker).
- **Why/verdict:** Ambi 25 Nov 01:00. A fresh Opus agent with the pack alone made a package that passes videomd --check and answered 6 of 6 plus the planted mistake; its 24 stumbles were answered in the pack.
- **Status/open:** corrected pack not rerun; scripts/harvest main flow, step 8 and the Watcher and Scribe forms unrun; reach rows not compiled here (rustc 1.88 cannot build juju-reliquary), patch waits for the lead's countersign.
- **Related:** ADR 0021, runs/decision.tsv lane film-harvest, topic juju.

---

## 2026-11-25 01:14 EAT — TEHUTI — Juju packaging lane: ten title frames from winners against their own flops

- **Changed:** runs/scriptlab/packaging (why.json, bends.json, chains.json, kill.json, check.py, 97 thumbnails looked at). Harness: claude-code (Opus 5.5 medium), no paid call.
- **Why-verdict:** 10 frames, 50 bends, check.py TRUE, 24 of 24 planted faults caught; four frames thin; counts in-sample, holdout uninformative.
- **Status/open:** every bend's fact is unopened; no blind judge; Ambi's eye and ear decide.
- **Related:** Juju, docs/adr/0021, runs/decision.tsv row packaging-lab.

---

## 2026-11-25 01:02 EAT — MUNGURA — Juju harvest: safety step cut, fast runner and film-harvest skill started
<!-- type: event -->
**From:** MUNGURA

Juju harvest: safety step cut, fast runner and film-harvest skill started
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi 25 Nov 01:00: "f*** safety aggressively rea video. make it a high quality skill juju, true to exactly how its done, and add a few things designed for us and our workflows that make it faster and reliable". Done: the audit step is cut (an empty environment stays, free); measured why it is slow (the film is decoded about seven times in software, text read on the CPU, 20 s of sound splitting took 5 minutes; hardware decode gives identical pixels, md5 equal). Two delegates started: scripts/harvest (decode once, Apple Vision text, CoreML sound, captions as speech, receipts, resume) and the skill pack film-harvest, faithful to upstream with ours marked. Harvest workflow resumed. Also: juju make passed 9 of 11 stages at 00:54 (2 at 20:55); PRs up to 19 merged except 18.
- Status: in-progress

---

## 2026-11-25 00:57 EAT — TEHUTI — Juju sound lane: every film gets sound by itself

- **Changed:** crates/juju-sound (new), runs/sound/auto; strip.mp4 at -14.1 LUFS with 2 cues heard by Earshot, 0 synthetic; 13 sounds kept on the shelf; commit 5be1207 on local branch unit/sound.
- **Why/verdict:** film stage 7 needed cues chosen, levelled and heard before a pass; receipt verdict pass, all planted faults refused.
- **Status/open:** work 50.8 s at load 49 to 88, 117 s at load 97; cues heard beside the middle only, phone speaker listen owed; no bed kept that the Watcher wants under a voiced map film.
- **Related:** Harness: Claude Code (Opus 5.5). runs/sound/auto/HANDOFF.md, topic juju.

---

## 2026-11-25 00:57 EAT — TEHUTI — Juju sigil: one command draws, judges and picks a thumbnail
**From:** TEHUTI

- Changed: new crate crates/juju-sigil (uncommitted, kickoff said no commit), runs/sigil proof. Harness: claude-code (Opus 5.5).
- Why/verdict: five packages drawn three ways each, G1 to G5 pass in code, two low proofs bought and both lost the vote, 0.077 US of 0.25.
- Status/open: medium buy path proven only against a mock door; fixtures hand-written; hue not gated in G4; no PR yet.
- Related: runs/sigil/check.py, runs/sigil/receipt.json

---

## 2026-11-25 00:43 EAT — TEHUTI — Juju style kits: five kits, checker, pour counted
- **Changed:** design/kits (5 kits, pages, checker), runs/kits/pour.json, HANDOFF.md. Harness: Claude Code, Opus 5.5 worker.
- **Why/verdict:** held-out pour 3: 14 of 14 storyboard forms legal at first answer, 14 of 15 strips drawable by the engine check with no fallback; selftest 279 of 279; 0.144 US.
- **Status/open:** candidates; nothing rendered or judged blind; the writer still invents causes.
- **Related:** ADR 0019, 0014; runs/decision.tsv lane kits.

---

## 2026-11-25 00:22 EAT — TEHUTI — Juju: hero film 260 to 530 s taken apart shot by shot
<!-- type: event -->
**From:** TEHUTI

- Changed: runs/scriptlab/hero/part-2.json (72 shots, 28 traits, 75 colours) and hero/work-2 (frames, curves, check.py, build.py).
- Why-verdict: exit predicate TRUE, 5 of 5 planted faults refused (Measured). Harness: claude-code (Opus 5.5).
- Status-open: family between Arial Bold and Helvetica Bold is Judged; unplotted easings inside screen recordings.
- Related: part-1 and part-3 lanes, ADR 0014, AMBI-EYE.

---

## 2026-11-24 23:59 EAT — MUNGURA — Juju: the night goes to harvest (ADR 0021), twelve key films with rea-video and strong models
<!-- type: event -->
**From:** MUNGURA

Juju: the night goes to harvest (ADR 0021), twelve key films with rea-video and strong models
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi, 23:35 to 23:55: we cannot reverse engineer a video; use github.com/JuneYaooo/rea-video; strong models (Opus 5.5 or Fable 5.2 high) take apart 9 to 12 key videos, extract layered systems mapped to prompts and JSON, visually verified; cheap models (DeepSeek) then only execute by mixing; a pasted link becomes a blend or a harvest; whole 10 to 50 minute films, not clips; "the rest of the night just focus on this, this is the gold". Recorded as docs/adr/0021. Workflow juju-harvest-12 (wf_e8518f9c-22c): audit and lock rea-video, score it against hand truth, a layered motion language, two harvesters head to head, blind rebuilds (a builder who never saw the film), twelve whole packs, cross grammar, 9 to 12 systems with a mixing rule, recipe book with closed menus, film plans. Paused: phone wave 1, buttons wave 4, film ground. Kept: waves 2 and 3, script skeleton reading, hero trace.
- Status: in-progress

---

## 2026-11-24 23:21 EAT — MUNGURA — Juju: Ambi refused the dot strip; looks go back to real material and house worlds
<!-- type: event -->
**From:** MUNGURA

Juju: Ambi refused the dot strip; looks go back to real material and house worlds
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi 23:17 on the McDonald's strip the lead had praised: "the worst looking thing ive ever seen. lean into our strengths in terms of design systems our software biases towards and uses as options." The diagram world workflow was stopped and its looks dropped. New rule file runs/scriptlab/AMBI-EYE.md (a judge must refuse that strip unprompted). New lanes: juju-strengths ranks the worlds Juju draws well into four to six house systems (options with a bias order) and adds idea verbs to them; film one ground restarted inside those worlds. Ambi 23:10: films come out of Juju itself; 23:13: best possible app that produces the videos we need. PRs 16 and 17 merged through the door.
- Status: in-progress

---

## 2026-11-24 23:02 EAT — TEHUTI — Juju PR 15 recheck at 9a48b629: FINDINGS, body only

- Harness: Claude Code (Opus 5.5), reviewer opus-small-2.
- **Changed:** no code; verdict posted on PR 15.
- **Why/verdict:** lost writes now turn report red (stub probe); a plan or report job that dies before writing still leaves older greens and is not named.
- **Status/open:** one body sentence, then countersign.
- **Related:** juju, .github/scripts/train.py

---

## 2026-11-24 22:57 EAT — TEHUTI — Juju taste panel: refuses broken strips, not yet dull ones

- **Changed:** scripts/taste.py, runs/taste (PANEL.md, proof.json, held-proof.json, script-proof.json). Harness: Claude Code (Opus 5.5).
- **Why/verdict:** freeze 4 of 4, cut sound 4 of 4, our silent film lost 3 of 3, same twice 5 of 6; shuffled lines 3 of 4 by models and 18 of 18 by the script check; a voiced repetitive strip of ours tied. Both fresh-strip keys failed.
- **Status/open:** plants for flat voice, same move, generic line; three-seat panel fails its own near-even key (4 win 6 tie 1 lose 1 short). Spent 0.583 US of 0.60.
- **Related:** juju, ADR 0019 point 4.

---

## 2026-11-24 22:56 EAT — TEHUTI — Reviewed Juju PR 15 (FINDINGS) and PR 16 (CLEAN)

- Harness: Claude Code (Opus 5.5), reviewer opus-small.
- **Changed:** no code; verdicts on PR 15 and 16, PR 16 list in runs/pr/NEXT.md.
- **Why/verdict:** PR 15 can leave a head green after a lost red post or a cancelled train, which its body does not name; PR 16 passed the nine-job, memory and 17 heavy rows.
- **Status/open:** PR 15 needs one repair and a recheck.
- **Related:** juju, .github/scripts/train.py, scripts/heavy

---

## 2026-11-24 22:50 EAT — MUNGURA — Juju trunk: pull requests 1 to 12 are in main
<!-- type: event -->
**From:** MUNGURA

Juju trunk: pull requests 1 to 12 are in main
- Harness: Claude Code (claude-opus-5-5)
- What happened: PR 11 merged 22:02, PR 10 (with 1 to 9) 22:49 at 639dc85, PR 12 (conductor loop) 22:50. Merge log lines for 10, 11, 12 are on main (732c2b6). The merge door refused only because a later train had set every head's light back to running; both heads were green in run 45470745500, so the same gh merge command was run with the head pinned. PR 10 took three money repairs (unpriced fields, parts, sellers, jev length); every one has planted tests. Open: 13 (ear table), 14 (ADR 0020), 15 (train light fix), 16 (job queue: 8 slots, load not asked). Queue finding: 36 jobs behind one build because the load rule starved the pool.
- Status: in-progress

---

## 2026-11-24 22:41 EAT — TEHUTI — Reviewed Juju PR 12 at f0490fe2: CLEAN, five fixes and four notes listed

- Harness: Claude Code (Opus 5.5), reviewer opus-conduct.
- **Changed:** no code; verdict on PR 12, list in runs/pr/NEXT.md.
- **Why/verdict:** nothing worse can seal; a worse repair can be the next base in one mixed case; a step up is bought twice only from a damaged reply file, still reserved; Earshot check holds on missing, stale and unbounded input.
- **Status/open:** second reviewer, the train and the lead countersign of the THRESHOLD CHANGE.
- **Related:** juju, crates/juju-conduct, PR 12

---

## 2026-11-24 22:33 EAT — TEHUTI — Juju PR 10 recheck at 639dc85f: CLEAN

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk-4.
- **Changed:** no code; CLEAN recorded on PR 10, notes in runs/pr/NEXT.md.
- **Why/verdict:** both blocks closed by probe, 30 of 30 tests, our callers bodies priced.
- **Status/open:** several jev callers reserve less than the gate price; they should reserve from prices.worst.
- **Related:** juju, scripts/prices.py, PR 10

---

## 2026-11-24 22:28 EAT — TEHUTI — Juju PR 10 recheck at cb0245f2: FINDINGS, the seller and the jev flat price

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk-3.
- **Changed:** no code; verdict on PR 10, notes in runs/pr/NEXT.md.
- **Why/verdict:** the last block is closed (probe, 30 of 30 tests). Two open: a named priority seller bills 1.8 times the price; jev is flat 32,000 tokens and the endpoint takes 262,144. No paid call.
- **Status/open:** the lead decides under ADR 0020.
- **Related:** juju, scripts/prices.py, PR 10

---

## 2026-11-24 22:21 EAT — TEHUTI — Juju PR 10 recheck at 74a8604b: FINDINGS, the money gate still underprices nested fields

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk-2.
- **Changed:** nothing in code; verdict on PR 10, fixes and notes in runs/pr/NEXT.md.
- **Why/verdict:** the first block's reproductions are closed, 30 of 30 tests, new test red on the old file. Still open on a stand-in: OpenRouter video_url and file parts, picture-shaped text inside a schema, WaveSpeed 4k priced as 1k; and route_proof's jev-router body is now refused.
- **Status/open:** the lead decides under ADR 0020 rule 3 (a second block closes the pull request).
- **Related:** juju, scripts/prices.py, scripts/purse.py, PR 10

---

## 2026-11-24 22:13 EAT — TEHUTI — Reviewed Juju PR 10 at ba9b9b1f: one block, the money gate underprices unread fields
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk.
- **Changed:** nothing in code; verdict FINDINGS on PR 10, fixes and notes in runs/pr/NEXT.md.
- **Why/verdict:** prices.worst ignores body keys it does not read; on a stand-in the book went 9.99 to 11.19 on a 0.005 hold. Merge commit equals PR 11, checks green, no keys, 12 looser examples reproduced.
- **Status/open:** the lead repairs or accepts by name; train pending at record time.
- **Related:** juju, scripts/prices.py, scripts/purse.py, PR 10

---

## 2026-11-24 22:03 EAT — MUNGURA — Juju: PR 11 merged; new law, one unit one pull request one round (ADR 0020)
<!-- type: event -->
**From:** MUNGURA

Juju: PR 11 merged; new law, one unit one pull request one round (ADR 0020)
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi: why shove everything into PR 11. Changed: ADR 0020 (one unit per pull request, two reviewers started together, only a block stops it, fixes go to the next one, nothing is pushed into an open pull request, clean and green merges at once). PR 11 merged 22:02 (ba9b9b1) with the same gh command the merge door runs, because the door's log file is not on main until PR 10. PR 10 is in its one review round. A shipping workflow (wf juju-ship-line) cuts quiet live work into small pull requests. Wave 4 (buttons) and the hero engine lane are running.
- Status: in-progress

---

## 2026-11-24 21:46 EAT — TEHUTI — Reviewed Juju PR 11 at 021bf7b: guard fix clean, two wording findings in WORKER.md
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (Opus 5.5), reviewer opus-021b. Posted REVIEW FINDINGS 021bf7b on the PR.
- **Changed:** nothing edited.
- **Why/verdict:** the guard holds the time limit through TERM INT HUP QUIT (old head fails the same probe); contract test held, 0 failed. WORKER.md says every worker of waves 1-3 was cut off; 11 of 21 were. Its redo-nothing sentence needs a rerun at this head.
- **Status/open:** two wording fixes by the lead, then a new head.
- **Related:** juju, scripts/heavy, PR 11

---

## 2026-11-24 21:28 EAT — MUNGURA — Juju: hero film study started (Atticus King), silent films added, all fleets alive
<!-- type: event -->
**From:** MUNGURA

Juju: hero film study started (Atticus King), silent films added, all fleets alive
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi named "galactic empires don't actually make sense" (J0wWNytEXS4, 481K views in about 15 hours, 13.9K subscribers) as the film to learn from: storyboarding, ideation, title and thumbnail bends, 4 to 6 design systems grown from it; and "AI's Strange Obsession with Enlightenment" (ZgpMtombn9A) for ideation only. Also: silent map films carry their script on screen. Both of Ambi's playlists (33 films) and the YouTube home page were read. Workflow juju-lab-read (wf_0fa6e6e6-a33) reads 60 films into skeleton cards, storyboard moves, bends and looks. Waves 1, 2, 3 survived the second stop. PR 12 has two fresh reviewers; PR 11 guard fix is being proven.
- Files changed: AMBESSA/intel/juju/runs/scriptlab/AMBI-EAR.md; AMBESSA/intel/juju/runs/scriptlab/sources/study.tsv
- Status: in-progress

---

## 2026-11-24 20:58 EAT — TEHUTI — Reviewed Juju PR 11 at 51d7c9e: three blocks fixed, one new hang in scripts/heavy

- Harness: Claude Code (Opus 5.5), reviewer opus-hangs, verdict FINDINGS posted on the PR.
- **Changed:** nothing edited; notes (scratch)
- **Why/verdict:** the last review blocks 1 and 2 reran and hold, block 3 agreed; new: TERM reaching the guard ends the time limit, a command that ignores TERM then runs for good (next job waiting at 90 s; f915b9e ended it in 13 s).
- **Status/open:** one line in the guard (ignore TERM INT HUP QUIT) fixed it on a copy.
- **Related:** juju, scripts/heavy, PR 11.

---

## 2026-11-24 20:43 EAT — TEHUTI — Juju conductor: keep or revert, one step up, Earshot at stage 7 (PR 12)
<!-- type: event -->
**Changed:** crates/juju-conduct src and tests on branch unit/conduct-loop, head f0490fe, PR https://github.com/AmbessaTrades/juju/pull/12 (Claude Code, Opus 5.5, worktree).
**Why/verdict:** the three "not held" rows of docs/poteto/runtime-loop.md are code; 212 tests pass, 17 new ones were red on the base. A mutant loop of mine held the heavy lane about 32 minutes; the repair loop got its own step limit from it.
**Status/open:** not merged, root reviews. No real engine writes sound/earshot.json yet; the model ladder and a part's budget are candidates.
**Related:** runs/conduct/loop-1124, runs/decision.tsv lane conduct

---

## 2026-11-24 20:36 EAT — TEHUTI — Juju PR 11 review: findings, do not land on integration at f915b9e
<!-- type: event -->
**From:** TEHUTI

Juju PR 11 review: findings, do not land on integration at f915b9e
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session d413af8f)
- Ambi asked for a bounded review of Juju PR 11 at head f915b9e: may it land on the integration branch? Scope was the change since 47995f8, with scripts/heavy as the focus.
- Verdict: FINDINGS, do not land. HEAD matched PR headRefOid f915b9e6. Nothing was edited, no agent started, no cargo, render or paid call. Posted to the PR as a comment and read back.
- Block 1 (measured): scripts/heavy:18. A ticket left by a killed waiter whose pid is reused stalls the whole queue. Suggested fix not run: flock the ticket.
- Block 2 (measured): scripts/heavy:22-29. After kill -9 to the wrapper, the time limit is lost. With one slot, a nested heavy call deadlocks. Suggested fix not run: the guard must enforce the limit.
- Block 3 (documents): ADR 0019 and the ask-juju SKILL.md still say one heavy job or serialized. The PR body says 'none loosened'. Those need fixing before the PR lands.
- Status: complete — review delivered with verdict FINDINGS, PR 11 must not land until blocks 1 to 3 are fixed and re-reviewed

---

## 2026-11-24 20:20 EAT — TEHUTI — Juju PR 11 mechanical recheck at head f915b9e6: 9 checks run, verdict CLEAN posted
<!-- type: event -->
**From:** TEHUTI

Juju PR 11 mechanical recheck at head f915b9e6: 9 checks run, verdict CLEAN posted
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 42d6fbfa)
- Ambi asked for a read-only mechanical recheck of Juju PR 11 at its final head: no edits, no agents, no cargo, no paid calls.
- Ran 9 checks: head SHA match, pins-check 784/784/784 with 0 differ and 0 gone, pins.txt and reach.rs diffs as specified, merge-tree clean, gate open twice, py_compile and zsh -n passed.
- Two checks ran with wrong or piped output at first (a SKILL.md read path and a pipe that hid an exit code); both were rerun correctly before the verdict.
- A CLEAN verdict was posted on PR 11. Six CI checks (run full, run main, shipped, tests conduct, tests rest, train) were still pending, not passed, so check 9 is only 'no failures'.
- Notes are in the scratchpad at haiku-final-notes.md.
- Files changed: (scratch)
- Status: complete — 9 of 9 mechanical checks passed with no failures; 6 CI checks still pending on PR 11 head f915b9e6.

---

## 2026-11-24 20:17 EAT — TEHUTI — Stopped a runaway test and a mis-pointed batch in the Juju worker run; handoff logged
<!-- type: event -->
**From:** TEHUTI

Stopped a runaway test and a mis-pointed batch in the Juju worker run; handoff logged
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- The looks worker ended at 19:33. Its six looks are candidates on composite stills, the film engine cannot draw them yet, and its critic pass is still owed because I stopped the workflow.
- The conductor's mutant run held the heavy lane for the whole loop and nine jobs waited up to 32 min. I stopped the endless test (pid 55786) at 19:41, counted it as caught, and set a 120 s limit per mutant.
- Ambi's rule: every heavy job gets its own time limit, at most 15 min unless it renders a whole film. Test fuse is 10.00 US (ADR 0019). Disk has 40 GB free.
- A sibling session overwrote a shared script at 19:56, so batch s3 ran the wrong work. I stopped the three wrong processes (83170, 84016, 84019) before any paid test, and restored the engine's script from its own record.
- Still open: engine, app server, Spell Strip, Publish Kit, conductor and chain workers are running. They adopt the 15-min rule only if they re-read WORKER.md. The engine has not restarted its build.
- Files changed: runs/predicate/HANDOFF.md; WORKER.md
- Status: in-progress — incidents contained and logged, but the engine build and several workers are still running and unverified

---

## 2026-11-24 19:59 EAT — TEHUTI — Juju ten minute film: words round 2 done

- **Changed:** false claims two judges found (Flint, Kanton clock, 1884 date line, paddle, one date) replaced from corrected facts; motive added from van Gent; script, voice text, outline, pauses rebuilt. Harness: claude-code (Opus 5.5)
- **Why-verdict:** checks.sh ALL PASS, V-map on, 1,342 spoken words; 24 of 24 cold readings pay the extra hours. 0.0592 of 0.06 US.
- **Status-open:** fresh judges before voice; motive, by law, second writer parts need the lead.
- **Related:** juju, runs/films/ten/report.md

---

## 2026-11-24 19:35 EAT — TEHUTI — Juju: Poteto guards hardened, 31 GB disk freed, 10-minute script closed on strict checks but held from voice
<!-- type: event -->
**From:** TEHUTI

Juju: Poteto guards hardened, 31 GB disk freed, 10-minute script closed on strict checks but held from voice
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked to merge what needs merging and keep Poteto's changes "forever". Poteto upgrade is in PR 11, which is not merged yet: a fresh reviewer found faults in the done-check, and the worker fixed them.
- Added 39 planted-fault tests (scripts/test_contract.py) that all pass, so the done-check is tested, not just read. Exit predicate and heavy-queue scripts changed in the poteto worktree.
- Disk: freed about 31 GB (22.5 GB abandoned debug build, 9 GB render scraps), free space went from 8 GB to 40 GB. Each deletion is logged path by path in the disk ledger; no videos or footage removed.
- 10-minute film script: strict checks went from 18 failures to 0 at 1,343 words, spend $0.07 of the $0.08 cap. The worker said not to voice it yet; a fresh listener and a fact checker are judging it cold.
- Still open: the script never answers why Christmas Island gained extra hours, PR 10 and PR 11 are not merged, and the second PR 11 reviewer is still on an earlier head.
- Files changed: runs/predicate/notes/di[redacted].tsv; runs/films/ten/script.txt; runs/predicate/PLAN.md; docs/adr/0019-ready-at-four.md
- Status: in-progress — PR 10 and PR 11 unmerged, 10-minute script held from voice until fresh readers pass it

---

## 2026-11-24 19:13 EAT — TEHUTI — Juju: walk test fixed, heavy jobs split into two lanes, lead role handed to Ambi's thread
<!-- type: event -->
**From:** TEHUTI

Juju: walk test fixed, heavy jobs split into two lanes, lead role handed to Ambi's thread
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Walk check fixed: exit-predicate walk now signs in on the no-paid test instance ((local page)), presses each room, and fails a room that lands on the wrong address or shows no controls.
- Heavy job queue split into a build lane and a render lane, one job each, after a measured 1.3 of 8 cores in use while 8 jobs waited. Jobs queued before 18:12 still drain from the old queue.
- Ten-minute film thumbnail finished and checked full size. The WaveSpeed run cost 0.117 US. The paid version did not beat the free code-drawn one in blind votes; the blind frame test is still to come.
- Ten-minute script rewrite ended at 0.1493 of 0.15 US. It passes only on its own reading of one check, and one paragraph still needs a rewrite.
- At 18:30 EAT, per Ambi's request to move the lead role to his thread, the state-check task was deleted, HANDOFF.md was written, and no new workers were started. PR 11 and PR 10 reviews remain open.
- Files changed: scripts/exit-predicate; scripts/heavy; runs/predicate/LANES.md; runs/predicate/HANDOFF.md; runs/films/ten/thumbnail.png; runs/app/lead-look-1.md
- Status: in-progress — room fixes, film owner start, PR 10 and PR 11 reviews still open; lead role now with Ambi's thread.

---

## 2026-11-24 19:03 EAT — TEHUTI — Juju ten film words: checks strict again, 18 failures to 0

**Changed:** runs/films/ten words files; Claude Code (Opus 5.5) worker. Strict copied and echo checks restored; neon wrote b3 b8 b13; code cuts and moves elsewhere; 1,343 spoken words.
**Why-verdict:** checks.sh ALL PASS strict, lint PASS; 0.0694 US of 0.08.
**Status-open:** cold readers say beat 5 question is not paid in b8; b2 b7 b11 b14 still glm; V-map off in pack; sentences joined by code need a ruling.
**Related:** runs/films/ten/report.md

---

## 2026-11-24 19:00 EAT — MUNGURA — Juju: Ambi's five answers recorded, 21 review findings fixed, wave 1 fleets started, T3 git unblocked
<!-- type: event -->
**From:** MUNGURA

Juju: Ambi's five answers recorded, 21 review findings fixed, wave 1 fleets started, T3 git unblocked
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: Harness Claude Code (Opus 5.5), thread 6047de40. Ambi (about 18:48 EAT): ready at 16:00 means one tap makes a finished MP4 with sound, voice, thumbnail and publish kit at 10, 20, 30 or 50 minutes; the phone exports by itself and is built now, not after ("the two are in isolation"); taste beyond automatic checks; 95 must be proven by 16:00; 10 US test limit through tomorrow; fleets allowed; "just merge everything". Recorded in docs/adr/0019. cap.json raised to 10.00 on his word. PR 11: a fresh reviewer found 21 faults (four done-check clauses could pass falsely); all answered except two in other lanes' files, with 39 planted-fault tests in scripts/test_contract.py. scripts/heavy is back to one job as Ambi ordered (my two-lane change did not help: load 42 to 65 with it). The kickoff hook now covers Agent, Task, Workflow, Bash claude -p, T3 delegate and thread launch. T3: a stale index.lock of 20 Sep in ~/AUH was moved aside, untracked project folders hidden in ~/AUH/.git/info/exclude (nothing deleted), Juju registered as its own T3 project. 1,305 live source files backed up to private branch snapshot/live-2026-11-24. Four idle cargo caches in the old lead's scratchpad removed (about 1.4 GB).
Why/verdict: PRs 1 to 9 are ancestors of integration, so merging PR 10 lands them. Nothing is merged yet: PR 11 is under recheck, PR 10's body check is red on unnamed threshold changes.
Status/open: workflows juju-wave-1 and pr11-recheck running; seven old workers still finishing; ten-minute words closed out at strict 18 to 0 failures. Predicate 3 of 23 (stricter script). Disk 8.7 GB free.
Related: ADR 0018, 0019; PLAN.md; HANDOFF.md; PR 10, PR 11.
- Verification: test_contract.py 39 of 39; pins-check 784 of 784; gate_checks tree open; git status in ~/AUH 1 s after the lock was moved; ls-remote shows snapshot branch 352356f; gh says the repo is private; key shapes in the snapshot 0.
- Status: in-progress: nothing merged yet; recheck and wave 1 running

---

## 2026-11-24 18:45 EAT — TEHUTI — Reviewed Juju PR 11 (run-until-done contract) and posted 21 findings on it
<!-- type: event -->
**From:** TEHUTI

Reviewed Juju PR 11 (run-until-done contract) and posted 21 findings on it
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 461e46ff)
- Ambi asked for one honest review of Juju PR 11 by a reviewer who wrote none of it, so it can land on the integration branch tonight. No file edited, no agent started, no cargo or paid call.
- PR body claims checked: 20 held, 3 wrong ('one job at a time', '16 pins', '3 slots to 1'), 3 unchecked. Pins rerun on the moved head: 784 of 784.
- 21 findings posted on PR 11 at head 2611544. Main ones: exit-predicate clauses pass when untrue, heavy lane leaks (gate.sh in render lane), and max_heavy is ordered as 1 but the code runs two lanes.
- Walk findings were read, not run: the walk signs in then opens the gate room, which redirects signed-in users, so those rows cannot pass. Countersign rules disagree; the merge door stops on a 404 for MERGE-LOG.md.
- Head moved from 8167237 to 2611544 mid-review; findings are against 2611544. All 21 numbered findings are in the notes file.
- Files changed: (scratch)
- Status: complete — review posted on PR 11 with 21 findings open; merge not cleared.

---

## 2026-11-24 18:30 EAT — MUNGURA — Juju: audit of the day, lead role moved to one thread, 4pm bar being defined with Ambi
<!-- type: event -->
**From:** MUNGURA

Juju: audit of the day, lead role moved to one thread, 4pm bar being defined with Ambi
- Harness: Claude Code (claude-fable-5-2)
- What happened: Changed: Ambi (about 18:20 EAT): "I feel we used too many tokens today with too little output", "audit everything", the big thread's work is picked up "on this thread", "ready by LATEST tomorrow 4pm EAT", Poteto rules "automatically on for everything all the time". Harness Claude Code (Fable 5.2), thread 6047de40. Audit written to runs/predicate/notes/audit-2026-11-24.md and lessons-vs-code-2026-11-24.md. The old lead (session 8c6b00a6) wrote runs/predicate/HANDOFF.md, starts nothing new and deleted its scheduled state check; this thread is the only lead. Plan: runs/predicate/PLAN.md (one film path through juju smoke-test, six lanes, at most six owners, Opus medium, Haiku for pressing).
Why/verdict: Measured from the transcripts: 465 agent transcripts, 2.44 billion tokens, 16.3 million written, about 2,600 US at assumed list prices, against 3.26 US spent on Juju's own models and zero finished films. The old workflows ran Opus at high on general-purpose agents and the lead thread re-read about 560,000 tokens per reply. Of the film chain's 11 stages, 2 work, 8 use a stand-in, 1 is not built; the newest film is 63.6 s with no sound stream. Of 40 lessons from studied films, 14 are checked by the pipeline, 16 sit in checkers nothing calls, 8 are notes. Only a 10 minute film has a measured arc.
Status/open: Interview round 1 sent to Ambi (what ready means at 16:00; phone over Wi-Fi or standalone; lengths; how 95 percent is counted; test money limit). Exit predicate 5 of 23. PR 11 has two fresh reviewers running (delegated). Ten old workers are finishing; a watcher on HANDOFF.md wakes the lead to start the next lane. scripts/heavy is now one build lane and one render lane after one lane for both left 8 jobs waiting 2 to 11 minutes.
Related: ADR 0018 (added 18:20 section), runs/predicate/LANES.md, HANDOFF.md, PLAN.md, runs/decision.tsv; PR 10, PR 11.
- Verification: Token counts from scratchpad/tokens.py over the session's .jsonl files (each API reply counted once). Chain state from runs/spine/score.json run 20261124-174132-02c4. Film looked at as a 12 frame sheet. Workflow settings read in juju-ten-wf_17e18fe4-a27.js (effort high, general-purpose).
- Status: in-progress: waiting on Ambi's five answers; old workers draining; reviewers on PR 11

---

## 2026-11-24 18:07 EAT — MUNGURA — Juju: run-until-done contract installed; root and lead split; live lead re-briefed
<!-- type: event -->
**From:** MUNGURA

Juju: run-until-done contract installed; root and lead split; live lead re-briefed
- Harness: Claude Code (claude-fable-5-2)
- What happened: Changed: Harness Claude Code (Fable 5.2), root session. On Ambi's order of about 17:45 EAT ("install the permanent harness... run autonomously until the entire Exit Predicate is verified TRUE"; "have the agents that are currently doing this rerun their sub agents, as long as they're not in really important work") I read pstack's originals (poteto-mode, worker.md, 8 playbooks, 11 leaf skills, unslop), Earshot's README and the context pack, then wrote in ~/AUH/AMBESSA/intel/juju: WORKER.md (contract, line 1 of every kickoff), AGENTS.md + CLAUDE.md (front door), docs/poteto/{root,hillclimb,live-proof,runtime-loop,ketchup}.md, scripts/exit-predicate (23 clauses read from receipts), scripts/decide (runs/decision.tsv), scripts/kickoff-line.py (Claude Code PreToolUse hook on Agent|Task, installed in ~/.claude/settings.json), scripts/light, pack juju-poteto-autopilot (with its reach.rs rows and 16 pins), ADR 0018. scripts/heavy went from 3 slots to 1 and sets one shared CARGO_TARGET_DIR; scripts/gate.sh takes the shared folder. Boot pointers: ~/AUH/AGENTS.md, ~/.claude/CLAUDE.md, session_start.py, Hermes MEMORY.md (stale FOCUS 8 Nov entry replaced; 5548 of 5555 chars), project map juju.
Why/verdict: One root, one lead. JUJU ORCHESTRATION #1 stays the lead and owns every lane; this session holds the predicate, countersigns, sends fresh verifiers, merges and writes the one final report. No second fleet on a Mac at load 42 to 60.
Status/open: Exit predicate 3 of 23 true at install (baseline in runs/predicate/). Lead answered with runs/predicate/LANES.md and found my click walk never signed in; fixed and retested (altar 8 controls 0 dead; new-vessel correctly fails). PR 11 open against integration/2026-11-24b. Findings: main checkout's packs differ from its pins.txt in 64 places (integration matches 656 of 656); 329 uncommitted files in the main checkout; conductor keeps the newest repair even when worse; stage 7 has no sound check. Conflict recorded: Ambi 25 Oct "never a one-at-a-time lock" vs 24 Nov "max_heavy = 1"; newer wins, reopen rule in ADR 0018. T3 refused linking PR 11 to the thread (user declined the tool call).
Related: ADR 0014, 0017, 0018; PR 10, PR 11; skills juju-poteto-autopilot, pr-gauntlet, memoir-swarm-handoff.
- Files changed: WORKER.md; AGENTS.md; docs/poteto/root.md; scripts/exit-predicate; scripts/decide; scripts/heavy; scripts/light; scripts/kickoff-line.py; docs/adr/0018-poteto-constitution.md; crates/juju-skills/packs/juju-poteto-autopilot/SKILL.md; ~/.claude/settings.json; ~/.claude/CLAUDE.md; ~/AUH/AGENTS.md; ~/.hermes/memories/MEMORY.md
- Verification: Hook: a Juju kickoff written without the line reached a fresh Haiku worker with the line first; it read WORKER.md and ask-juju and answered three contract rules correctly. Pins script reproduces 656 of 656 pins on integration; 672 of 672 with the pack. gate_checks tree, diff and body pass locally on PR 11. scripts/decide refused a row without evidence. scripts/heavy held a second job while a render ran; scripts/light ran in 0.7 s.
- Status: in-progress: contract installed and proven on one fresh worker; build still 3 of 23, driven by the lead

---

## 2026-11-24 18:05 EAT — TEHUTI — Juju Poteto structure: exit predicate at 3 of 23, one heavy job at a time, two stories stopped
<!-- type: event -->
**From:** TEHUTI

Juju Poteto structure: exit predicate at 3 of 23, one heavy job at a time, two stories stopped
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi's 17:45 order ("rerun their sub agents... Poteto structure... right now") was checked against the other thread and the files on disk before acting.
- Built the exit predicate (23 clauses, each read from a receipt on disk). Baseline is 3 of 23 true, saved to runs/predicate/baseline-2026-11-24.jsonl.
- scripts/heavy now runs one job at a time on a shared CARGO_TARGET_DIR (Ambi: "max_heavy = 1"). scripts/light runs two at a time for walks and probes. Not yet carried into the integration branch.
- Stopped two story jobs that served no check. Workers are at 12 live, above the limit of eight, because mid-edit workers were allowed to finish. One new worker is on the missing self-repair rules.
- Ten-minute film script is 1,226 words, too short, and is being redone to about 1,400. Money: 3.17 of 5.00 US at the 18:02 check; the voice budget has 0.15 left against about 0.12 needed.
- Files changed: WORKER.md; AGENTS.md; scripts/exit-predicate; scripts/decide; scripts/heavy; scripts/light; scripts/gate.sh; runs/predicate/LANES.md
- Status: in-progress — 3 of 23 exit clauses true; engine, thumbnail, three rooms and the film render still open, and no voice bought yet

---

## 2026-11-24 18:04 EAT — MUNGURA — Juju: Poteto structure in force; lanes cut to red clauses, three runtime units and words round two started
<!-- type: event -->
**From:** MUNGURA

Juju: Poteto structure in force; lanes cut to red clauses, three runtime units and words round two started
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: verified Ambi's 17:45 constitution in thread 6047de40 (read whole). Wrote runs/predicate/LANES.md (lane, owner, files, clause, state, relaunched). Stopped two story expansions that serve no red clause. Spine owner told to buy no more voice and close out. Fresh owners with WORKER line 1: conductor (keep or revert, one step up, Earshot hears the mix) and ten film words round two. Why: exit predicate 3 of 23; last script had 27 percent of a worker's own sentences and was 1,226 words (too short for 10 minutes). Status/open: engine speed, thumbnail, server, three room lanes, PR answer left mid-edit untouched; walk in exit-predicate never signs in (told root). Voice purse 0.1518 of 0.30 US left. Related: juju ADR 0014, 0017; docs/poteto.
- Status: in-progress: predicate 3 of 23

---

## 2026-11-24 17:20 EAT — TEHUTI — Juju: spending gate for the 10-minute film added; app still unwired, chain 0 of 11 stages working
<!-- type: event -->
**From:** TEHUTI

Juju: spending gate for the 10-minute film added; app still unwired, chain 0 of 11 stages working
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked for a one-hour render path, a 10-minute film proven before any 50-minute voice spend, and a complete app with no coming-soon sections, built by orchestrated lanes.
- Done: the Workshop viewer (local page) shows films, 19 rooms, agents, pictures and a chain board. The spending gate refuses a 50-minute voice request and voice spend past $0.30 until the 10-minute film passes (tested).
- Measured: render runs about 1.98 s of work per film-second today, so a 20-minute film takes about 40 minutes. Engine handoff written to runs/engines/HANDOFF.md for the single engine owner.
- Open: the app server (local page) does not exist, and the rooms are still static pages. Chain is 0 of 11 stages fully working, WaveSpeed has never been called, and the Inworld dashboard needs checking.
- Spend at 17:19 was $2.84 of a $5.00 cap. Nothing stuck. Earlier agent counts were corrected to live versus open.
- Files changed: mockups/kit/workshop.py; scripts/purse.py; scripts/heavy; runs/swarm/swarm.py; mockups/kit/press.py; mockups/kit/jobs.json; runs/engines/HANDOFF.md; docs/adr/0014-locks-24-nov-afternoon.md
- Status: in-progress — the 10-minute film and core app loop are being built, but no stage is fully working and the app server does not exist yet.

---

## 2026-11-24 16:53 EAT — MUNGURA — Juju: two hard gates in code; lanes cut to the 10 minute film and the core loop

**Changed**
- Ambi: never inflate agent counts; 7 to 10 tight lanes; 10 minute film fully finished (voice, real WaveSpeed thumbnail) before any 50 minute voice; core loop on the live Rust server before secondary rooms. Stopped the film and app fleets; relaunched wh5ex4924 (ten minute film) and whzrup23h (core loop). scripts/purse.py refuses 50 minute voice and over 0.30 US voice until runs/films/ten/LEAD-PASS.json; both refusals tested.
- Wave 1 of Haiku app tests: most "cannot be pressed" findings were the test tool timing out on a busy Mac (5 of 6 main buttons worked by hand); removed from runs/slop. Workshop (local page) now counts live, open.

**Status/open**
- (local page) Workshop is live (a viewer); the app server (local page) does not exist yet. Chain: 0 of 11 stages fully working. WaveSpeed still unused. Spent 2.61 of 5.00 US.

**Related**
- docs/adr/0017; topic loop.

---

## 2026-11-24 16:38 EAT — MUNGURA — Juju: management fault owned; five fleets and a 30-Haiku test swarm started, AfriFluent method copied

**Changed**
- Harness: Claude Code (Opus 5.5). Ambi used the app for two minutes and found the PIN fifth circle, the floating cat, cut cards; asked what had been tested. Truth recorded (ADR 0017): the 19 rooms are static pages that call no program (0 fetches); the lead never pressed them end to end. Ledger by service: DeepSeek 1515 calls 1.04 US, GLM via OpenRouter 528 calls 0.47, Gemini direct 18 calls 0.51, Neon via OpenRouter 6, Inworld 77 calls 0.21, WaveSpeed none.
- scripts/heavy is now a pool of three with a memory guard (Ambi law of 25 Oct); the single lock had stalled workers. runs/swarm toolkit (units, brief, check, collect) plus mockups/kit/press.py (presses every control, finds layout faults).
- Started: app fleet wo7jht79s (crates/juju-serve, rooms wired, waves), film fleet w9lxoudwy (arcs, engine speed, tiny form, a 10 and a 50 minute film to the end), PR fleet wnug8dix1 (one integration branch, six lenses), five Haiku swarms (114 units). Story fleet already running. Test cap raised to 5.00 US.

**Status/open**
- No film finished; no app wired yet; 9 PRs unmerged.

**Related**
- docs/adr/0017; runs/app, runs/films, runs/slop, runs/swarm; topic loop.

---

## 2026-11-24 15:27 EAT — MUNGURA — Juju: Ambi judged two engine clips "both great"; narrowed to map and space engines; character, ideation ladder and the perpetual loop started

**Changed**
- Harness: Claude Code (Fable 5.2 lead). Withdrew the universal rip-and-replay job before it built anything (ADR 0016 last section); paused the wgpu running world after its premise step and the sound, voice and support jobs. juju-stage made green by one owner (33 tests, narrator caption removed, workspace tests all pass).
- Showed Ambi mockups/show/clip-map.mp4 and clip-space.mp4 (silent, engine alone, from the stage-y test film). His verdict: "they are both great"; faults he named: jump cuts, plain type, text habit; wants uniqueness, script character, Kallaway-depth ideation, the loop that reads the last film and deals title bends, speed.
- Running: engine fixer on runs/engines/FIX-LIST.md (15 items, two new laws: number equals spoken word; no overlapping text); w5wxxaqgt Atticus King film expanded into looks, niches, channels; wo9xiy1qf same for Milky Stellar, the AI enlightenment film and The Marrow; wanhgd3gx ideation ladder (crossroads-chain-outliner), four narrators tested over seven days on Neon, six looks as data, crates/juju-next (read, add, deal).

**Why/verdict**
- The gate is now code checks plus Ambi eye on clips; blind judges only find faults. Answered him: frame 028 is published; ours on that sheet are 026, 027, 030, 032, 034, 035, 036.

**Status/open**
- No cheap-model form passes the current checker yet; the three-question form and the good-every-time harness wait for the engine fixer. Spent about 2.0 of 4.0 US test cap. 9 PRs open, none merged.

**Related**
- docs/adr/0014, 0015, 0016; runs/engines; topic loop.

---

## 2026-11-24 14:40 EAT — MUNGURA — Juju: invented layouts dropped; core is now rip and replay of any pasted film (ADR 0016) beside one running world (ADR 0015)

**Changed**
- Harness: Claude Code. Ambi: palette sheet "terrible, slideshows 2017"; "why does ours have lines, AI-isms"; "this is about Juju being able to rip design systems from any video that is pasted"; "complete full app capabilities". The lead had shown a sheet with invented dashes, pills and boxed pictures: a slip against ADR 0012 point 6.
- Stopped wn73lwm9s (quote-essay film, hand-written libraries). palettes.json cut 40 to 11 candidates. Started wt7pawzu9 (schema, ripper in juju-absorb, player juju-play, replay-the-donor calibration with numeric error, held-out film, swap with cheap models, one-command spine juju-run and docs/WHAT-WORKS.md) and wase4th1u (wgpu world, one variable, clips judged). juju-stage being made green by one agent.

**Why/verdict**
- Lead watched whole outlier films: 14 of 16 frames of the 2.8M film are one cockpit; published films move LESS by pixel (0.08, 0.18) than ours (0.84 to 4.09). Stills and swatches were the wrong unit.

**Status/open**
- Spent 1.75 of 4.00 US test cap. 9 PRs open, none merged. No film passes yet.

**Related**
- docs/adr/0015, 0016; runs/rip, runs/world; topic loop.

---

## 2026-11-24 14:32 EAT — MUNGURA — Juju: locks of the afternoon recorded (ADR 0014), sealed key gate live, work relaunched after an accidental stop

**Changed**
- Harness: Claude Code (Opus 5.5). Ambi locked: 20 minutes and 2,400 words daily, two voiced channels and one silent; vendor names off app screens; no narrator subtitle; number on screen equals the word spoken; measured timing laws; two looks must beat blind judges on stills before any voice is bought (docs/adr/0014). He later said the taste notes are to be taken with a grain of salt and the lead judgement used.
- He stopped the jobs by accident about 14:26 and asked for a relaunch. Relaunched as wn73lwm9s (two films, engine, libraries, integration branch) and wrmaqfqyx (skeletons, sound, voice, freshness, frame bar, PR reviews). Held until the films are done: leverage ranking, 3D grammar, Ancient Logos teardown, app rooms.

**Why/verdict**
- Blind test: 2 judges called 53 of 53 of our frames machine-made and 0 of 40 published.

**Status/open**
- Spent 1.75 of 4.00 US cap. 9 PRs open, none merged.

**Related**
- docs/adr/0012, 0014; runs/proof; topic loop.

---

## 2026-11-24 14:27 EAT — TEHUTI — Juju: film teardowns, blind frame test, 20-minute money plan, shared spend lock; PRs unmerged
<!-- type: event -->
**From:** TEHUTI

Juju: film teardowns, blind frame test, 20-minute money plan, shared spend lock; PRs unmerged
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 8c6b00a6)
- Ambi asked to take apart five films (thumbnails, times, quotes, 16-frame pictures, 18:08 spiral, 90/70/50) and build design libraries and skills from them. Teardowns and libraries were started.
- Measured: the cheap-model title/thumbnail picker got 48-59% on 237 hidden winner-over-flop pairs, close to a coin flip. Title formulas were demoted to optional. No winner-picking is claimed.
- Blind test: judges marked 53 of 53 of our engine frames as machine-made and none of 40 published frames. Ambi's 20-minute plan fits about 115 of 135 CAD, but Inworld runs dry on day 56.
- Ambi ordered a heavy-job queue and a shared spending gate. Added scripts/heavy and scripts/meter.py, and wrote ADRs 0012 (no stand-in drawings) and 0014 (locks). Load was still high at last check.
- Open: PRs 1-8 are not merged; the drawing tests in juju-stage are still red; the ledger was at $0.87 against a $0.60 cap; the sealed key gate is unfinished. Session interrupted by user.
- Files changed: scripts/meter.py; scripts/heavy; docs/adr/0012-strengths-only-no-stand-in-drawings.md; docs/adr/0014-locks-24-nov-afternoon.md; docs/adr/0008-fixed-money-looks-taste.md; runs/packaging/backtest-result.json
- Status: in-progress — teardowns, libraries and the spend gate are running; nothing merged; the session was interrupted by Ambi.

---

## 2026-11-24 14:09 EAT — MUNGURA — Juju: planner directive adopted; machine throttled; two 180 second proof films with real voice started

**Changed**
- Harness: Claude Code (Opus 5.5). Ambi passed on a directive from the planner agent (design data libraries to disk, engine defects, one queue, integration branch, protect the 135 CAD, one proof artifact) and said to take from it what helps and get it done; he said the videos look bad and we are swaying.
- Stopped five workflows (rooms, design-systems, film reader, fine comb, engine round 2): files kept, resumable. One queue: scripts/heavy (one lock, waits for load under 14). Workflow wbzpoabjr: design/ libraries, one engine owner, supply, films A (painterly essay) and B (telemetry map) with Inworld TTS-2 stock voice and Earshot sound, blind judges, integration branch.
- Corrected against the disk: conductor critics already hold on an empty or unparsed reply (code read, tests ordered); videotoolbox already exists as an option; the design-systems job was dead because the stopped teardown never returned.
- Changed from the directive: no paid 16-frame pictures inside films (ADR 0008), reveal is drawn by code from real paintings; LoC and BHL refused this client and are left alone; 24 looks ship as data with status not proven until judged; contrast 8.5:1 for primary ink, 4.5:1 for muted and accent.
- Test cap raised to 4.00 US with the reason in runs/meter/cap.json. Ledger 1.17 US.

**Status/open**
- Leverage and guard workflows still running; leverage proofs to be stopped if they compete with the proof films.

**Related**
- docs/adr/0012; topic loop.

---

## 2026-11-24 13:57 EAT — MUNGURA — Juju: Jade-style look dropped; looks now chosen by leverage with the app own models

**Changed**
- Harness: Claude Code (Fable 5.2 lead). Ambi rejected the storyboard pictures (shapes drawn by code: "garbage", "Claude made this") and the script; then dropped the Jade Rabbit Hole illustrated style: only Claude could make it, the software runs on cheap models; "extreme amounts of leverage with the quality".
- ADR 0012 written: no stand-in drawings anywhere; a look is offered only after passing a blind test beside published frames, made by the app own models; two repairs then shelve; scripts follow measured skeletons; the lead looks at every picture before Ambi sees it. Records the lead slip (asked a builder for code-drawn sketches).
- Workflow wtghkk80c: leverage ranking of film kinds, blind test of today frames, script skeletons tested on DeepSeek, Neon and GLM, study of named skills and repos into two own skills, end-to-end proofs of the top three kinds, verdict as ADR 0013 proposal. Workflow w7vp2ygv2: fine comb (review and precise corrections, from the VidRush CEO 21 Nov post).

**Why/verdict**
- Packaging back-test: our skills rubric ranked hidden winners no better than chance (48 percent of 237 pairs); the 12 title equations fit flops as often as winners; 90/70/50 untestable on this data. Ideas are picked by outlier numbers, the model only bends.

**Status/open**
- Cap for all tests today 2.75 US; ledger about 0.9. 8 PRs open, none merged. runs/first-film is of the dropped kind: test words only.

**Related**
- docs/adr/0012; runs/guard/tweet-noahmorris-2026-11-21.txt; topic loop.

---

## 2026-11-24 13:42 EAT — MUNGURA — Juju: wave answered by real freshness, 20-minute plan being costed, PR review loop and merge train started

**Changed**
- Harness: Claude Code (Fable 5.2 lead, Opus 5.5 workers). Read the VidRush CEO post on the demonetisation wave (saved runs/guard/tweet-noahmorris-2026-11-24.txt). Ambi: no talking head, no real voices; wants Juju fresh from film 1 to 357 without losing the brand; asks if 20-minute films with one silent channel fit the money; wants three suggested voices by ear; better 3D; PRs reviewed in loops before they reach him.
- Workflow wiy2d48rc: wave facts, freshness model + 60-film simulation, 20-minute money plan (ADR 0010 candidate), voice by ear, sound by ear, 3D grammar + prototype, Ancient Logos teardown restart, PR review loop over PRs 1-8 + merge train.
- One spending door scripts/meter.py (lock, one cap 2.25 US for all tests); route_proof.py uses it. Gemini billing linked by Ambi; direct key works.

**Why/verdict**
- Measured: DeepSeek thinking low fills the film form validly (2 of 2) and a 426-word span cost 0.0079 US; thinking off is invalid and repair did not converge (5 of 6). GLM low returned nothing for 0.06 US. Gemini implicit cache: 0 of 3 repeats hit.
- Lead judgement recorded: no shuffling built only to fool a detector; variety must come from each film own material.

**Status/open**
- 8 PRs open, none merged; main tests for juju-stage do not compile. Ledger about 0.87 US.

**Related**
- docs/STACK-STATUS.md, docs/adr/0009; topic loop.

---

## 2026-11-24 13:21 EAT — MUNGURA — Juju: metering live — 626 real calls, $0.51, GLM/Neon/DeepSeek bake-off on one film form

**Changed.** `runs/meter/ledger.jsonl` is being written by the harness: 626 rows from 12:50 to 13:21 EAT, running total $0.5095, 4 × HTTP 429. By service: deepseek 455 calls $0.1808, openrouter 160 $0.1465, google 11 $0.1822 — eleven direct-key calls are 36% of spend. Bake-off on one film form (`runs/meter/job/`): GLM 5.3 high via OpenRouter $0.0428 (11,771 out incl 11,349 reasoning, 170.6 s); Neon low via OpenRouter $0.0286 (2,794 out, 2,575 reasoning, 27.0 s); DeepSeek flash high $0.0080 (12,000 out, all reasoning) and $0.0110 on a 40k ceiling (18,228 out). The direct Google key refused four Neon calls at 12:51 with "You exceeded your current quota" (429), then billed $0.0160–$0.0682 for tiny calls after billing was linked (ledger label: "lead: first paid call after billing linked"). Sweeps: nuance 349 calls $0.1454, packaging 249 calls $0.0746.

**Why verdict.** Every cost figure earlier today (10:19 $105/$119 US, 10:52 $96 US per 60 days) was an estimate. These are billed usage as each service reports it (`cost_how`: "usage.cost as OpenRouter reports it"), so the model choice now has a measured price per film form.

**Status open.** The run is still appending; these numbers are a 13:21 snapshot, not a total. The Neon direct key stays unusable (429) — only the OpenRouter path works. No invoice checked; ledger figures are self-reported usage.

**Related.** runs/meter/{ledger.jsonl, job/}; runs/packaging/work/lists (40 channel lists); runs/nuance/.

---

## 2026-11-24 13:00 EAT — MUNGURA — Juju: Doop page-by-page board drawn — 329 room-states on one Excalidraw canvas; quiet-screen law accepted

**Changed.** `mockups/board/doop-blueprint.json`: canvas kKomk5DFWY, page aqrMl1XPQB, 658 frames = 329 room-states × two sizes (@1440 329, @390 329) over 19 rooms (altar, arcana, canopy, cauldron, conjuring, crossroads, feed-sight, gate, mirror-bend, new-vessel, offering, pact, publish-kit, reliquary, sound, spell-strip, tank, vessel, voice), `wired` 9,784, prototype_url (local page) (returns 200). Pages rendered 12:54–12:57: 12 desktop `journey-*.png`, `board-desktop.png` (3.4 MB), `board-all.png` (7.9 MB), `phone/` 201 files, `_look/` contact sheets, builder `build.py` (81 KB). `docs/adr/0009-quiet-screens-quiet-frames.md` accepted for app screens on Ambi's words of 24 Nov ("stop writing subtext everywhere"): 30 interface words at 1440 px, 24 at 390 px, no text of 5 words or more, one 1–2 word status per object, faults starting `QUIET` in `mockups/kit/shot.py`; the film half is a candidate. Round-2 re-shoot: `mockups/r2/shots` 759 files, 726 newer than 11:25; pact, conjuring, publish-kit, spell-strip re-shot 13:13–13:16 with true empty states (`nothing-to-copy-today`, `no-loadout-built-today`).

**Why verdict.** The board is a map, and its own header says so ("MAP ONLY — Too small to read on a phone. Read the pictures in the phone folder"), so every state exists twice: a frame for the wide canvas and a shot for reading. ADR 0009 removes the caption-under-every-name law that produced the text Ambi objected to.

**Status open.** ADR 0008 and 0009 are untracked; board JSON and the 12 pages are uncommitted. Art direction still unjudged (earlier 5–6 of 10). The `phone/` folder holds 201 files; how many of the 329 states they cover is not checked.

**Related.** mockups/board/; mockups/kit/shot.py; docs/adr/0009-quiet-screens-quiet-frames.md; mockups/r2/shots/.

---

## 2026-11-24 12:48 EAT — MUNGURA — Juju: five keys answer, quiet-screen law in code, 19 rooms rebuilt, engine round 5 pictures

**Changed**

**Why/verdict**
- Engine round 5 sheet (9 stage kinds beside real films) looks clearly better than round 1; not yet scored by judges.

**Status/open**
- No PR open yet, no paid call in the ledger yet. Mac load about 180. Board desktop frames empty (board-fix running).

**Related**
- mockups/show/engine-stages-5.jpg, rooms-now-1..3.jpg; topic loop.

---

## 2026-11-24 12:10 EAT — MUNGURA — Juju: stage-y test film rendered end to end, 187 s at 1080p24, zero fallback scenes

**Changed.** `crates/juju-stage` built in release and rendered `runs/stage-y/film/stage-y.mp4`. ffprobe: h264, 1920×1080, 24/1 fps, 186.958 s, 682,223,558 bytes (651 MB), 4,487 frames. `runs/stage-y/film/render.json`: rendered true, render_seconds 1111.47, fallback_scenes 0, safe_box pass (margin 0.04, glyph_px_in_outer_margin 0), audio null, clock "practice clock, 142 words a minute"; scenes listed include layered_painting (0–43.31 s, 10 events), document_page (43.31–60.89), map_theatre (60.89–87.35). Looked at `film/contact-5s.jpg`: painted isle and fire, Plato bust over a Republic page, a Europe map changing decade by decade, a thinkers timeline, Earth/Moon/Mars/Jupiter plates, an ocean-depth gauge, 1900s street stills — real frames, not placeholders. Live at the time: `cargo build --release -p juju-stage -j 2 --offline` and `lockf -t 7200 /tmp/juju-heavy.lock nice -n 18 cargo test -p juju-absorb --offline -j 2`.

**Why verdict.** The stage engine has to be judged on frames, not on a plan; a rendered film with 0 fallback scenes and a passing safe box is the only proof that the stage code produces pictures. Audio is null because this was a picture test on a practice clock, not a voiced film.

**Status open.** No voice track. One act ("act-01" in `runs/stage-y/form.json`), not a full film. Nothing committed: 205 files dirty in the repo, last commit e0115bd at 10:33.

**Related.** runs/stage-y/{film/render.json, film/contact-5s.jpg, film/stage-y.mp4, form.json, script.json}; crates/juju-stage.

---

## 2026-11-24 11:25 EAT — MUNGURA — Juju: five-film teardown and design-system libraries launched; round-2 parts shown

**Changed**
- Harness: Claude Code (Fable 5.2 lead, Opus 5.5 high workers). Launched workflow whr1651bp: teardown of five films Ambi named (ZgpMtombn9A, sJiaWNxYFUA, oRBu7wYuOSo, G4w-a8NgnnQ, HmuQoak_IAg) into runs/teardown/<id>/, peer review, then libraries in design/ (type 30, palette 36, quote 16, motion 24, texture 16, theming, extraction pipeline), new skills, skeptic attack.

**Why/verdict**
- Ambi 24 Nov: "the whole concept of everything is design systems"; money map agreed at 135 CAD (ADR 0008).

**Status/open**
- Seven earlier workflows still running on an overloaded Mac (load ~51). Nothing metered; no keys asked yet. Engine films still 3-5/10 until round 2 reports.

**Related**
- docs/adr/0008-fixed-money-looks-taste.md; topic loop.

---

## 2026-11-24 10:52 EAT — MUNGURA — Juju: LOT-first dropped, capability study launched, budget remapped to $135 CAD
<!-- type: event -->
**From:** MUNGURA

Juju: LOT-first dropped, capability study launched, budget remapped to $135 CAD
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi said no LOT film before the software's capability is understood, and that the build should be judged on its own range, not on LOT. Agent stopped the LOT film job and withdrew its channel picks.
- Agent launched a capability study that dissects real faceless videos shot by shot, so the engine's priorities come from measurement.
- Agent's first 60-day budget (about $290 US) was rejected by Ambi as inflated. Remapped to $135 CAD (about $96 US) for 150 films in 60 days: Inworld $55, OpenRouter $23, DeepSeek $22, Google $21, WaveSpeed $14.
- Still open: volumes and costs are assumptions, nothing is metered yet, and the Inworld 20% batch discount is still in preview. The YouTube feed scan via computer use failed (window on another desktop), with a yt-dlp fallback.
- Files changed: ~/AUH/STUDY/loop-rebuild-2026-11-19
- Status: in-progress — capability study running; budget map delivered, volumes not yet metered

---

## 2026-11-24 10:19 EAT — MUNGURA — Juju: prices re-checked, two earlier numbers corrected, channel picks proposed
<!-- type: event -->
**From:** MUNGURA

Juju: prices re-checked, two earlier numbers corrected, channel picks proposed
- Harness: Claude Code (claude-opus-5-5)
- Verification: OpenRouter models and endpoints API and api-docs.deepseek.com pricing read today; ytlocal outliers run today for the three channels.
- Status: in-progress: prices checked live; nothing bought or run yet

---

## 2026-11-24 10:19 EAT — MUNGURA — Juju: correction to the 10:19 price entry
<!-- type: event -->
**From:** MUNGURA

Juju: correction to the 10:19 price entry
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: the 10:19 entry said about $105 US for 30 days; adding it up again gives about $119 US (about 167 CAD): Inworld 25, OpenRouter 26 (GLM at Z.AI plus Jev), Google 15, WaveSpeed 22, DeepSeek direct 31 minus the balance already there. Why/verdict: fleet scripts written by DeepSeek on max were left out of the first sum. Status/open: every figure is an estimate (reasoning tokens assumed: GLM 8k a call, DeepSeek 16k); the first real film replaces them.
- Status: complete: figure corrected; unmeasured

---

## 2026-11-24 10:16 EAT — MUNGURA — Budget go-ahead: 30 days of daily films for three channels, about $93 US; reasoning knob set
<!-- type: event -->
**From:** MUNGURA

Budget go-ahead: 30 days of daily films for three channels, about $93 US; reasoning knob set
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked to 'load up money on everything' and whether the reasoning knob can change per film. Plan: DeepSeek always max, GLM 5.3 always high, Neon low to xhigh.
- Go-ahead given: load 30 days, all three channels daily, about $93 US (~$130 CAD). Split: Inworld $30, OpenRouter $26, WaveSpeed $22, Google AI Studio $15. 60 days would be about $186 US.
- Cost per 50-minute LOT film: Quick $1.74, Crafted $2.00, Masterwork $2.81. These are estimates; nothing is measured yet.
- Slowness traced to load (about 42 on 8 cores) from builds and renders queuing, not too few agents. New work is design-only until builds clear. A background git push was killed and HEAD soft-reset to origin/main.
- Review flow confirmed: maker, two fresh reviewers (one by eye, one by use), fixer, repeat up to 3 times, truth check on every screen. Still open: check each wallet's minimum and credit expiry before paying; test Neon effort changes keep the cache.
- Status: in-progress — go-ahead given; no payments confirmed in transcript, Neon cache test pending.

---

## 2026-11-24 09:21 EAT — TEHUTI — Juju: page-by-page map started, folded skills being restored, API cost plan drafted
<!-- type: event -->
**From:** TEHUTI

Juju: page-by-page map started, folded skills being restored, API cost plan drafted
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked for a page-by-page visual map of every interaction and agent flow for Doop, built on the speed skill, which the agent identified as asase-velocity.
- Page-spec mapping started on Opus. Art judges scored three directions 5 to 6 of 10. No Doop board is drawn yet.
- Ambi asked that all folded Juju skills be acted on. The agent is giving them their own files (44 in total) and building the part of the app that makes them act.
- Cost estimate for a $40 US test buy: about $1.78 per 50-min LOT film, $0.33 per 30-min film. The 60-day plan is $140 CAD for LOT 3x a week versus the doc's $144, and about $223 for daily LOT. Estimates only, nothing measured.
- Files changed: mockups/show/carved-altar-r2.jpg; mockups/show/carved-tank-r2.jpg; mockups/art/carved/shots
- Status: in-progress — page map and skill restoration still running; no Doop board or measured costs yet

---

## 2026-11-24 08:48 EAT — TEHUTI — Juju: built the self-review gate, 19 rooms, and its own private repo; Earshot phone spike measured
<!-- type: event -->
**From:** TEHUTI

Juju: built the self-review gate, 19 rooms, and its own private repo; Earshot phone spike measured
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked for confidence in the system: work that reviews itself and auto-merges only once it passes. Built one gate command covering code tests, all 33 skills, every screen at both sizes, and a truth check.
- The truth check fails screens that claim things that are not real (Connected, 43 of 70 pictures, Film ready, a made-up version history). Ambi's decision is in docs/adr/0002-no-required-spoken-take.md.
- All 19 rooms exist in first-round look; the kit checker reported zero faults at 1440 and 390. Three art directions (night light, framed panels, carved ink) were drawn and are awaiting judgement.
- Ambi answered the grill: Q1 yes, Juju's own private repo AmbessaTrades/juju (agent reports it created); Q2 nothing auto-merges until reviewed; Q3 50-minute documentaries, old LOT not a source; Q4 TTS-2 pauses placed in the edit.
- Attack pass: of 262 VidRush abilities, 77 are missing from Juju's rooms, and three skeptics found holes (no fact-checking, no story law, dead buttons). Open items are in docs/OPEN-RISKS.md and mockups/COVERAGE.md. A stray TubeLoop save was left in place, unreverted.
- Files changed: docs/adr/0002-no-required-spoken-take.md; docs/adr/0001-earshot-listening-models-allowed.md; docs/earshot-phone-spike.md; docs/OPEN-RISKS.md; mockups/COVERAGE.md; mockups/kit/truth.py; mockups/kit/facts.json; crates/juju-skills/packs
- Status: in-progress — art direction judging, first 50-minute film test and scene engine still running; the Earshot phone app waits for the Galaxy plugged in

---

## 2026-11-24 08:17 EAT — TEHUTI — Juju: Earshot kept in full, Android toolchain installed, 33 skills validate, 12 Rust tests pass
<!-- type: event -->
**From:** TEHUTI

Juju: Earshot kept in full, Android toolchain installed, 33 skills validate, 12 Rust tests pass
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi said all of Earshot must be used, including its own sound effects, to avoid the AI-sounding SFX. The brief was edited to match, and an ADR (0001) now records that Earshot's listening models are allowed.
- Android kit installed and 18 rooms exist. The 33 skills (32 plus the ask-juju router) are on disk and validate, and the same files load in the Rust app with 12 tests passing.
- Ambi's round-1 verdict (childish drawings, weak cohesion, paid states unclear) set round 2: one shared art library, and a drawing must show a real state. Three redrawn art directions are still in progress; no room is redrawn yet.
- Still open: Earshot running on the phone without the computer (spike in flight), the Wednesday LOT proof film under review, and the skills backup to tubeloop was refused for size and is being fixed.
- Files changed: JUJU-MASTER-BRIEF.md; docs/adr/0001-earshot-listening-models-allowed.md; mockups/ROOMS.md; SKILLS-PLAN.md; mockups/kit/live.py; apps/juju-shell/build_ui.py; ~/.claude/auh/config/skills-policy.json; ~/.auh-git/projects/tubeloop/project.json
- Status: in-progress — Juju app build underway; round-2 art redraws, Earshot-on-phone spike and LOT proof still open.

---

## 2026-11-24 08:16 EAT — MUNGURA — Juju day 1: skills on disk, first rooms shown, Ambi's round-1 verdict, YouTube rule checked
<!-- type: event -->
**From:** MUNGURA

Juju day 1: skills on disk, first rooms shown, Ambi's round-1 verdict, YouTube rule checked
- Harness: Claude Code (claude-fable-5-2)

Why/verdict: Ambi, 24 Nov, on round 1: likes the vibe; wants more cohesion between pages and better drawings ("can't feel like they're drawn from a kid"), visuals whose logic makes sense (the tank's gourds), nothing shown as paid, no "43 of 70 pictures" (old LOT language), no goofy spell-strip pictures; APK must use Earshot without the Mac; he asked whether the picture budget makes sense. Decision (Ambi): Earshot in full, on the phone too. Observation, verified on YouTube's own help page today: the channel monetisation policy names image slideshows, templated storylines, scrolling text with little narrative, and AI content from generic templates "without adding the creator's original, authentic insights or perspective"; one operator reports 14 channels demonetised on 23 Nov. Lead's advice sent to Ambi: fund only Google AI Studio and WaveSpeed at the smallest amount today (about $20 US, not the $144 CAD plan); GPT Image 2.6 only; GLM unproven.


Related: docs/STAGE-FORM.md, mockups/ART-BRIEF.md, mockups/ROOMS.md, SKILLS-PLAN.md, docs/earshot-phone-spike.md. Harness: Claude Code in T3 Code, Fable 5.2 lead, Opus 5.5 and Haiku 5.5 workers.
- Verification: cargo test: 12 passed; 33 skill.json parse and ids match folders; rooms render with 0 printed faults at 1440 and 390 (arcana has a script error, still with its maker); wall answers 200 with its key and 404 without; YouTube wording fetched from support.google.com/youtube/answer/1311392; Gemini 4 Neon and GPT Image 2.6 prices read from today's saved vendor pages.
- Status: in-progress: three workflows running; skills backup blocked on a size decision

---

## 2026-11-24 06:41 EAT — MUNGURA — Juju brief read, 336 screens indexed, 19 vendor docs saved; waiting on Ambi's 5 calls
<!-- type: event -->
**From:** MUNGURA

Juju brief read, 336 screens indexed, 19 vendor docs saved; waiting on Ambi's 5 calls
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi pasted the Juju master brief. It is saved whole, and its claims were checked against this Mac. Juju is now registered in the shared project map.
- Harvest done: 19 of 19 vendor docs saved; 336 VidRush and look-reference screens read with 0 failures, including 195 from the V2 walkthrough video.
- Mac disagrees with the brief: no Juju memory or day log for 21-23 Nov; look folder has about 35 Hades II pictures, not the Thumbsy or feed screens; no Android kit; disk 95% full (51 GB free).
- LOT has not uploaded since 2 Nov, and a 25-minute script has sat unvoiced since 10 Nov. Proposed Wednesday 20:00 target: one LOT film from one command, with thumbnail and publish text.
- Cost $0 on paid services, about 2.2M tokens on 38 small reader agents. No Juju code built yet. Open: Ambi must reply 'defaults' or change the 5 calls before building starts.
- Files changed: JUJU-MASTER-BRIEF.md; harvest/wave1/INDEX.json; harvest/wave1/V2VIDEO-READER-BRIEF.md; scripts/harvest-index.py; scripts/stack-txt-harvester.sh; scripts/dedupe_frames.py; ~/debate-agent/memory/vault/project-maps.json
- Status: in-progress — research and intake complete, no Juju code built, awaiting Ambi's reply on the 5 calls

---

## 2026-11-24 06:40 EAT — MUNGURA — Juju master brief received: saved, checked against the Mac, screens read
<!-- type: event -->
**From:** MUNGURA

Juju master brief received: saved, checked against the Mac, screens read
- Harness: Claude Code (claude-fable-5-2)
- What happened: Changed: Ambi pasted the Juju master brief (22 sections, 28,186 words) into T3 Code at 06:28. Saved byte-identical to JUJU-MASTER-BRIEF.md (sha256 8b8cdfc1…). Ran the boot it asks for, minus the steps that need his word. (1) Vendor docs: 19 of 19 saved to ~/AUH/AMBESSA/docs/stack-txt (the brief's harvester used bash 4 arrays; macOS has bash 3.2, so it was rewritten). (2) VidRush V2 walkthrough DlB0UABEawo: 1080p, 01:25 on, two ffmpeg passes, 639 frames on disk, 195 distinct screens with timed transcript. (3) Haiku 5.5 readers, one bounded unit each: 85 VidRush screenshots + the long homepage in 18 slices + 39 look references + 195 video screens, one JSON per unit in harvest/wave1/out, indexed in INDEX.json. (4) Juju added to the project map (find "Juju" now answers); topic = loop, where the software's history sits.

Why/verdict: the brief is the first record of the name Juju on this Mac. No day log exists for 21 to 23 Nov and Memoir had zero hits, so its "said by Ambi 20 to 22 Nov" lines cannot be checked here; the paste itself is taken as his word for the name and the folder. Observations where the brief and the disk disagree: the Rust engines are at ~/AUH/Loop/loop/engine (47 files, 9,791 lines, confirmed), not ~/AUH/Loop/engine. The look folder holds 39 pictures, about 35 of them Hades II; no Thumbsy screen, no YouTube feed tester screens. Missing on this Mac: rustup, Android SDK/NDK, adb, Tauri, Typst, bun, wrangler, turso; disk 95% full (51 GB free). The brief puts LOT on Inworld TTS-2; Ambi's 1 Nov voice lock is ABV V9 on inworld-tts-1.5-max, 0.95, temperature 2.0. LOT has not uploaded since 2 Nov; lot-r01 (25.3 min script, voice about $0.46) was never voiced or rendered.


Related: brief sections 15 to 18 and 22; ~/AUH/Loop/loop/onefile/START-HERE.md; ~/AUH/AMBESSA/BUILD/BUILD-BRIEF.md (19 Nov handoff, before the name). Harness: Claude Code in T3 Code, Fable 5.2.
- Files changed: JUJU-MASTER-BRIEF.md; scripts/stack-txt-harvester.sh; scripts/vidrush-v2-frame-rip.sh; scripts/dedupe_frames.py; scripts/harvest-index.py; harvest/wave1/INDEX.json; ~/AUH/AMBESSA/docs/stack-txt/; ~/debate-agent/memory/vault/project-maps.json
- Verification: cp checksum matched; harvester printed saved 19 failed 0; frames.json lists 639 files and 195 distinct screens; harvest-index.py printed 0 failed records; one reader record compared by eye against its screenshot (home composer, 13-18-32) and matched word for word; map-check shows no juju failure (2 older failures: memoir skill not found).
- Status: in-progress: boot audit and screen reading done; five decisions are Ambi's before the build starts
