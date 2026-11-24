# Juju now

As of 13:45 EAT, Tue 24 Nov 2026. Written every two hours by claude-haiku-5-5 (medium) from facts collected by code and the lead agent's own messages. Reports are not proof.

## Changed since the last sheet
- Paid calls in the test ledger: 1,188, $0.8778 (last sheet: 1,055, $0.7310). DeepSeek $0.4004, OpenRouter $0.2951, Google $0.1822.
- Direct Google key: the lead reports it works (13:42). This corrects the 13:21 report that only the OpenRouter route worked. The ledger shows 4 refused Google calls, last success 13:13.
- One spend meter now covers all paid tests, cap $2.25 for today (lead, 13:42). The ledger is at about 39% of it. The earlier $0.60 cap in one script is replaced.
- Mac load (1, 5, 15 min): 67, 60, 64 (last sheet: 45, 42, 61).
- Rust: 12,772 lines in 7 crates (last sheet: 12,109). Skills: 46 (last sheet: 44).
- Engine: 3 of 4 agents finished (last sheet: 2).
- Model measurements (lead, 13:42): DeepSeek on low thinking filled the film form validly 2 of 2 times. Thinking off was invalid. GLM low returned nothing for $0.06. Gemini cache: 0 of 3 repeats saved.
- Nuance test done (13:43): 21 of 24 risky instruction lines were misread by cheap models. 8 are fully cured on fresh material.
- Packaging test (13:46): 6 title and thumbnail packages drawn. The skill-ordered ranking got 48% of pairs right; random got 50%.
- ADR 0009 (quiet screens) accepted (13:00). ADR 0010 (20-minute plan) is a candidate.
- Ancient Logos teardown: silent since 13:14. The lead's 13:42 workflow includes a restart. Not reported running.
- Commits on main: none reported since e0115bd (10:33).

## App engine and films
- Engine: 3 of 4 finished. build:worlds running.
- Round 5 picture sheet (12:48): not scored by judges. Lead says it looks better than round 1. Earlier scores were 4 to 6 of 10.
- Subtitles and small labels are too wordy (12:48). Not confirmed fixed.
- Test render, 187 seconds (12:10): 1080p, 0 fallback scenes, safe-box check passed, no voice track, one act. A picture test, not a full film.
- Film reader: 0 of 1 finished. build:absorb running (tests, build, first clip).
- Design systems: 0 of 5 finished. Five teardowns running. No design-system library on disk.
- Milky Stellar teardown (lead, 13:17): 16 devices with times. Its job waits up to nine minutes for shared-lock jobs.
- Film cost (lead, 13:17): about $0.55 per 50-minute film on DeepSeek and $2.14 on GLM, at high or max thinking. Not shown to fit the budget.
- 20-minute plan (lead, 13:42): the lead's estimate says it fits. Voice is the tight part. Voice cost is not measured. Filling the film form is measured at about 5 cents per film.
- Freshness answer to the YouTube demonetisation wave (lead, 13:42): locked stance, voice and type; slow changes; new argument, opening, worlds and title per film; length 16 to 24 minutes. A sameness meter is planned, not built. The lead rejects random shuffling to fool a detector.

## Web app and rooms
- All 19 rooms have a first build. 4 of 8 room builders finished.
- Still running: crossroads, cauldron, conjuring, new-vessel.
- Cauldron: price overlaps the list on the phone screen (lead, 12:48). Round 6 renders running. No fix confirmed.
- Board (13:00): 329 room states at two sizes on one canvas. Desktop frames were empty at 12:48. A 13:00 log lists them as rendered. No judge check reported.
- Page map: board-fix was 12 of 13 finished, waiting for the final build and push. It is not in the 13:45 job list, so its end is not reported.
- ADR 0009: 30 interface words at desktop, 24 at phone, no text of 5 words or more, one 1 to 2 word status per object. Quiet-screen rules are in PR 3, open.
- Outside critics have not reviewed the rooms.

## Mac app and APK
- APK files built: 0. APK not tested.
- Mac app: nothing reported. Not tested.
- Earshot runs in full, phone included (Ambi, 08:16). Phone spike measured 08:48. No later result. build:voice is finding the Earshot model cache and running a check.
- Video work runs one job at a time (lead, 12:37). Load is still high.

## Agents running now
- Engine: build:worlds (3 of 4 finished)
- Conductor: fix:r2 (10 of 11 finished)
- Rooms: crossroads, cauldron, conjuring, new-vessel (4 of 8 finished)
- Film reader: build:absorb (0 of 1 finished)
- Design systems: five teardown jobs (0 of 5 finished)
- Guard, voice, 3D, PR loop: six jobs (0 of 6 finished): wave facts, PR review loop, one teardown, freshness build, money build, voice build
- Page map: board-fix, not in the 13:45 list

## Money spent on services
- Ledger: $0.8778 over 1,188 calls. Successful answers: DeepSeek 824 (1 refused or failed), OpenRouter 351 (1), Google 7 (4).
- Balances at 12:37 (lead): OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00. Not rechecked since.
- Google: billing linked; direct key works (lead, 13:42). Prepaid balance not in the facts.
- Inworld: key works, 403 stock voices (lead, 13:42; earlier 407). No charge seen. Making speech not tested.
- Budget: 135 CAD agreed (ADR 0008). The 10:52 split was Inworld 55, OpenRouter 23, DeepSeek 22, Google 21, WaveSpeed 14. Film costs above are not shown to fit.
- Gemini cache: 0 of 3 repeats saved (lead, 13:17; earlier figure of 5 corrected).
- Spend guard: one meter, cap $2.25 for today (13:42). The earlier worst case of $1.25 is superseded.

## Broken, blocked or open
- Engine drawing tests do not compile on main. PR 5 fixed the picture finder (26 of 26 pass). Lead says the main tests for juju-stage do not compile (13:42).
- PR 1 loosened the checks, so green status is partial. The 8 PRs were tested alone, not together. None merged.
- Conductor room list: a worker says two entries must be added, or the conductor refuses to start on its next build (13:41). Not reported done.
- Cauldron price overlap, board desktop frames, subtitles: not confirmed fixed.
- Art direction: not judged (earlier 5 to 6 of 10).
- Voice: no voice track. Inworld speech not tested.
- Film costs and the 20-minute plan: not measured end to end. Not shown to fit.
- Nuance: 6 new rules are written but no code enforces them. 3 repairs are better, not cured. 4 cannot be fixed by wording.
- Packaging: 4 of 6 packages are below the winners' median contrast, on hold. Foil is rated weak. The skill-ordered ranking did no better than random. The 90/70/50 rule could not be tested.
- Thinking level: the packaging flow runs with thinking off, which departs from ADR 0006. The lead found thinking off invalid for the film form.
- Full run from script to finished film on your keys: not tested.
- Repo: uncommitted changes (205 files at 12:10). ADRs 0008 and 0009 are untracked (13:00).
- Ancient Logos teardown: status unknown since 13:14.

## Waiting on Ambi
- No item is marked as waiting on Ambi at 13:42 or 13:45.
- ADR 0010 (20-minute plan) is a candidate. Acceptance not reported.
- Replacement 90/70/50 wording is a candidate for Ambi (packaging worker, 13:46).
- Standing advice (lead, 12:48): keep Inworld permissions on Read only.

## Counted by code

- Pull requests: 8 open, 0 merged, 0 closed
- Paid calls in the test ledger: 1188, $0.8778 in all {deepseek: 0.4004, openrouter: 0.2951, google: 0.1822}
- Paid services answering: deepseek 824 ok, 1 refused or failed, last ok 24 Nov 13:43 EAT; openrouter 351 ok, 1 refused or failed, last ok 24 Nov 13:40 EAT; google 7 ok, 4 refused or failed, last ok 24 Nov 13:13 EAT
- Rust: 12,772 lines in 7 crates. Skills: 46. Rooms drawn: 19. Decisions: 9. APK files built: 0
- Design-system libraries on disk: none yet
- Mac load (1, 5, 15 min): [67, 60, 64]
- Job Engine: 3 of 4 agents finished; running: build:worlds (Bash)
- Job Conductor: 10 of 11 agents finished; running: fix:r2 (Bash)
- Job Rooms: 4 of 8 agents finished; running: rooms:crossroads+2 (Wait for full run a third time); rooms:cauldron+2 (Wait again for round 6 renders); rooms:conjuring+2 (Read the spell strip and publish kit sweep); rooms:new-vessel+3 (Wait for round five and truth output)
- Job Film reader: 0 of 1 agents finished; running: build:absorb (Wait for tests, build and the first clip)
- Job Design systems: 0 of 5 agents finished; running: teardown:ZgpMtombn9A (Correct the median and recheck queues); teardown:sJiaWNxYFUA (); teardown:oRBu7wYuOSo (Wait for frames); teardown:G4w-a8NgnnQ (Wait for caption fallback or Earshot); teardown:HmuQoak_IAg (Summarise all Earshot windows)
- Job Guard, voice, 3D, PR loop: 0 of 6 agents finished; running: facts:wave (List daily snapshots May-Aug 2026); pr-loop:build (See PR 5's gate.yml change); teardown:sJiaWNxYFUA (again) (Read the OCR function and find a Python with Vision); build:fresh (Check time, FACTS.md, load); build:money (Read Gemini Neon pricing section); build:voice (Find Earshot model cache and run doctor)
