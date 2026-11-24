# Juju now

As of 13:25 EAT, Tue 24 Nov 2026. Written every two hours by claude-haiku-5-5 (medium) from facts collected by code and the lead agent's own messages. Reports are not proof.

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

## Counted by code

- Pull requests: 8 open, 0 merged, 0 closed
- Paid calls in the test ledger: 940, $0.6548 in all {deepseek: 0.2627, openrouter: 0.2098, google: 0.1822}
- Rust: 11,670 lines in 7 crates. Skills: 44. Rooms drawn: 19. Decisions: 9. APK files built: 0
- Design-system libraries on disk: none yet
- Mac load (1, 5, 15 min): [36, 43, 75]
- Job Engine: 2 of 4 agents finished; running: build:worlds (Bash); build:speed (Bash)
- Job Conductor: 10 of 11 agents finished; running: fix:r2 (Bash)
- Job Rooms: 3 of 8 agents finished; running: rooms:altar+2 (Wait for the final batch and show truth lines); rooms:crossroads+2 (Wait for full run a third time); rooms:cauldron+2 (Patch look undo and wait for renders); rooms:conjuring+2 (Collect faults from the sweep); rooms:new-vessel+3 (Wait for interaction renders)
- Job Film reader: 0 of 1 agents finished; running: build:absorb (Wait for tests and build, third window)
- Job Design systems: 0 of 5 agents finished; running: teardown:ZgpMtombn9A (Wait for bursts; show queue); teardown:sJiaWNxYFUA (); teardown:oRBu7wYuOSo (Wait for frames); teardown:G4w-a8NgnnQ (Count distinct hedge footnotes and headers on code cards); teardown:HmuQoak_IAg (Wait for dates to finish)
- Job Page map: 12 of 13 agents finished; running: board-fix (Show where the placed ways out went, then start the final picture build and Doop push)
- Job Keys and PRs: 3 of 3 agents finished; none running
