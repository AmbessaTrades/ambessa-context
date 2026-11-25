# 0018 The run-until-done constitution

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

**Status:** Ambi's order, 24 Nov 2026 about 17:45 EAT ("Install the permanent harness, upgrade the skills, and run
autonomously until the entire Exit Predicate is verified TRUE"; "have the agents that are currently doing this rerun
their sub agents, as long as they're not in really important work"; "don't be stubborn with it"). The files, the lane
split, the receipt names and every wording are the root's.

## What was installed

| Law (Ambi's words, shortened) | Where it lives | Held by |
|---|---|---|
| Line 1 of every worker kickoff | `WORKER.md` | `scripts/kickoff-line.py`, `scripts/kickoff-line.py`: a SubagentStart hook that tells every sub-agent and workflow agent, and a PreToolUse hook that puts the line first on Agent, Task, T3 delegate, thread launch and create_threads |
| State the exit predicate, drive until true | `docs/poteto/root.md` | `scripts/exit-predicate` (23 clauses, baseline 3 true) |
| Prove on the live thing | `docs/poteto/live-proof.md` | the receipts the predicate reads; `scripts/exit-predicate walk` |
| One change, one measurement, keep or revert | `docs/poteto/hillclimb.md` | `scripts/decide` refuses a row without evidence |
| No worker loosens a gate or the meter | `WORKER.md` | `pins.txt` audit, `scripts/purse.py`, a countersign from someone who did not write it |
| One build folder, heavy work serialized | `WORKER.md` | `scripts/heavy` (one job, shared `CARGO_TARGET_DIR`), `scripts/light` (2 slots) |
| The same loop inside Juju | `docs/poteto/runtime-loop.md`, pack `juju-poteto-autopilot` | partly: see that page's last table |

Sources read word for word that day: pstack `poteto-mode`, `worker.md`, eight playbooks, eleven leaf skills, `unslop`;
Earshot's README; the context pack's `00-READ-FIRST.md` and `01-context.txt`.

## Conflicts this order settles, and what each supersedes

1. **Heavy work.** `scripts/heavy` was a pool of 3 since 16:38 (ADR 0017 era), citing Ambi on 25 Oct ("never a
   one-at-a-time lock"). The 17:45 order says "serialize heavy GPU/render/cargo builds (max_heavy = 1)". The root set
   one slot at 17:57 and measured at 18:10: load fell from 42 to 60 down to 16, but one render used 1.3 of 8 cores
   while 8 jobs waited 2 to 11 minutes, three of them cargo builds, and a trivial test job waited 621 seconds.
   At 18:12 the root made two lanes of one job each against the literal order, and said so to Ambi. Measured 18:39 to
   18:43 with two lanes: load 42 to 65, 9 and 10 jobs queued. The change did not help and was reverted at 18:50: **one
   job at a time, as ordered.** The lock now lives in the waiting process, so a child left running holds nothing, and a
   heavy command inside a heavy command does not wait on itself. Click walks and probes have their own lane, `scripts/light`.
2. **Build folder.** `scripts/gate.sh` set `CARGO_TARGET_DIR` to its own checkout. It now takes the shared folder
   unless one is given. Nothing about what the gate checks changed. Root's countersign: this line.
3. **Model levels.** pstack defaults to Opus at xhigh. Ambi's standing rule (27 Oct, 1 Nov) caps Opus at medium and
   keeps Haiku for sweeps. The standing rule stays.
4. **Draft PRs, forge.** pstack opens every PR ready and uses `gh`. Same here. Reviews run on GitHub's runners
   (`pr-gauntlet` rule 2), not on this Mac.
5. **The 16:48 gates stay binding:** the 10 minute film before any 50 minute voice; the eight core rooms before any
   other room; `scripts/purse.py` and the cap of 5.00 US are untouched.

## Found while installing (not fixed here; each is a unit for its lane)

- The main checkout's packs differ from its own `pins.txt` in 64 places (measured by recomputing the pins; the
  integration branch matches 656 of 656). The integration branch is the trunk candidate; the main checkout is not.
- PR 1 made the tests of `juju-stage` and `juju-reliquary` non-blocking in `gate.yml`. That softened check comes out
  before a merge counts as green.
- 329 uncommitted files sit in the main checkout. The predicate's trunk clause stays red until they land or leave.
- The conductor keeps the newest repair even when it finds more (`run.rs`, the repair loop). Unit: keep or revert.
- Stage 7 has no sound check. Unit: Earshot hears the mix before the film passes.

## What the hook covers, and what it cannot

Claude Code: every sub-agent is told at its start by the SubagentStart hook, whatever its prompt says. Agent, Task, T3
delegate, thread launch and create_threads kickoffs also get the line put first. A headless `claude -p` gets it from the
SessionStart boot text. No shell command is judged: a reviewer showed that judging one both misses real kickoffs and
refuses innocent commands. Not covered by code: Hermes delegation, Codex, and an agent started by a program. For those the
line is in `~/.hermes/memories/MEMORY.md`, `~/AUH/AGENTS.md` and this repo's `AGENTS.md`, which is text an agent can miss.

## Review of PR 11 (24 Nov, 18:38 to 18:55)

A fresh reviewer found 21 faults, four of them clauses of `scripts/exit-predicate` that passed when the thing was not
true. Two fresh reviewers then rechecked 181246f and found twelve more, nine of them blocking (signals that freed the
heavy lane early, siblings inside one job, a walk of uncommitted fixes, a three second picture under ten minutes of
sound). They are answered at the next head. Open and named: `pr_state.py` PROTECTED is shorter than `WORKER.md`'s list;
`purse.py` opens the voice gate on an empty `LEAD-PASS.json`; the merge door needs `docs/MERGE-LOG.md` on main, which
lands with PR 10; `scripts/test_contract.py` is run by no workflow yet; not every fix has its own planted fault.

## Who merges

One lead thread, one door: `pr_state.py merge` after two fresh clean reviews and green checks. The lead's own gate
changes are countersigned by a fresh reviewer. Ambi, 24 Nov about 18:48: "merge what needs to be ... just merge everything."

## The cost of one build folder

`target/release/*` is now last writer wins across branches. A binary used as proof is copied beside its receipt with
its sha256 and commit (the app server lane already did this). `python3 scripts/pins-check.py .` recomputes the pins
without a build.

## Added 18:20 (Ambi): one thread leads, and a date

Said: "the giant one, that's doing all the work. Which we're going to pick up all of its work and ... continue on this
thread." Said: "we need it ready by LATEST tomorrow 4pm EAT." Said: "I hope this potato structure is not a skill that I
have to keep referring back to. It should just be automatically on for everything all the time."
The root session becomes the only lead as the old lead's lanes end; the old lead starts nothing new and writes
`runs/predicate/HANDOFF.md`. This supersedes the root and lead split above. What "ready" means at 16:00 on 25 Nov is an
open question in the interview that began at 18:35.

## Added 20:04 (Ambi): "remove 1 job at a time limit."

Supersedes `max_heavy = 1` of 17:45 and everything above that follows from it. `scripts/heavy` runs jobs side by side, first
come first served, up to four (six were tried for eight minutes: load 77), holding a job back only when the pool is full, or while others run and memory free is under 18
percent or the load is over 3 a core. Each job has a time limit. Measured just before: one test loop held the single lane 13 minutes
while nine jobs waited up to 32, then sixteen jobs waited up to 46 minutes with the load at 11 and 74 percent of memory free.
