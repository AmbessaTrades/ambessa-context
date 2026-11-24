# Pull requests on the private Juju repo

As of 13:45 EAT, Tue 24 Nov 2026. The repo is private: the links need access, so each request's own description is copied here.
Nothing merges by itself yet. The lead merges after the gate is open and fresh reviewers find nothing that matters (ADR 0003).

| No. | State | Checks | Title | Lines |
|---|---|---|---|---|
| 8 | open | success | One command to see balances and models | +30 -2 |
| 7 | open | success | The sample film the rooms are drawn from | +5951 -2 |
| 6 | open | success | Library of Tehuti channel record and variety rules | +2519 -2 |
| 5 | open | success | Reliquary: patient archives, fewer wrong refusals, tests compile again | +84 -37 |
| 4 | open | success | Decision record: fixed money, looks, taste | +34 -2 |
| 3 | open | success | Quiet screens: names and verbs only, checked by code | +1292 -19 |
| 2 | open | success | Script gates, rounds 3 and 4 | +4319 -133 |
| 1 | open | success | Workspace list is a glob | +15 -2 |

## 8. One command to see balances and models

**What it adds.** `scripts/keys-check.sh`: one command that asks each paid service for the balance and the models on offer (OpenRouter, DeepSeek, Gemini, WaveSpeed). It only reads; it makes nothing and spends nothing.


**How it was checked.**
- `zsh -n scripts/keys-check.sh`: no errors. Read line by line.
- Key scan: clean, no literal hit either. Rust tests run in the PR's gate; this change holds no Rust.

**Not verified.** It was not run here, because it would use the owner's live keys. It was written on this Mac and names `/usr/local/bin/python3`. If a service answers with an error page, the script prints the first 200 to 300 letters of it.

**What the owner sees differently.** A way to see what money is left without opening four websites.

Contains the two-file change of #1 (merge #1 first; then this page shows only its own files).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 7. The sample film the rooms are drawn from

**What it adds.** The sample film every room is drawn from: `runs/first-film/film.json`, "The ENTIRE Journey After Death in 52 Minutes", with the nine act files it was written from. Main already holds its research and spine, and `MAKER.md` and `ART-BRIEF.md` already point at this file, but the file itself was missing from the repo.

**How it was checked.**
- All ten JSON files open in Python.
- `film.json`: nine acts numbered 0 to 8. Counting the spoken words gives 5,943, the number it claims. Its ledger holds 75 claims.
- Key scan: clean. Largest file 179 KB. Rust tests run in the PR's gate; none reads these files.

**Not verified.**
- It is short of its title: the file says 41.9 minutes, the title says 52. The title or the script has to change before it is ever used as a film.
- The act files hold earlier wording; `film.json` is the later text. `act-09.json` is only a "skip" mark.
- The 75 quoted passages were not checked against the books here, and the script was not run through the round 4 gates.

**What the owner sees differently.** Nothing new on screen; a fresh copy of the repo now has the film the rooms show.

Contains the two-file change of #1 (merge #1 first; then this page shows only its own files).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 6. Library of Tehuti channel record and variety rules

**What it adds.** The channel record for Library of Tehuti, as data.
- `vessels/lot.json`: the first real channel file.
- `vessels/lot-variety.json` and `LOT-VARIETY.md`: ten kinds of film, when each may come back, the rules code can check, and a 28 day sample calendar.

Most of it is marked candidate or inferred; what the owner said is quoted with the date.

**How it was checked.**
- `python3 -m json.tool` on both JSON files: valid.
- A Python copy of the Rust rules in `crates/juju-core/src/vessel.rs` run on `lot.json`: only known fields, all eight layers present, versions above 0, keeper, sound mode and slug allowed. 6 of 6 true.
- Key scan: clean. Rust tests run in the PR's gate; none of them reads these files yet.

**Not verified.** The Rust loader itself has not opened `lot.json`. The calendar's measured numbers were not re-run. The judge test (can a fresh eye tell two films apart) has not been run; no film exists yet. The voice is still empty.

**What the owner sees differently.** Nothing on screen yet. The day's kind can be dealt from this file.

Contains the two-file change of #1 (merge #1 first; then this page shows only its own files).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 5. Reliquary: patient archives, fewer wrong refusals, tests compile again

**What it adds.** The archive-picture finder, made patient and readable by the stage.
- A busy archive is rested 30 seconds and asked again; four refusals in a row count as a shut door. Before, one refusal ended that archive.
- Slower calls to the Met (0.7 seconds apart instead of 0.3).
- A picture is no longer thrown out because editing software once wrote a Getty tag name in it. A real "Photo: Getty Images" line still throws it out.
- `sheet --all` draws one last page of every kept picture.
- The candidates file holds only what the stage reads; the full licence record moves to `rights.json`.

It also repairs this crate's tests, which do not compile on main, and puts the crate back into the full gate in `gate.yml`.

**How it was checked.** In the PR's gate, now with this crate in the main line: 26 of 26 laws pass (on main they do not compile). Key scan: clean. No file over 1 MB.

**Not verified.** No live archive was called from this pull request; the tests use recorded answers. Not run against the newer stage engine that is still being written, so it may need a touch when that lands.

**What the owner sees differently.** Fewer "archive closed" stops while pictures are gathered.

Contains the two-file change of #1 (merge #1 first; then this page shows only its own files).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 4. Decision record: fixed money, looks, taste

**What it adds.** One page, `docs/adr/0008-fixed-money-looks-taste.md`, with the owner's words of 24 Nov:
- The money is fixed at 135 CAD, WaveSpeed is only for thumbnails, and the app never asks for more.
- 24 ready-made looks, exactly four for spirituality; none built on a count of pictures.
- Taste comes from his faceless-only YouTube account; never Shorts.
- Fonts, palettes, quotes and motion live as libraries of data, and nothing invents a one-off style.

The split of the 135 (voice 55, flagship scripts 21, daily scripts and checks 22, picture checker 14, thumbnails 14, outlines 9) is marked as the lead's candidate. He said "I agree with your exact mapping of the money"; it is open until metered.

**How it was checked.** Read in full. The split adds up: 55 + 14 + 14 + 21 + 22 + 9 = 135. Key scan: clean. Rust tests run in the PR's gate; this change holds no code.

**Not verified.** The quotes were not checked against the recording. No call has been metered yet. `docs/DESIGN-SYSTEMS.md`, which the page points to, is not written yet.

**What the owner sees differently.** Nothing on screen.

Contains the two-file change of #1 (merge #1 first; then this page shows only its own files).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 3. Quiet screens: names and verbs only, checked by code

**What it adds.** The owner's "stop writing subtext everywhere", as a decision and as code.
- ADR 0009 records his words and the rule. His direction; the numbers (30 words wide, 24 on the phone, no text of 5 words) are the lead's.
- `mockups/kit/shot.py` fails a room that has a sentence, a line under a name, or too many words.
- The maker law, the art brief and the two screen skills (`impeccable-juju-ui`, `calm-room-and-mind-touch`) now say the same.
- `mockups/kit/copy.json` and `COPY.md`: every word each of the 19 rooms may show.

**How it was checked.**
- `python3 -m py_compile mockups/kit/shot.py`: compiles. `json.tool` on the three JSON files: valid.
- `copy.json`: 925 strings, none of 5 words or more. Gate's own pack check: 44 skills, none bad.
- Rust tests run in the PR's gate. Key scan: clean.

**Not verified.**
- `shot.py` was not run on a room here (the Mac is busy). Older rooms were drawn under the old law, so expect `QUIET` faults in them, and `scripts/gate.sh` reads that tool.
- One leftover: `impeccable-juju-ui/skill.json` still says "at most 40" under `done_when`. The real limit is 30.

**What the owner sees differently.** New rooms carry names and verbs only.

Contains the two-file change of #1 (merge #1 first; then this page shows only its own files).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 2. Script gates, rounds 3 and 4

**What it adds.** Rounds 3 and 4 of the script gates: what attackers and forgers got past rounds 1 and 2 is now caught.
- 21 new "sounds like AI" rows in the healer pack (104 to 125), and scoped ones that flagged plain human writing.
- The claim reader asks for a source when a script says an amount, a crowd, a decade or a half-hidden book title it used to miss.
- A denial the source itself makes word for word is not treated as an AI trick.
- The round 4 trial scripts and ledger the tests read, and the round 4 reports on the sample film (largest 28 KB).

**How it was checked.**
- `python3 -m json.tool` on every JSON file in the change: all valid. Healer rows: 125, all ids unique.
- The gate's own pack check: 44 skills, none bad.
- Test count in `tests/gates.rs`: 48 before, 64 after. In the PR's gate: 64 of 64 pass, and all 74 `juju-conduct` tests pass against the new script code.
- Key scan: clean. The only plain hit on `sk-` is the row name `B-ask-yourself`.

**Not verified.** No new script has been judged by a person against these rows. The pack's own notes list what no rule can hold: stock metaphors, a quip after a fact, triads of nouns.

**What the owner sees differently.** Fewer AI tells survive in a script, and more unsourced claims stop before recording.

Contains the two-file change of #1 (merge #1 first; then this page shows only its own files).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 1. Workspace list is a glob

**What it adds.**
- `Cargo.toml`: the crate list becomes "every folder under `crates/` and `apps/`", so two pull requests that each add a crate never collide on that line.
- `gate.yml`: main's own tests are broken in two crates. They still run on every pull request, but each now blocks only a pull request that touches that crate.

**Why the gate changed.** The gate had never run before today. Its first run was red on main itself:
- `juju-stage`: `tests/laws.rs` does not compile against `src/heal.rs` (4 errors, for example "expected `Healed`, found `(_, _)`"). It also reads `runs/stage-x` and `runs/lot-r01-proof`, which `.gitignore` keeps out of the repo.
- `juju-reliquary`: `tests/laws.rs` does not compile against main's `juju-stage` (4 errors).

This is looser than before on purpose. It is undone crate by crate: when a crate lands green, its name goes back in the main line and its step is deleted.

**How it was checked.**
- The PR's gate: cargo accepted the glob and all six crates compiled. 138 tests pass in conduct, script, skills and core. The stage and reliquary steps show red inside a green job.
- All 7 folders on main have a `Cargo.toml`. Key scan of the diff: clean.

**Not verified.** `apps/juju-shell` is left out of the gate, as before. Cargo was not run on the Mac. A folder under `crates/` without a `Cargo.toml` would now break the build.

**What the owner sees differently.** Nothing in the app. Pull requests can now go green.

🤖 Generated with [Claude Code](https://claude.com/claude-code)
