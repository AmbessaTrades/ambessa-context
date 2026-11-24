# Juju day log, newest first

Rebuilt 13:45 EAT, Tue 24 Nov 2026. Only entries whose title names Juju. Times are EAT (UTC+3). Logged by agents: evidence of what they report, not proof. Where two entries disagree, the later one wins and the older stays.

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

**Changed.** `mockups/board/doop-blueprint.json`: canvas kKomk5DFWY, page aqrMl1XPQB, 658 frames = 329 room-states × two sizes (@1440 329, @390 329) over 19 rooms (altar, arcana, canopy, cauldron, conjuring, crossroads, feed-sight, gate, mirror-bend, new-vessel, offering, pact, publish-kit, reliquary, sound, spell-strip, tank, vessel, voice), `wired` 9,784, prototype_url http://localhost:4300/c/kKomk5DFWY/proto (returns 200). Pages rendered 12:54–12:57: 12 desktop `journey-*.png`, `board-desktop.png` (3.4 MB), `board-all.png` (7.9 MB), `phone/` 201 files, `_look/` contact sheets, builder `build.py` (81 KB). `docs/adr/0009-quiet-screens-quiet-frames.md` accepted for app screens on Ambi's words of 24 Nov ("stop writing subtext everywhere"): 30 interface words at 1440 px, 24 at 390 px, no text of 5 words or more, one 1–2 word status per object, faults starting `QUIET` in `mockups/kit/shot.py`; the film half is a candidate. Round-2 re-shoot: `mockups/r2/shots` 759 files, 726 newer than 11:25; pact, conjuring, publish-kit, spell-strip re-shot 13:13–13:16 with true empty states (`nothing-to-copy-today`, `no-loadout-built-today`).

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
- What happened: Changed: (1) 33 Juju skills (32 + router) written once at ~/.hermes/skills/juju, each SKILL.md + skill.json; the app embeds the same folder (crates/juju-skills, 4 tests) and juju-core loads a channel pack and a word clock (8 tests). (2) Android kit, Earshot with its listening models, Doop, bun and Tauri CLI installed inside .toolchain only. (3) 19 rooms mocked in two passes with a shared kit, a fault checker, and a live wall on the home network (mockups/kit/live.py, port 4600, private link). (4) An 85 second $0 proof cut of lot-r01 at runs/lot-r01-proof. (5) Brief edited on Ambi's word: all of Earshot is used and its listening models are the one exception to the no-local-weights ban (ADR 0001); the pasted original is kept beside it.

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
