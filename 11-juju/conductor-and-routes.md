# Juju conductor, its critics, the paid-route proof, and the taste scout

As of 13:10 EAT, 24 Nov 2026. Source: workflows a workflow (conductor build, two attack rounds, fix round), a workflow (paid routes), a workflow (YouTube-taste scout).

> **Read with this:** the second attack round was still running at 13:10. Google billing was linked at 13:10 and Gemini answers directly since; lines below that say Google refuses or that billing waits on Ambi are out of date. Its cache was then tested and saved nothing in three repeats. Money lines are in `money-and-stack.md`.

## In short
- Built `crates/juju-conduct`, the runtime that makes each skill of a stage act: make, check, critique, repair, learn. Every stage ends in PASS or HOLD, with a receipt.
- Worked on Mock providers only: a good film passed all 11 stages in 37 calls. A forced crash at act 4 resumed to PASS.
- Broke: attack round one found blockers that let a forged script pass, let blind critics pass a film, and let spend run past the fuse. The fix round reports fixes for those. Attack round two re-hit several.
- Paid routes: DeepSeek, GLM 5.3 and Neon through OpenRouter each returned a valid 60-second form. Direct Google calls were refused. Spend was $0.0926 of a $0.60 cap.
- Open: the Atticus King study itself (not in this file), the Neon cache question, critic recall, and most round-two blockers.

## What was done
**Conductor.** The 11 stages are typed data. 38 of 44 skills are reached through a typed "when" row; 6 are builder-only, each with a reason. Stages 5 and 6 may run together. Each stage runs the same loop:
- MAKE: one call carrying only the matched skills' positive fragments.
- CHECK: 104 checks in code run against 86 of the 234 gates in force, plus juju-script lint, claims, story and newthing.
- CRITIQUE: three lenses, each asked a different question. Critics get no maker prompt or thinking.
- REPAIR: only the failing part or sentences, at most 2 times. A quote a critic flagged must change.
- Then PASS, or HOLD with one reason and one way out. Gates without code are listed as not enforced.

PASS can only come from `Receipt::seal`, which refuses when a required skill is missing or a rule is unaccounted for. Critic and person defects go to a candidate file. A candidate becomes a diff only if it catches its own example and stays silent on a clean set. Nothing writes to a skill file. The provider has one Mock implementation. The fuse reserves each call's worst price before sending.

**Five scenario runs** on harbour-log, an invented test channel (nothing from LOT):
- Good: PASS, 37 calls, 57.29 s before render against a 90 s budget.
- Weak model: HOLD after stages 0 to 3, on an invented quote in act 3. Broken JSON in act 1 was re-asked alone and recovered.
- Slow provider: PASS at 98.13 s, with three overruns.
- Fuse: HOLD at stage 6, with $0.747 of the $0.75 test fuse already spent or promised.
- Crash: exit 70 at act 4. Resume gave PASS on attempt 2 and kept the four finished acts.

**Fix round.** It reports 127 tests passing, up from 80. It says it closed all 4 blockers and 19 important findings from round one. 

**Paid route proof.** One 60-second form job (same bytes) went to three routes, plus probes. The maker reports that the OpenRouter account moved by exactly the ledger's sum, and the DeepSeek account agrees to the cent.
- Google direct: all 4 calls to gemini-4-neon were refused with 429 (free-tier quota limit 0). Nothing was charged. The Google project's billing must be linked before the Neon cache or thinking level can be tested.
- DeepSeek: JSON mode worked at off, low, high and max (4 of 4). Its first form reply was blank (ceiling too low); it was sent again.
- GLM 5.3 via OpenRouter: 200 on 5 of 5. The default route was not the listed price; it went to Together, then InferenceNet. Pinning mattered: Wafer at fp4 cost $0.000028 for the same question, against $0.000106 at Z.AI fp8. No seller lists precision above fp8.
- Money: 92 to 98 percent of output is thinking. Scaled to 50 minutes (an assumption, not measured), a film costs about $0.55 to $2.86 by route. ADR 0006 had guessed $2.00.

**Taste scout and Atticus King.** The scout pulled recommendations 5 times, then read 120 subscriptions and the top outliers of 12 channels: 266 videos. It dropped 8 (short clips, a mix, compilations, game play), leaving 258 thumbnails on 14 contact sheets, all viewed. It picked 28 films:
- 3 map films (cap 4): Atticus King, Ethos, Battle Blueprint. 0 group-chat films (cap 2). 8 inner-life films, each in a different style. 13 films of 30 minutes or more, not counting two sleep pieces.
- Both required films are in: Atticus King J0wWNytEXS4 and Bygone Philosophy IEWMpPs0M-M.
- Looks were judged from thumbnail and title only. No video was downloaded. Views were read for 27 of 28 picks. About a third of the subscription picks are one to two days old, so their views do not yet show whether they work.

The Atticus King pick is 13 minutes long. The owner named it (ADR 0008) to study its editing, audio and pacing. The scout's read is a hand-drawn sketch map on paper, not a game map. This file has no study of its editing, audio or pacing. Result: unknown.

## Breakthroughs
- The full path runs on Mock answers: 11 stages, 105 gates passed, 0 failing. The maker reports 57.29 s before render against a 90 s budget, using assumed Mock latencies. Measured, Mock.
- A crash at act 4 resumed to PASS and kept four finished acts. Attack round one had shown the same resume paying twice for settled replies. The fix round says replies are now saved as they settle. Measured, Mock.
- Three routes returned a valid form for the same act 1 bytes: DeepSeek ($0.0110, 88 s), GLM ($0.0428, 171 s, valid first time) and Neon via OpenRouter Flex ($0.0286, 27 s). The checker accepts form shape only (see critics). Measured, one job each.
- Jev 1.14 is reachable with the OpenRouter account at $0.042 per million. One 512 px picture with two questions cost $0.000047. It scored a right brief 2.24 of 3 and a wrong one 0.52. Judged, two calls only.

## What critics found
Findings from the two attack rounds on the conductor. "Fixed" means the fix round reports a fix; the fix round is not re-run in this file. Where round two re-hit a finding, it is marked open.

1. **Blocker: required skill skipped when its flag is missing.** A donor transcript copied word for word gave PASS, with root-bending on no receipt (probe exit 0, PASS). Fixed per fix round: donor fields now set the flag. Round two re-hit it via the BEND badge, which nothing reads. Open.
2. **Blocker: resume trusts finished stages.** The stage hash has no key. A forged line was appended, the hashes recomputed, and the film passed with the healer receipt. The same text in a fresh run held. Fixed per fix round (checks re-run on resume). Round two: receipts are still trusted unsealed, and wiping every skill from receipts still passed with zero skills applied. Open.
3. **Blocker: thread start delay became a permanent HOLD.** A good film scaled to 50 ms held in 3 of 3 solo runs; act 5 started 16 ms after act 1 ended. Seven of 8 concurrent runs held. Resume never cleared it. Unknown: the fix round does not name this gate.
4. **Blocker: the fuse hold's way out broke resume.** Raising the fuse from $0.75 to $1.00 changed the stage input hash, so stages passed went from [0,1,2,3] to []. Fixed per fix round (fuse amount left out of stage hashes).
5. **Fuse per folder.** Nine fresh folders spent $1.889424 against a $0.75 fuse, and none was refused. Fixed per fix round (per-machine ledger with a file lock).
6. **Two processes on one run folder.** Three of four trials crossed $0.75 (ledger plus prior: 0.7697, 0.782, 0.8596). Fixed per fix round (folder lock).
7. **Paid replies not saved until a part passed.** In a kill loop, each act's make call settled 11 times, costing $0.411686 against $0.21 for a clean run. Fixed per fix round (replies saved as they settle).
8. **Stage 7 render gates passed on self-reports.** A render with no file passed "every act under 580 MB". Fixed per fix round: a new Unproven class holds on a reported failure but never counts as passed.
9. **Critics shown few or no rules.** In the good film, the eye, picture and buyer lenses were shown zero rules; ear and fact saw one each. Round two confirmed it. Open.
10. **A learned regex was promoted.** A critic's one-word pattern, tide, was promoted on a three-sentence clean set, then flagged a good line. Unknown: the fix round does not name the learn trial.
11. **Outline size bought the acts.** A 40-movement outline led to 40 paid act calls; acts_min 4 and acts_max 8 were read nowhere. Fixed per fix round (count check 4 to 8).
12. **Maker text reached critics unfenced.** A planted reviewer note sealed into the script, and the mock critics gave PASS. Round two: a fake fence marker split the fence, and the marker was sealed. Open.
13. **Blind critics pass the film.** An empty defects list from every lens still gave PASS on all 11 stages, and the recall score is never called by run. Open.
14. **One quote judges many rules.** The quote "the tide gauge at Port Selwyn" marked five shown rules judged; "the Harbour Wall" judged four. Only a three-word minimum was added. Open.
15. **Crown-weight passes a junk title.** Title "zzqx" with an invented equation id still passed. The fix round added KG1 to KG5 checks; round two's probe still passed. Open.
16. **Hollow outline passes crossroads.** Every movement's event, friction, actor and echo read "stone", with cold open at 1 s, and R1, R3 and R4 still passed. The receipt records these as Pass, not Unproven. Open.
17. **Skill-folder edits erase obligations.** A gate prefixed with "At render," vanished from every receipt. A skill with all 14 rules turned into prompts, and the fragment "Go.", passed. Open.
18. **Form check passes without juju-stage.** Fixed per fix round: missing juju-stage now holds stage 6 unless --no-form-tool is given. Round two: with juju-stage present, the harbour-log good film fails, because its stage pack names a world absent from the catalog. Open.
19. **Gate counts disagree.** One probe counted 261 gates, another 262. Of 86 coded gates, 66 ran in the good film. The receipt's "judged" label overstates enforcement. Open.
20. **Route checker hole.** GLM and DeepSeek both placed Republic page 323 under a line not on that page, and the checker passed it. Open.

## Numbers
| Measure | Value | Basis |
|---|---|---|
| Gates in skill files | 261 or 262 (two counts) | Measured |
| Gates with code / listed not enforced | 86 / 148 (plan: 234 in force) | Measured |
| Coded gates that ran in the good film | 66 of 86 | Measured |
| Conductor tests | 80, then 127 after fix; 28 attack tests failed on old code | Measured |
| Good film | 11 stages, 37 calls, 105 gates passed | Measured, Mock |
| Good film before render | 57.29 s against 90 s | Measured, Mock timing |
| Nine folders, one fuse | $1.889424 against $0.75 | Measured, Mock |
| Kill loop | 11 settles per act, $0.411686 against $0.21 | Measured, exaggerated scale |
| Two processes, one folder | 3 of 4 crossed $0.75 | Measured |
| Route spend | $0.0926 of $0.60 | Measured |
| DeepSeek small call | about $0.0004 at peak | Measured |
| DeepSeek cache hits | 896 of 1,151 eight seconds apart; 0 one second apart | Measured |
| GLM at Wafer fp4 against Z.AI fp8 | $0.000028 against $0.000106 | Measured |
| DeepSeek form job | 18,228 out (17,937 thinking), $0.0110, 88 s | Measured |
| GLM form job | 11,771 out, $0.0428, 171 s | Measured |
| Neon form job via OpenRouter Flex | 2,794 out, $0.0286, 27 s | Measured |
| Jev 1.14 | $0.042 per million; $0.000047 per picture; 2.24 of 3 and 0.52 | Price Measured; scores Judged, two calls |
| 50-minute film, by route | DeepSeek $0.55 off-peak, $1.10 peak; GLM $2.14 unpinned, about $0.84 at Wafer; Neon $1.43 Flex, $2.86 Standard | Estimated (scaled) |
| Scout pool | 5 pulls; 266 videos; 8 dropped; 258 thumbnails on 14 sheets | Measured |
| Scout picks | 28; 3 map, 0 group-chat, 8 inner-life, 13 long | Measured counts |

## Still open
- The Atticus King study: editing, audio and pacing are not in this file. Unknown.
- Neon: link billing on the Google project, then run the cache and thinking-level probe (about 2 cents). Ambi is the one to link it.
- Round-two blockers: resume trusting unsealed receipts, the critic fence, and blind critics. The conductor cannot yet show that a critic finds a planted defect.
- Stage 2 holds for a person's tap, while ADR 0002 says no per-film human input is required. Whether a person must watch before publish is also open.
- Root bending for uploads 1 to 12 is unresolved. Ambi decides.
- The default spend ledger refuses roughly the fourth mock film per machine. Ambi decides whether that stays.
- WaveSpeed's API shows 12 for its image count; the owner said 10. Unresolved. The image listing itself ($0.027 low, $0.045 medium at 1k) is a listed price, with no call made.
- The 50-minute costs are assumed, not measured. Not measured: DeepSeek on low and max for the form job, spans over 60 s, and Jev on human picks or larger pictures.
