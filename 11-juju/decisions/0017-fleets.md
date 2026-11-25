# 0017 Five fleets, one owner each

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

**Status:** Ambi's order, 24 Nov about 16:25 ("while one fleet is testing, the others should be doing the vids and design
systems, 50 and 10 minutes all the way to completion [...] the third refining script human logic, storyboarding [...] a
whole anti AI slop fleet [...] another PR fleet [...] you're not orchestrating well, take the initiative"). The split is the lead's.

| Fleet | Owns | Done when |
|---|---|---|
| App | `crates/juju-serve`, `mockups/r2`, `apps/` | every control on every room does a real thing on a real server, pressed at phone and desk size, 0 dead, 0 layout faults |
| Films | `crates/juju-stage`, `runs/films` | a 10 and a 50 minute film finished, voiced, mastered, inside 60 and 90 minutes of machine time |
| Story | `runs/character`, `runs/expand`, `runs/atlas`, script packs | cheap models write the arc; the lead reads and it has character |
| Slop | `runs/slop` (reads everything, edits nothing) | its open blockers are zero |
| PRs | worktrees only | one branch, whole workspace green, every finding answered |

Rules between fleets: nobody edits another fleet's folder; a fleet reads `runs/slop/<its name>.md` before it calls
anything finished; nothing reaches Ambi before the lead has used it himself.

**Truth recorded the same hour.** The app rooms were static pages: no room called any program (0 fetches in 19 rooms).
The lead let them be shown as the app. They had never been pressed end to end by the lead. WaveSpeed has never been used.

## Added 16:50 (lead): the order of work, after Ambi asked why the plan in the .md was not the plan being run

Cause, plainly: the brief's section 15.1 (11 stages) and 17.3 (one command, no Claude, a 60 second film) define a chain.
Work went into parts, studies and pictures before that chain existed, so nothing could be tested whole. From now:
1. **The chain first.** `crates/juju-cli` (`juju smoke-test`) runs all 11 stages; a missing one says NOT BUILT. Its
   scoreboard (`runs/spine/score.json`, shown in the Workshop) is the only progress report.
2. **Work in hand is capped.** No new fleet starts until a stage turns from red. A fleet's work counts when the chain uses it.
3. Build order is whatever blocks the most stages: form, sound mix, pact, review, publish kit, slot store.
4. Spending: the brief set a 0.75 US test fuse (16.3). The lead's cap today is 5.00 US. That difference is Ambi's to accept.

## Gates of 16:48 (Ambi), binding
1. The 10 minute film is finished, voiced, given a real WaveSpeed thumbnail and verified end to end before a cent is spent
   voicing the 50 minute film. In code: `scripts/purse.py` refuses a 50 minute voice, and any voice past 0.30 US, until
   `runs/films/ten/LEAD-PASS.json` exists (the lead's alone). Tested: both refused.
2. Gate, Altar, Crossroads, Cauldron, Pact, Conjuring, Spell Strip, Publish Kit live on the Rust server before any other room.
3. Seven to ten tight lanes, one owner each, Haiku click verifiers. Counts are stated as live, open, queued.
