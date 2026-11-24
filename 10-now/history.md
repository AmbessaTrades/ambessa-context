# Every sheet, newest first

The last 84 two-hour sheets. Older ones are in the git history of this file.

---

# Sheet of 13:45 EAT, Tue 24 Nov 2026

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

# Sheet of 13:32 EAT, Tue 24 Nov 2026

## Changed since the last sheet
- Paid calls in the test ledger: 1,055, $0.7310 in all (last sheet: 940, $0.6548). Split: DeepSeek $0.317, OpenRouter $0.2317, Google $0.1822.
- Rooms: 4 of 8 builders finished now (last sheet: 3). The altar room finished.
- Mac load (1, 5, 15 min): 45, 42, 61 (last sheet: 36, 43, 75).
- Rust code: 12,109 lines in 7 crates (last sheet: 11,670).
- The lead reports a model test on one film form (13:21): GLM 5.3 high $0.0428, Neon low $0.0286, DeepSeek high $0.0080.
- Conflict, not resolved: the lead's 13:17 message says Gemini works. The 13:21 day log says direct Neon calls still get 429 and only the OpenRouter route works.
- ADR 0009 (quiet screens) is accepted (lead, 13:00).
- Ancient Logos teardown: silent since 13:14 (lead). The lead plans to check at 13:33.
- Commits on main: no new ones. Latest is e0115bd (10:33).

## App engine and films
- Engine: 2 of 4 agents finished. Running: build:worlds and build:speed.
- The lead reports 9 world kinds drawn and 112 licensed pictures gathered (12:48).
- Round 5 picture sheet (12:48): not scored by judges. The lead says it looks better than round 1. Earlier scores were about 4 to 6 out of 10.
- The lead reports subtitles and small labels are too wordy (12:48). Not confirmed fixed.
- Test render, 187 seconds (12:10): 1080p, 0 fallback scenes, safe-box check passed, no voice track, one act only. It is a picture test, not a full film.
- Film reader: 0 of 1 finished. build:absorb is running. The lead reports it is still building (12:48).
- Design systems: 0 of 5 finished. Five teardown jobs are running. No design-system library exists on disk.
- The lead shared a Milky Stellar teardown with 16 devices and times (13:17). Its job waits up to nine minutes for shared-lock jobs (facts, 13:32).
- Film cost estimates (lead, 13:17): about $0.55 per 50-minute film on DeepSeek and $2.14 on GLM, at high or max thinking. The lead says 92 to 98% of output is hidden thinking. These are not shown to fit the budget. The next test uses lower thinking and longer stretches per call.

## Web app and rooms
- All 19 rooms have a first build. 4 of 8 room builders are finished.
- Still running: crossroads, cauldron, conjuring, new-vessel.
- Cauldron: the lead reports a price overlapping the list on the phone screen (12:48). The round 6 renders are running. No fix is confirmed.
- Board (13:00): 329 room states at two sizes on one canvas.
- Page map: 12 of 13 finished. board-fix is still running and waiting for the final build and push.
- Desktop frames on the board were empty (lead, 12:48). Not confirmed fixed.
- ADR 0009: 30 interface words at desktop, 24 at phone, no text of 5 words or more, one 1 to 2 word status per object.
- Quiet-screen rules are in PR 3, which is open, not merged.
- Outside critics have not reviewed the rooms (lead, 12:48).

## Mac app and APK
- APK files built: 0. APK not tested.
- Mac app: nothing reported in the facts. Not tested.
- Earshot runs in full, including on the phone (Ambi's decision, 08:16). The phone spike was measured at 08:48. No later result is reported.
- Video work runs one job at a time to protect the Mac (lead, 12:37).

## Agents running now
- Engine: build:worlds, build:speed (2 of 4 finished)
- Conductor: fix:r2 (10 of 11 finished)
- Rooms: crossroads, cauldron, conjuring, new-vessel (4 of 8 finished)
- Film reader: build:absorb (0 of 1 finished)
- Design systems: five teardown jobs (0 of 5 finished)
- Page map: board-fix (12 of 13 finished)
- Keys and PRs: none running (3 of 3 finished)
- The lead reports nuance, storyboard and packaging test jobs. Nuance and packaging have ledger calls (13:21). Storyboard has not been reported since. None are in the job list.

## Money spent on services
- Ledger: $0.7310 across 1,055 paid calls (split above).
- Balances at 12:37 (lead): OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00. Ambi's note said $10 for WaveSpeed. Not rechecked since.
- Google: billing linked and the first paid call worked at 13:10 (lead). The prepaid balance is not in the facts.
- Inworld: key works, 407 voices listed, no charge. Making speech is not tested.
- Budget: 135 CAD agreed (ADR 0008). The film costs above are not shown to fit it.
- Gemini cache: 3 repeat calls saved nothing (lead corrected its earlier figure of 5). The paid cache and batch route are not tested.
- Spend guard: each job has its own limit. A shared lock now exists (teardown jobs wait on it). The lead has not reported a total-limit test. Worst case if all jobs hit their limits: $1.25 (lead, 13:21).

## Broken, blocked or open
- Engine drawing tests do not compile on main. PR 5 fixed the picture finder (26 of 26 pass). The drawing part is still red.
- PR 1 loosened the checks, so green status is partial. The 8 PRs were tested alone, not together. None are merged.
- Cauldron price overlap: not confirmed fixed.
- Board desktop frames: not confirmed fixed.
- Art direction: not judged.
- Engine subtitles and labels: too wordy, not confirmed fixed.
- Voice: no voice track. Inworld speech is not tested.
- Film costs: not shown to fit the budget.
- Gemini: direct-route status conflicts (see above).
- Full run from script to finished film on your keys: not tested.
- Repo: uncommitted changes (lead's count at 12:10: 205 files). ADRs 0008 and 0009 are untracked.
- Ancient Logos teardown: status unknown since 13:14.

## Waiting on Ambi
- Nothing is reported as waiting on Ambi (lead, 13:21).
- The Google billing step asked for at 13:07 is done. The first paid call worked at 13:10.
- Standing advice (lead, 12:48): keep Inworld permissions on Read only.


# Sheet of 13:27 EAT, Tue 24 Nov 2026

## Changed since the last sheet
- Paid calls rose from 940 to 991. Spend rose from $0.6548 to $0.6938.
- Mac load (1, 5, 15 min) went from [36, 43, 75] to [35, 41, 69].
- Several running tasks have new notes. Details are in the agent sections below.
- Newest commit on main: e0115bd, 24 Nov 10:33, "Decision: the software first, no channel drives the build."
- Pull requests, Rust size, skills, rooms drawn, decisions, APK count and design-system libraries: No change reported.

## App engine and films
- Job Engine: 2 of 4 agents finished. Running: build:worlds and build:speed, both Bash.
- Skills: 44. Decisions: 9.
- Commit 05d3a20 (24 Nov 09:20) reports stage engine test 1. Cheap-model films scored about 4 of 10. This is from the commit message, not a test shown in FACTS.
- Commit 3e91606 records the decision that LOT is 50-minute documentaries and old LOT is not a source.
- Film reader: 0 of 1 agents finished. Running: build:absorb. Its note now reads "Keep waiting and view the queue." Before, it read "Wait for tests and build, third window."
- Pull request #7, the sample film the rooms are drawn from, is open with checks SUCCESS.

## Web app and rooms
- No web app facts were reported.
- Rooms drawn: 19.
- Job Rooms: 3 of 8 agents finished. Five are running:
  - rooms:altar+2. Note changed to "Wait for truth on the final files."
  - rooms:crossroads+2. "Wait for full run a third time."
  - rooms:cauldron+2. "Patch look undo and wait for renders."
  - rooms:conjuring+2. "Collect faults from the sweep."
  - rooms:new-vessel+3. "Wait for interaction renders."

## Mac app and APK
- APK files built: 0.
- Mac load now [35, 41, 69]. It was [36, 43, 75].
- No Mac app facts were reported. Not tested.

## Agents running now
- Job Engine: build:worlds, build:speed (2 of 4 finished).
- Job Conductor: fix:r2 (10 of 11 finished).
- Job Rooms: five running, listed above (3 of 8 finished).
- Job Film reader: build:absorb (0 of 1 finished).
- Job Design systems: five teardown tasks running (0 of 5 finished). Notes:
  - teardown:ZgpMtombn9A: "Wait for bursts; show queue."
  - teardown:sJiaWNxYFUA: no note.
  - teardown:oRBu7wYuOSo: "Wait for frames."
  - teardown:G4w-a8NgnnQ: changed to "Wait up to nine minutes for lock jobs." Before, it was "Count distinct hedge footnotes and headers on code cards."
  - teardown:HmuQoak_IAg: "Wait for dates to finish."
- Job Page map: board-fix running (12 of 13 finished). Note changed to "Wait for the final build and push." Before, it was "Show where the placed ways out went, then start the final picture build and Doop push."
- Job Keys and PRs: 3 of 3 finished. None running.

## Money spent on services
- Paid calls in the test ledger: 991. Total $0.6938.
- deepseek $0.2899 (was $0.2627). openrouter $0.2217 (was $0.2098). google $0.1822 (no change).
- Wallet balances: not reported.

## Broken, blocked or open
- Design-system libraries: none on disk yet.
- Film reader and Design systems jobs are still running with no finished agents.
- Cheap-model film score about 4 of 10 (from commit 05d3a20). Newer tests not shown.
- Rooms still waiting on final truth files, a look patch, fault collection and interaction renders.
- Pull requests: 8 open, 0 merged, 0 closed. All checks SUCCESS.
- Lead has sent no messages and no day log entries.

## Waiting on Ambi
- No request to Ambi is stated in the messages or facts.



# Sheet of 13:25 EAT, Tue 24 Nov 2026

## Changed since the last sheet
The last sheet had no facts, so everything here is new.
- The test ledger shows 940 paid calls and $0.6548 spent.
- The lead's earlier spend figures ($0.44 at 13:17, $0.51 at 13:21) are superseded by the ledger.
- Google's direct key answers now. The lead reports billing was linked and the first paid call worked at 13:10. Earlier 429 refusals (12:51) are superseded.
- Eight pull requests are open, none merged. The lead corrected its "all checks green" claim at 13:21.
- All 19 rooms have a first build (ledger count). The lead's ADR 0009 on quiet screens is accepted.
- Mac load is now 36 (1 min), 43 (5 min), 75 (15 min). The lead reported 233 earlier.

## App engine and films
- Engine: 2 of 4 agents finished. Running: build:worlds and build:speed.
- The lead reports 9 world kinds drawn and 112 licensed pictures gathered (12:48).
- The lead's round 5 picture sheet is not yet scored by judges. Earlier scores were about 4 to 6 out of 10.
- A 187-second test render (12:10) had no fallback scenes and passed the safe-box check. It has no voice track and is one act only.
- Design systems: 0 of 5 agents finished. The five-film teardowns are still running. No design-system library exists yet.
- Film reader: 0 of 1 finished. build:absorb is running. The lead reports it is still building.

## Web app and rooms
- Rooms: 3 of 8 agents finished. Still running: altar, crossroads, cauldron, conjuring, new-vessel.
- The lead reports a price overlapping the list on the Cauldron phone screen (12:48). No fix is confirmed.
- The board (13:00) maps 329 room states at two sizes. The page map job is 12 of 13 finished, with board-fix still running. The desktop frames were empty earlier. A fix is not confirmed.
- ADR 0009 limits screens to 30 interface words on desktop and 24 on phone, with no text of 5 words or more.
- Outside critics have not reviewed the rooms yet (lead, 12:48).

## Mac app and APK
- APK files built: 0. APK not tested.
- Mac app: No change reported.
- The lead reports video work now runs one job at a time to protect the Mac (12:37).

## Agents running now
- Engine: build:worlds, build:speed (2 of 4 finished)
- Conductor: fix:r2 (10 of 11 finished)
- Rooms: five running, 3 of 8 finished
- Film reader: build:absorb (0 of 1 finished)
- Design systems: five teardown agents running, 0 of 5 finished
- Page map: board-fix (12 of 13 finished)
- Keys and PRs: none running (3 of 3 finished)
- The lead reports three test jobs (nuance, storyboard, packaging). They are not in the job list.
- The lead reports the Ancient Logos teardown has been silent since 13:14. Its status is unknown; the lead plans to check at 13:33.

## Money spent on services
- Ledger total: $0.6548 across 940 paid calls. DeepSeek $0.2627, OpenRouter $0.2098, Google $0.1822.
- Balances at 12:37 (lead): OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00. Not rechecked since.
- Inworld: key works, 407 voices listed, no charge. Making speech is not tested.
- Film cost estimates from 13:17: about $0.55 per 50-minute film on DeepSeek, $2.14 on GLM, at high or max thinking. The lead says 92 to 98% of output is hidden thinking. The lead says these are not yet shown to fit the agreed budget (13:21).
- Gemini cache: three repeat calls saved nothing. The lead corrected its earlier figure of five. The paid cache and batch route are not tested.
- Spend guard: each job has its own limit. No shared total limit exists yet. Worst case if all jobs hit their limits: $1.25 (lead, 13:21).

## Broken, blocked or open
- Engine drawing tests do not compile on main. PR 5 fixed the picture finder (26 of 26 pass). The drawing part is still red.
- PR 1 loosened checks, so green status is partial. PRs were tested alone, not together. Not merged.
- No shared spend limit yet.
- Ancient Logos teardown: status unknown since 13:14.
- Cauldron price overlap: not confirmed fixed.
- Board desktop frames: not confirmed fixed.
- Art direction: not judged.
- Voice: no voice track. Inworld speech is not tested.
- Film costs: not shown to fit the budget.
- Full run, script to finished film, on your keys: not tested.
- Repo: uncommitted changes exist (lead's count at 12:10: 205 files). ADRs 0008 and 0009 are untracked.

## Waiting on Ambi
Nothing is waiting on you (lead, 13:21).
