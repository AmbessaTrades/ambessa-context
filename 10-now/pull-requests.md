# Pull requests on the private Juju repo

As of 04:46 EAT, Thu 26 Nov 2026. The repo is private: the links need access, so each request's own description is copied here.
One unit, one pull request, one review round (ADR 0020). The lead merges when fresh reviewers find nothing serious and the checks are green.

| No. | State | Checks | Title | Lines |
|---|---|---|---|---|
| 27 | open | ?, success | Rules agents read: WORKER.md, Ambi's eye, the film-harvest row | +21 -0 |
| 26 | open | ?, failure, skipped, success | juju-sound: a film's sound, heard by Earshot | +1240 -0 |
| 25 | open | ?, success | juju-gather: a bare card to sourced facts, tables, pictures | +2503 -0 |
| 24 | open | ?, success | juju-next: grounded cards, two sealed readers, one journal | +8100 -854 |
| 23 | open | ?, success | Style kits and their checker, as they are | +5284 -0 |
| 22 | open | ?, success | scripts/harvest and ADR 0021: take a film apart | +2153 -0 |
| 21 | open | ?, success | juju-sigil: thumbnails from a film's own data, gates in code | +1378 -0 |
| 20 | merged | ?, skipped, success | Skill film-harvest: take a film apart, with its rows and pins | +5730 -0 |
| 19 | merged | ?, skipped, success | Six looks: One Ink and Downlink in, with their fonts and tools | +1305 -560 |
| 18 | merged | ?, skipped, success | Pack spirit-tongue 0.3.0: numbers, event times, needs, facts told | +104 -43 |
| 17 | merged | ?, skipped, success | ADR 0017: Ambi's gates of 16:48 | +7 -0 |
| 16 | merged | ?, success | The job queue: eight side by side, the load is not asked | +7 -7 |
| 15 | closed | skipped, success | A head keeps its train light while a later train runs | +23 -6 |
| 14 | merged | ?, skipped, success | ADR 0020: one unit, one pull request, one round | +23 -3 |
| 13 | merged | ?, success | Ambi's ear table and the script lessons, under docs | +41 -0 |
| 12 | merged | ?, skipped, success | Conductor: keep or revert, one step up, Earshot hears the mix | +542 -51 |
| 11 | merged | ?, skipped, success | Run-until-done contract: worker contract, exit predicate, attempt log | +1283 -8 |
| 10 | merged | ?, skipped, success | Integration 24 Nov | +64252 -1698 |
| 9 | merged | ?, failure, success | PR gauntlet: merge train, gate checks without a model, review states | +1284 -2 |
| 8 | merged | ?, success | One command to see balances and models | +30 -2 |
| 7 | merged | ?, success | The sample film the rooms are drawn from | +5951 -2 |
| 6 | merged | ?, success | Library of Tehuti channel record and variety rules | +2519 -2 |
| 5 | merged | ?, success | Reliquary: patient archives, fewer wrong refusals, tests compile again | +84 -37 |
| 4 | merged | ?, success | Decision record: fixed money, looks, taste | +34 -2 |
| 3 | merged | ?, success | Quiet screens: names and verbs only, checked by code | +1292 -19 |
| 2 | merged | ?, success | Script gates, rounds 3 and 4 | +4319 -133 |
| 1 | merged | ?, success | Workspace list is a glob | +15 -2 |

## 27. Rules agents read: WORKER.md, Ambi's eye, the film-harvest row

## What it adds

`WORKER.md` as the main checkout holds it (two more rules: films come out of Juju; the Mac is for films and a lane's own build), `runs/scriptlab/AMBI-EYE.md`, `runs/scriptlab/AMBI-EAR.md` as a link to `docs/AMBI-EAR.md` (the same bytes, already in main), and the `film-harvest` row of `ask-juju`, section D, as `reach-and-pins.patch` gives it. The one ADR main lacks, 0021, comes with #22; four ADRs of the main checkout are older than main's and were left.

## How it was checked

`scripts/test_contract.py`: held, 0 failed, pins match. `gate_checks.py tree` open. `skills_routed` and every pin are unchanged.

## Not verified

- `skills_routed` says 32 and was not raised for the new row: it is pinned, and the lead's to change.
- No agent has been started from these files in a clean checkout.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 26. juju-sound: a film's sound, heard by Earshot

## What it adds

The crate `juju-sound`: places for sound found by rule in a film, kept sounds offered, the Watcher picks, Earshot hears each cue, one mix at -14 LUFS, or a refusal. Its two glue files stand in `scripts/sound` (same bytes; the paid call still goes through the gate of `scripts/purse.py` with a `scripts/meter.py` reservation; the lead's ruling of 25 Nov 07:28, gate untouched). `scripts/sound/BEDS.md` holds licence and source of the two beds that are real recordings. From the main checkout (the same files as `unit/sound`), with one change for GitHub's machines: ffmpeg, ffprobe and python3 are taken from the path where this Mac's own are absent. No receipts, replies or sounds are in it.

## How it was checked

Measured by the maker, 25 Nov, not run again: a 60 s film at -14.1 LUFS with 2 of 2 cues heard, 9 planted faults refused, a silent kit at -14.2 with 4 cues. Here: `cargo check --all-targets`. The tests run on GitHub.

## Not verified

- The Vision frame test (`the_frames_of_the_film_are_really_read`, Mac only) is left out: it reads two film frames, and no film frame goes in. So reading real frames has no test in main. The test and frames stay in the main checkout.
- The 1.28 s hush on silent films: `make-mongols` is refused at -21 LUFS, open, not a blocker (lead). Levels of a film with no voice are Judged.
- Under a fast narrator a cue is heard only in its pause (about 0.2 s). No listen on a phone speaker.
- A 20 minute film takes 912 s at load 35 to 49. The beds' licences are the shelf's own record, not read again at the source.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 25. juju-gather: a bare card to sourced facts, tables, pictures

## What it adds

The crate `juju-gather` as it stands (freeze 14): from a bare card, the sourced facts, the tables `juju-stage` draws and the pictures, or an honest no. It joins the workspace by the glob; its own `[workspace]`, lock and profiles are removed and two `[profile]` lines are added to the root `Cargo.toml`. It builds against main's `juju-reliquary`. Source as in the main checkout, with one repair round:

- `docs.rs`, `spot.rs`: official is the last address's host, equal to or under a listed one.
- `door.rs`: promises are never under main's `prices.py`; the film limit and the 0.20 ceiling are counted over paid rows and open promises under one lock across processes.

## How it was checked


## Not verified

- The lane's predicate is not TRUE: 0 of 100 second readings done, no cold run of the newest binary (about 0.08 US; the lead's limit of 0.35 allows it once).
- Moons and the Ottoman film carry; Black Death, Zulu and Magellan are honest holds.
- The maker's proofs ran with the main checkout's `juju-reliquary`, which is not main's; here the two only compile together.
- Open for the stage lane: rims drawn between pieces of one owner, invented days on year tables, stairs on wide coasts. Map tables may carry no take rows; Borodino stood at 94.9 E in one table.
- A page that answers only http is now lost. Official pages an older program kept have no last address: they are refused until fetched again into a new shelf. The second reader's model (gpt-6-luna) has no price in main's `prices.json`, so main's gate refuses it.
- Needs data that is not in the repo (`JUJU_DATA`, `runs/gather/data`, `runs/stage-y/fonts`) and the local gate.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 24. juju-next: grounded cards, two sealed readers, one journal

## What it adds

`juju-next` as it stands in the main checkout (work of 25 Nov, 05:26): cards built from their answer outward, words of a title held to its passage, two readers sealed to the card, pictures from their own records, bends on the donor's shape, one journal for a deal. `juju-core` and `juju-script` are no longer needed by it; `glue/bend.py` is no longer called, and stays because `scripts/tests/test_money.py` tests it. It stays a workspace member, with main's `Cargo.toml` lines. Two edits for GitHub's machines: the program and one test fall back to `python3` where `/usr/local/bin/python3` is absent, and `glue/checks.py` reads the checkout it stands in, not a fixed path.

Repair round: `door.rs` reserves as the job `juju-next`, so main's cap of 0.06 US a UTC day in `scripts/prices.json` is asked inside `meter.reserve`; the 0.12 and `JUJU_NEXT_DAY_USD` are gone; one lock across processes. A missing or empty word list refuses to start; tests carry `tests/words.txt` (2,535 words).

## How it was checked

Repair, on the Mac: 43 and 14 tests pass, with main's own `meter.py` in a temp folder: 20 callers at once stop at the day cap with the old env set to 99; a task ceiling only stops sooner; an unreadable book stops; no list and an empty list are refused.

Here: `cargo check --all-targets`, `gate_checks.py tree` and `diff` open. Measured by the maker, not run again: 15 of 15 planted false titles passed before, 0 of 15 now; two deals at once and kills lose nothing (13 of 13).

## Not verified

- Its predicate is FALSE: 0 cards stand, the readers give pull 2 to 5 where 6 is the bar. No hand is dealt with this version.
- `test_money.py` still tests the old door; the new one is tested in `door.rs`. `gpt-6-luna` and `gemini-3.5-flash-lite` have no price in main's `prices.json`, so main's gate refuses those readers. At 0.06 a day a deal may stop early.
- No vote, no paste, no timing under load 20. Judges were weak in the earlier vote (3 of 6 plants).
- Map checks return early where the Natural Earth data is absent, so GitHub does not run them.
- The door is this Mac's: yt-dlp, `ytlocal.py`, the local gate.

## THRESHOLD CHANGE

- `main.rs`: three added lines trip the loosening pattern by their words: yt-dlp's `--skip-download` flag and two help lines that say `exit 0`. No test is skipped. The day cap of 0.06 US stays and is asked (an earlier head of this pull request did not ask it).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 23. Style kits and their checker, as they are

## What it adds

Five style kits (`design/kits/kit-*.json` and `.md`), the liked films, worlds and Vault part names they read, and their checker `design/kits/check` (Rust, its own root, not a workspace member), as they stand on 25 Nov 2026. Working documents: nothing in them is decided until Ambi says so.

## How it was checked

Here: `cargo check --locked` of the checker, `gate_checks.py tree` open. `kits check` and `selftest` were the maker's, on the Mac, not run again. GitHub does not build the checker, because it is no member, and it has no `#[test]`.

## Not verified

- The pour is not proved: 11 of 15 strips were never asked. No kit has passed a blind sheet.
- The checker reads files that are not in main: `runs/sound`, `runs/kits/tools/ask.py`, `runs/films/arcs`, `runs/character/narrators`, `crates/juju-db`, `~/AUH/DATA`. From a clean checkout it cannot pass.
- Faults open for the engine (each kit's `engine_lacks`): the date line runs through invented days, the last thing of a scale rests off centre, a route shows the Sun alone on a long leg, the counter's words cross borders.
- Lines are true and plain; a viewer may find them flat. Bygone Philosophy is in `liked.json` and no kit learns from it (ADR 0014 point 9).

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 22. scripts/harvest and ADR 0021: take a film apart

## What it adds

`scripts/harvest` and `scripts/harvest_lib`, the command the merged skill `film-harvest` already names, and `docs/adr/0021-harvest-first.md`. No film, no frame, no model: `mdx_cpu.npy` (12 KB) is a 4 x 48 x 16 slice of one model's answer that `check_models.py` compares with. `STEMS-OFF` is the lead's switch of 25 Nov 03:16, kept.

## How it was checked

The maker's runs (Measured by the maker, 25 Nov, not run again here): windows answer the same as upstream; three windows scored against hand truth. Here: `gate_checks.py tree` open (the Python compiles), `scripts/harvest` parses. `scripts/tests/test_harvest.py` (repair round: a survey that dies silent is refused; the old source fails it) was run on the Mac; GitHub's workflow does not name it, and the workflow was not touched.

## Not verified

- The 3 times speed target was not reached (about 1.2 times, Measured by the maker).
- Works on this Mac only: `~` paths, `.toolchain/rea`, CoreML, Vision. rea-video itself and its models are not in the repo.
- `--vision` gives other text tracks on busy maps. The sound split is off.
- The whole flow by a fresh agent.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 21. juju-sigil: thumbnails from a film's own data, gates in code

## What it adds

The crate `juju-sigil`: three free thumbnail layouts from a film's own data, gates G1 to G6 in code, a blind vote, and one buy only when a bought picture wins. It joins the workspace by the glob; its own `[workspace]`, lock and profiles are removed and two `[profile]` lines for it are added to the root `Cargo.toml`. Source and tests are the main checkout's, with one repair round: the cost and time of a bought picture are read from the book's row, which main's gate writes at the POST.

## How it was checked

The lane's own check (Measured by the maker, 25 Nov 03:36, not run again for this pull request): `runs/sigil/receipt.json` all true, 20 of 20 fault tests, 19 of which fail on the older source; lane spend 0.0903 US. Here: `cargo check --all-targets` in this workspace, `gate_checks.py tree` open (39 tests counted). The repair is tested against main's own `purse.py`, `meter.py` and `prices.py` on a book in a temp folder, the sending replaced (no paid call): `tests/buy.rs`, 6 of 6 on the Mac. The tests run on GitHub.

## Not verified

- The medium buy path ran only against a mock door; two real low proofs were bought and both lost the vote.
- Fixtures are written by hand; hue is not judged in G4; no outside reader has judged the pictures.
- A package that asks for a picture its film does not hold is a HOLD; `juju-cli` does not expect that yet.
- The door is this Mac's: `/usr/local/bin/python3`, `scripts/meter.py`, the local gate on port 4610.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 20. Skill film-harvest: take a film apart, with its rows and pins

## What it adds

The skill pack `film-harvest`: how a film is taken apart shot by shot, upstream's method exactly (rea-video fc69e19, Apache-2.0, licence and notice in the pack), all thirteen of its references in English, answer forms as JSON schemas, kickoff texts, a self test, and step 8, which is ours (hand truth, motion language, blind rebuild, systems). Its rows in `reach.rs` and 16 pins, additions only.

## How it was checked

`pins-check.py`: 800 of 800. `gate_checks.py tree`: open. The maker's own run: skills check at main passes, 8 of 8 juju-skills tests; a fresh agent given the pack alone made a package of a 20 s film that passes `videomd --check` and answered the self test 6 of 6.

## Not verified

Films over 20 s by this pack, `scripts/harvest`'s whole flow, step 8, and the Watcher and Scribe forms. The lead countersigns the pins: every changed line is an addition.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 19. Six looks: One Ink and Downlink in, with their fonts and tools

## What it adds

The six looks as they closed at 19:33 on 24 Nov. `design/looks` is the live folder, byte for byte, except the source picture that stays out of git.

1. **Two looks replaced.** One Ink (`map-one-ink`) takes the place of Broadsheet, Downlink (`space-downlink`) the place of Space Age. The other four (Survey File, Bartholomew 1875, Signal, Ledger) are the newer files.
2. **Fonts.** B612 and VT323 come in, each with its SIL Open Font License. Michroma and Share Tech Mono go out: no tracked file names them, nor the two old looks (`git grep`, Measured).
3. **Tools.** `needs.py` writes `ENGINE-NEEDS.md` from the look files, so its tables cannot drift. `territory.py` computes contrast under territory names. `gen.py`, `distinct.py` and `proof.py` are the versions that made these files.
4. **Pack `ghost-onions` 0.3.0.** It names the two new looks and the two new tools. The branch's own text of R10 and R11 stays. Two edits in `SKILL.md` say what the looks are: candidates, with contrast recorded on composited stills only.

THRESHOLD CHANGE (a pin change; nothing is loosened): two existing lines of `crates/juju-conduct/src/pins.txt` change, `data ghost-onions` 476d9628cab97f1b to 4bf06da14c3ab392 and `skill ghost-onions` 35d9679069118bdf to 46c3fbd5fa86a209, because the pack's data and skill text changed as in 4. No line is added or removed, no rule, limit, kind or stage in the pack changes; its version goes 0.2.0 to 0.3.0. Also named here so it is seen: the list of fields `design/looks/tools/distinct.py` counts has changed. A name-size field came in, and the black-point half of the relief field went out, because the looks dropped black point. The bar stays at 3 and the closest pair scores 7 with the base's list and with this one. Countersign: the lead, who did not write it.

## How it was checked

At this head, on main at 2f7f6bc:

- `python3 design/looks/tools/gen.py` and `python3 design/looks/tools/needs.py`: `git diff` stays empty (Measured).
- `/usr/local/bin/python3 design/looks/tools/distinct.py`: all pairs at 3 or more, smallest 7; `git diff` stays empty (Measured). The base's own `distinct.py`, run over the new look files, says the same: all at 3 or more, smallest 7 (Measured).
- `python3 scripts/pins-check.py .`: 784 of 784 (Measured).
- `gate_checks.py` tree, diff and body: open (Measured).
- Both new fonts open, and their ten digits have one advance each (Measured).
- `scripts/heavy cargo test --offline -j 3 -p juju-conduct -p juju-skills`: 220 passed, 0 failed (Measured), built from this worktree in a build folder of its own, with debug info off to save disk. A first run in the shared build folder was thrown away: cargo called it finished and ran the binaries of another worktree.

`scripts/gate.sh` was not run whole: this unit has no room and no Rust source, so its Rust part is the two crates above and the rest is the GitHub gate.

## Not verified

- **The engine cannot draw these looks.** On this branch it reads fonts, six colours and side colours; sizes, tracking, case, bed, sea, relief, lamp and finish are hard-coded (`ENGINE-NEEDS.md`).
- A fresh critic of the six looks is still owed. Ambi has not chosen one. No film wears a look and no blind judge saw one.
- `proof.py` and `territory.py` were not run again here. The contrast, spacing and safe-box numbers in the look files come from one engine build (16:42, 24 Nov) and need `runs/stage-y` and `runs/engines`, which are not in git.
- No proof frame carries a territory name, so those names are unproven on screen. `map-bartholomew-1875` says of itself that some side tints are hard to tell apart.
- Paths that are named but not in git: the 3.1 MB picture `design/looks/sources/bartholomew-africa-1875.jpg`, and four narrator files under `runs/character/narrators/`.
- The licence text of VT323 carries its author's public contact address. It is the upstream copyright line, so it stays whole.
- The unit was cut from integration/2026-11-24b at ba9b9b1. Pull request 10 merged while it was checked, so it is opened on main (ADR 0020, 1 and 5); the patch is the same bytes.
- This pull request and the spirit-tongue one both edit `pins.txt`; the second to land may need a rebase.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 18. Pack spirit-tongue 0.3.0: numbers, event times, needs, facts told

## What it adds

Pack `spirit-tongue` 0.2.0 to 0.3.0, with its pins. No Rust code changes.

- **R15** numbers and lengths of time: each is on the fact list beside its event, or worked out by code. **R16** event times: an event is told with its own clock, within 1 minute. **R17** needs: a habit, opening or ending goes to the writer only when a fact carries its tag. **R18** facts told: at least 0.9 of a part's facts. Candidates, run once, held by no crate.
- **flight-engineer v6** (from v3): quieter habits, endings and number line, and a `needs` list for code.
- The deal for a film of several parts (one habit a part, the number habit in one part only), marked as candidates run once and not shown to work.
- The measured four part Apollo 13 film: 949 and 1,197 words, 36 and 37 of 37 facts told, and the character did not hold. The pack says: do not ship the film recipe.
- `chapter_card` leaves the narrator routes: a chapter card is type on the screen.
- `SKILL.md`: the running text of 24 Nov, 17:02, with the branch's order line, Pinned line and Mac-only footer kept; wrapped paragraphs are joined to fit the gate's 110 lines (107).
- The header of `pins.txt` now says nobody but its builder has read spirit-tongue R10 to R18 (it said R14).

**THRESHOLD CHANGE** (countersign: the lead, who did not write it). `gate_checks.py` finds no loosening; these are the pins, and what a person should rule on:

- `pins.txt`: three pins change (`data`, `params` and `skill` spirit-tongue), four are new (`rule spirit-tongue/R15`, R16, R17, R18), one header line changes. No other pin changes.
- `narrator_routes.kinds` drops `chapter_card`, so a chapter card is no longer sent to a narrator. This is the one change that narrows what a rule covers. R1 to R14 are unchanged.
- New candidate numbers: `facts_told_share_min` 0.9 and `event_clock_tolerance_min` 1.

**Left out of the cut on purpose.** The patch for this unit also added R15, R16 and R18 to the builder-only list in `crates/juju-conduct/src/reach.rs`, so that the ear critic would not be shown gates it cannot judge. No critic is shown them without those lines: `lens_rules` shows a critic only rules named in `READS_WORK`, and no spirit-tongue rule is there. The lines would only have taken the three gates off the list of gates not enforced. Without them they stand on that list beside R10 and R12 to R14, which is the truth.

## How it was checked

At fdfd6fa, whose parent is 74a8604:

- `scripts/heavy cargo test --offline -j 3 -p juju-conduct -p juju-skills -p juju-script --no-fail-fast`: **272 passed, 0 failed, 0 ignored**, exit 0 (Measured).
- `scripts/pins-check.py .`: 788 of 788 (Measured). `gate_checks.py` tree and diff: open; this body: open.
- `juju-conduct plan`, built from this commit (binary sha256 464356d6d63d141a): spirit-tongue's gates not enforced are R7, R8, R9, R10, R12, R13, R14, R15, R16, R18; none is builder-only; no warnings (Measured).
- `skill.json` is byte for byte the lane's file of 17:02 (sha1 2b1a3066858e, Measured).
- The four commits that landed on the base since 74a8604 touch none of these three files.

## Not verified

- No crate runs R15 to R18. They ran only in Python stand-ins on the maker's Mac (`runs/character/narrators`, not in git), so the steps that name those files cannot be followed in a clone. The pack says so.
- The film numbers are the maker's, read in its report and not run again here. The pack's words "no false sheet number found by code" are that report's; the code check has known holes ("one day" and "one year" pass, comparisons with no unit pass).
- flight-engineer v6 ran once, on one fact list, and was never in the blind sort. R17 was never run on a list without tags. The paid rewrite call has no valid measurement. No voice was heard. A 2,400 word film was not run.
- No person has read R10 to R18.
- `SKILL.md` still says `order` printed 26 rules and 500 words; that was an earlier build and it was not run again.
- The room checks of `scripts/gate.sh` were not run: no room changes.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 17. ADR 0017: Ambi's gates of 16:48

## What it adds

- `docs/adr/0017-fleets.md` gains the section "Gates of 16:48 (Ambi), binding" (+7 lines, nothing removed): the 10 minute film first, the eight core rooms first, seven to ten lanes with one owner each. Gate 1 names the code that holds it, `scripts/purse.py`. ADR 0018 (point 5) already cites these gates; this is their text.

## How it was checked

- Base 639dc85. `scripts/purse.py` lines 36, 37 and 57 to 64 hold the refusal gate 1 claims: a voice reservation that names the fifty film, and any voice past 0.30 US since 13:48 UTC (16:48 EAT), until `runs/films/ten/LEAD-PASS.json` exists.
- "Tested: both refused" was run, not only read: `python3 scripts/tests/test_money.py`, 30 of 30. `test_ten_first` sends a voice call named fifty, one whose sender is named fifty and one that names no film (402 each, nothing reached the stand-in service), then twelve calls at once for the ten film (some 200, some 402, at most 0.30 US spent).
- Planted fault on a copy: with the `ten_first` check switched off, the same file fails `test_ten_first` (200 != 402). So the test sees the refusal.
- `python3 .github/scripts/gate_checks.py tree`: open. `diff` and `body` against the base: open. No threshold, gate or code changes here.

## Not verified

- The voice gate opens on an empty `LEAD-PASS.json`: `purse.py` line 60 asks only whether the file exists (PR 11's body says the same). "The lead's alone" is a rule in words; no code checks who wrote the file.
- The fifty film is known by its label: `film` starts with "fifty", or `who` holds it. A caller who names it something else is held only by the 0.30 US budget.
- The gate running on port 4610 is the older copy in the live folder (read there, not called). It refuses by the same two rules, with 403 for 402, and sees a fifty film only by `who`. This pull request does not restart it.
- Gates 2 and 3 are rules for people: no code holds the room order or the lane count.
- `scripts/gate.sh` was not run whole: its Rust, skill and room checks read none of this file. GitHub's checks run them on this head.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 16. The job queue: eight side by side, the load is not asked

## What it adds

`scripts/heavy` lets eight jobs run side by side and no longer asks the load. Measured 24 Nov 22:15 to 22:45: 36 jobs stood behind one build with three of four slots empty, because small work outside the pool held the load over 24; then three of four slots held cargo builds waiting for one build folder at no processor.

## THRESHOLD CHANGE

Looser: `JUJU_HEAVY_SLOTS` 4 to 8, and the load limit of 3 a core is gone. Kept: memory free under 18 percent holds a job back, first come first served, the time limit, the guard.

## How it was checked

`scripts/heavy /bin/echo runs` on its own pool; live on this Mac since 22:45 with 53 to 67 percent memory free. `scripts/test_contract.py` sets `JUJU_HEAVY_ANYLOAD`, which is now read by nothing; its tests do not depend on it.

## Not verified

`scripts/test_contract.py` whole at this head.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 15. A head keeps its train light while a later train runs

## What it adds

A head that already has its train light keeps it while a later train runs. Until now every new pull request set every open head back to "running", so with five pull requests opening in an hour nothing could merge: 639dc85 was green at 22:42:46 on 24 Nov and "running" again at 22:43:08.

## THRESHOLD CHANGE

Looser in one way: `train.py` no longer takes a light away before the next train has answered, so for the length of one train a head may show the green of the train before it, made against an older main. The next report overwrites it, green or red. A head with no light is set to "running" as before. Two ways an older green could outlive its report, both named: the write of the new light fails (now tried four times over 85 s, and then the report job is red and says not to merge), and a person cancels a train after its plan (then no report is written; the concurrency group does not cancel a running train, and nothing else does). `pr_state.py` also needs every check at the head green and two clean reviews.

## How it was checked

`light()` run against two real commits of this repository: f0490fe gives its newest light, an unknown commit gives None. `status()` against a stub: four failures give False, a success at the third try gives True.

## Not verified

A whole train with the change: the first one after the merge is the proof.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 14. ADR 0020: one unit, one pull request, one round

## What it adds

One unit: the rule for small pull requests. Words only, no code (+23 -3 in three files).

1. `docs/adr/0020-small-prs-one-round.md` (new): one unit, one pull request, one round of two reviewers started together. Only a block is FINDINGS (wrong result, hang, lost work or money, a leaked secret, a loosened gate). A fix or a note is CLEAN and goes to the next pull request. Ambi's words and what went wrong in #11 are at the top.
2. `docs/poteto/root.md` rule 7: the same rule for a leading agent.
3. `WORKER.md`, the merge line: the same rule in one sentence.

Unchanged: two reviewers who did not write it, green checks at that head, the lead's word on a gate change, `scripts/pr_state.py merge` as the only door. The ADR narrows what a reviewer reports as FINDINGS, on Ambi's words; no threshold, gate file or script is touched.

The base is `integration/2026-11-24b` and not `main`, because `WORKER.md` and `docs/poteto/root.md` reached that branch with #11 and are not on `main` yet.

## How it was checked

On base 74a8604 plus this commit, in a worktree of its own (all Measured):

- `python3 scripts/test_contract.py`: `{"contract": "held", "failed": 0}`, exit 0, 63 tests passed.
- `python3 .github/scripts/gate_checks.py tree`: open. `diff --base origin/integration/2026-11-24b`: open, 23 added lines, no key shapes. `body` on this text: open, nothing loosened.
- The three files are byte for byte the lead's live copies. The patch, cut against ba9b9b1, applied clean.
- No crate, script or workflow reads the three files' text: `git grep` finds only the kickoff line, which names the path of `WORKER.md`, and one Rust comment that names another ADR.

## Not verified

- `crates/juju-skills/packs/pr-gauntlet/SKILL.md` still says three rounds and "answer every finding" (lines 29, 38, 47, 63), and its `skill.json` line 105 asks for a reply to every finding. `docs/adr/0017-fleets.md` line 15 says "every finding answered". ADR 0020 replaces all of them; the pack's edit is a follow-up, not in this unit.
- Nothing in code holds the rule yet. `scripts/pr_state.py` takes CLEAN or FINDINGS as the reviewer gives it; it does not know block, fix or note, and does not stop a push into an open pull request.
- `runs/pr/NEXT.md`, named by the rule, is not in git. It is a file on this Mac.
- `scripts/gate.sh` was not run in full. Its four checks are Rust tests, installed skills, room faults and room truth, and none of them reads these files.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 13. Ambi's ear table and the script lessons, under docs

## What it adds

Maker: ship-script-lessons

Two documents, so a fresh checkout holds what Ambi's ear refused. Until now both lived only under `runs/` on this Mac. No code, no check and no number changes.

1. `docs/AMBI-EAR.md` (19 lines): the line Ambi refused ("The sun gave nothing"), what was ordered in the same message, and the three kinds of film praised, in quotes. Copied byte for byte from `runs/scriptlab/AMBI-EAR.md`.
2. `docs/SCRIPT-LESSONS.md` (22 lines): the nine script lessons of the ten minute film. Copied from `runs/predicate/notes/script-lessons-2026-11-24.md`; line 20 names `docs/AMBI-EAR.md` where the source names `runs/scriptlab/AMBI-EAR.md`.

**Which copy is worked on:** until the open script and words lanes close, a new refused line is written in `runs/scriptlab/AMBI-EAR.md` and a new lesson in `runs/predicate/notes/script-lessons-2026-11-24.md`, and the copies here are taken again from them. When those lanes close, the docs copies are the ones worked on and the `runs/` ones stop.

## How it was checked

- sha256, first 12, of the two live sources, read again just before the commit: `84505a6595ce` and `221fcea7460a`, the same as when the patch was cut (Measured).
- `diff` of each docs file against its source: none for the ear table; one line, the path, for the lessons (Measured).
- `gate_checks.py tree`: open. `gate_checks.py diff`: no key shapes in the added lines. `gate_checks.py body`: open, nothing loosened.
- `test_gate_checks.py`: 6 tests OK.
- No email shape and no long dash in either file, by grep; both read whole: no key, account or address.

## Not verified

- Cargo, the rooms and the rest of `scripts/gate.sh` were not run on the Mac: the diff is two new text files and no code, test or workflow reads them. The pull request's own checks run the Rust tests.
- The numbers inside the lessons (0.13 US for four drafts, 1,591 to 1,655 words, 0.03 to 0.04 US for the empty call, the order of the two listeners) are the earlier lane's and were not measured again here.
- The documents hold no check in place: nothing in code on this branch refuses a line because it is in the ear table.
- One of Ambi's orders is quoted word for word and names the browser; no account is in it. The repository is private.
- `juju-cli` `words.rs`, live on this Mac and not on this branch, names `runs/scriptlab/AMBI-EAR.md` in a comment. It is left alone: its lane owns it, and that is still the copy worked on.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 12. Conductor: keep or revert, one step up, Earshot hears the mix

## What it adds

The three rows of `docs/poteto/runtime-loop.md` that said "not held" are now code in the conductor.

1. **Keep or revert** (`run.rs`: `put_back`, `fewer`, `make_part`). After a repair the same checks run again, for each part. Fewer findings keeps it. The same or more discards it: the earlier output goes back in the part's newest file and in the record, the round stays spent, and the discarded text is kept in `parts/discarded/` where nothing reads it. What a critic rejected in a discarded repair stays rejected, and a quote still in a text that was put back is a finding even if the critics go quiet. The comparison is written on disk with the repair, so a run that dies before measuring does not trust the newer file. A repair that brings a finding a person must decide still holds the film at once, as before; it is not kept, and a run again holds the same way and buys nothing. When critics looked at only one of the two texts, code may not find more than it did, and only a quote that is gone counts as mended. If the first answer could not be read there is no earlier output, so whatever can be read after it is kept.
2. **One step up** (`run.rs`: `above`, `afford`, `stuck`; `provider.rs`: `LADDER`). After two rounds a writing part gets one try on the next model up, through the same `call()`: reserved first, settled, saved. A try that was promised in any attempt and has no reply on disk is never bought again (`Meter::of` reads the run's own spend file). The hold names what failed and the way out.
   The repair loop also has a step limit of its own (`Steps`): the most measures its rounds can need, then a hold.
3. **Earshot at stage 7** (`acts.rs`: `house/earshot`; `work.rs`: the `mix` job). It reads `sound/mix.wav` and `sound/earshot.json` in the run folder: `verdict` "pass", `synthetic_cues` 0, `listening_model`, `integrated_lufs` at the skill's `film_lufs` (-14) within 1, `mix_sha256` equal to the hash of the bytes, and `heard` {voice, bed, effects}. Missing, unreadable, stale or failing holds. A silent film keeps every clause and needs bed and effects heard and no voice. The film is sealed with the mix's hash. A receipt a Mock wrote is refused in a run that is no Mock, and is Unproven in one that is.

Candidates, not decided by Ambi: the ladder `glm-5.3-flash`, `glm-5.3`, `gemini-4-neon`; and a part's budget, which nothing defined. It is the film's tapped `pool.cost_per_film_usd` shared by the writing parts of its stage, or `part_budget_usd` on the film when a person sets it. That field is left out of the stage hashes, because raising it is the way out of the hold.

THRESHOLD CHANGE (new and stricter, nothing looser): `("earshot-sound-engine", "film_lufs", -14, -14)` is added to the bounds table in `acts.rs`, so a looser number in the pack would hold. No pin and no pack changes. Countersign: the lead, who did not write it, after the review at this head.

Two existing expectations changed. The two tests that count repairs now name the one try on the next model up (still exactly 2 repairs, then hold), and a finished run makes 38 calls instead of 37, the mix job at $0.

## How it was checked

`scripts/heavy cargo test -p juju-conduct` at f0490fe, on integration head 2c640bd: **212 passed, 0 failed** (Measured). `gate_checks.py` diff, body and tree: open; no key shapes in the added lines, nothing loosened.

17 new tests in `tests/runtime_loop.rs`. All were red on the integration branch's own `src` (0 passed, 17 failed; one row each in `runs/decision.tsv`, lane `conduct`), and one unit test for the step limit. Every call is the Mock's: $0 spent.

Changes made on purpose to break the code, each caught by a new test (Measured):

- rejected quotes not looked for in a text that was put back
- put back in memory only, not on disk
- the round refunded when a repair is put back. First run: it looped for ever, and its test held the heavy lane until the lead stopped it. That is why the step limit exists; with it the same change ends red in 8 s
- the promise of the one try not looked up

## Not verified

- No real model, engine or listening model has run through this; the crate has no network code and refuses any provider that is not a Mock.
- No real engine does the `mix` job or writes `sound/earshot.json` yet. The film lane's `runs/films/ten/earshot.json` has three of the fields and would need `integrated_lufs`, `mix_sha256` and `heard`.
- Loudness is read from the receipt. The conductor does not measure it.
- The receipt counts synthetic cues. It does not say that every cue of the film was listened to.
- A resume that finds some of a round's acts repaired and others not asks the critics about a mixture the first run never made, so a later replay can hold with "gone" replies. It was so before this change.
- `docs/poteto/runtime-loop.md` still says "not held": it is in #11, not on this branch.

🤖 Generated with [Claude Code](https://claude.com/claude-code)


## 11. Run-until-done contract: worker contract, exit predicate, attempt log

## What it adds

- `WORKER.md`: the contract every agent obeys, with line 1 of every kickoff. `AGENTS.md` and `CLAUDE.md`: the front door.
- `docs/poteto/`: five playbooks (lead, hillclimb, live proof, the loop inside Juju, the one report), written from pstack's originals for one Mac and a fixed purse.
- `scripts/exit-predicate`: 23 clauses read from receipts on disk; a clause that cannot be read is false; film receipts carry the film's sha256. `scripts/decide`: one row per attempt.
- `scripts/kickoff-line.py`: a SubagentStart hook that tells every sub-agent and workflow agent (seen in 4 of 4 workflow agents' transcripts), and a PreToolUse hook that puts the line first on kickoffs. `scripts/heavy`: four jobs side by side, first come first served, memory guarded, each with a time limit, one shared build folder (Ambi, 20:04). `scripts/light`: two at a time for click walks and probes. `scripts/pins-check.py`: recomputes the pins without a build.
- `scripts/test_contract.py`: 62 planted faults and controls for those tools.
- Pack `juju-poteto-autopilot`, with its three rows in `reach.rs` and its 18 pins. `ask-juju` gets section 0.
- ADR 0018 (the order, what it supersedes, what was found) and ADR 0019 (Ambi's answers on what ready means).

THRESHOLD CHANGE: `scripts/heavy` is looser on Ambi's order of 20:04 ("remove 1 job at a time limit"): three slots become four, and an empty pool takes a job whatever the memory. Nothing else is loosened. `scripts/gate.sh` changes one line (the build folder it uses; what it checks is the same). `pins.txt` gains the 18 lines of the new pack and no existing line changes. `scripts/heavy` goes from 3 slots to 4 with a load guard, a time limit and a fair queue, on Ambi's order.

## How it was checked

- `python3 scripts/test_contract.py`: 62 of 62 hold, with the false passes the reviewers of 2611544 and 181246f showed, and a control that a true film passes all 11 film clauses.
- `python3 scripts/pins-check.py .`: 784 of 784. `gate_checks.py` tree, diff and body: open.
- A kickoff without the line reached a fresh Haiku worker with the line first; two later workers of the old lead also open with it (read from their first message).
- `scripts/exit-predicate` ran on the main checkout: 3 of 23 true.

## Not verified

- `scripts/exit-predicate walk` and `gate` have not been run end to end.
- Hermes, Codex and agents started by a program are reached by text only; no hook covers them.
- Two findings belong to other files and are open: `pr_state.py` PROTECTED is shorter than WORKER.md's list, and `purse.py` opens the voice gate on an empty LEAD-PASS.json.
- Rules R9, R10 and R12 of the pack describe the runtime loop; no merged code holds them yet.
- The merge door needs docs/MERGE-LOG.md on main, which lands with PR 10. No workflow runs test_contract.py yet. Not every fix has its own planted fault.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

## 10. Integration 24 Nov

## What it adds

One branch that holds everything finished on 24 Nov 2026, with nothing left out of the tests.

- **Pull requests 1 to 9, merged in number order.** No conflict came up. 9 was red alone because its new skill pack `pr-gauntlet` had no row in juju-conduct; that is fixed here.
- **Live state of the folder, 16:46 EAT:** crates core, skills (51 packs), script, conduct, reliquary, absorb and next; decision records 0010, 0012 and 0014 to 0017 (0011 and 0013 do not exist); scripts (meter, route proof, purse, heavy; no key); `design/looks`, `design/fonts` with their licences, palettes and camera motion; the round 2 rooms, kit tools, flows and wiring; the swarm toolkit.
- **juju-stage** is commit 669deb1 of this branch: the live folder as it stood at 16:29 EAT, quiet for 17 minutes when it was copied at 16:46 and still the same at 16:58. The Films fleet has edited it since; that newer state is not here. main's copy has tests that never compiled on GitHub, so there was no older green state to fall back to.
- **juju-next** joins the workspace. It is the live state of 16:39 (copied 16:46, unchanged at 16:58) plus fixes: it was its own workspace root, its glue pointed at one Mac, and its test file did not compile (an index inside `json!`). Commit 669deb1; it needs `runs/packaging/check.py` and `runs/fresh`, which come with it.
- **A skill pack with no row** in `reach.rs` warns and places itself by the `stage` word of its own `skill.json`. Where a model writes at that stage its fragment is sent; anywhere else, or when the pack is broken, it waits for a builder. Its rules are listed on the receipt as not enforced. It never stops the app or holds a film. A pack that was reviewed still stops the app when it is changed, renamed or gone.
- **Critics that say nothing hold.** Every critic of every stage (9 critics at 5 stages) is run against 17 answers that judge nothing (empty, blank, `{}`, `null`, prose, cut-off, error bodies, HTML and others), a blind answer, a call that fails and a call that times out; both viewers against 21 answers, a failed call and a timed-out one. A last test fails when a stage with a critic is left out.
- **Round 1 findings** (commits ee7558c, 0ba8749, 37f8662 and 2c640bd): what was fixed and what was not is in the comment of that name below. In one line each: one `Skill::sha()` over the whole pack for pins and `input_sha`; the money gate uses a reservation up once, prices the body itself and writes the row; one Vessel, one Rights shape and one clock door in juju-core; a stage's behaviour in one place a stage; locks, deadlines and honest failures in reliquary, absorb, next and conduct.
- **The gate** runs every crate and app on GitHub, in two halves side by side (`conduct` and `rest`), the panic tests once more as a release build, and the Python that holds money on stand-in servers; on main too, so main keeps a build cache. The merge train leaves no crate out either. From a cold start 12 min 59 s became 7 min 5 s.

## THRESHOLD CHANGE

**How each row was told.** An independent reviewer (opus-ready, 24 Nov about 19:20 EAT) ran main's linter and this branch's linter (2c640bd) on the same texts: 1,188 planted ones (every row's example and clean sentences, old and new, every sentence of `gates.rs`, and near misses the reviewer wrote) and 8,396 three-sentence windows of 31 published transcripts on disk. "Planted" and "windows" below are texts the old row hit and the new row does not; windows overlap, so one sentence can count three times. The reason for every healer row is in `clean-calabash-42tic-healer/SKILL.md` lines 71 and 72 (it flagged plain writing), and each has sentences in `gates.rs` that must still hit. Measured: no row hit fewer of its own planted examples.

Looser, healer rows (18):

- `A-its-not-x-its-y`: looser. A sentence with a proper name after `not`, a thing that looks or seems like another, and a kind told from a kind pass (This is not the road to Nairobi). Planted 9, windows 5. It also lets through: It is not the Nile. It is your own blood.
- `A-isnt-x-its-y`: looser. Only the looks-like and kind-from-kind exits open (the proper-name exit reads the word `not`, which `isn't` has not). Planted 2 (two sentences written after the first set), windows 0.
- `A-the-problem-isnt`: looser. A problem that is hard, easy, new, old, small, fixed and so on passes (The problem is not hard). Planted 5, windows 0.
- `A-paragraph-opens-on-denial`: looser. The exits of A-its-not-x-its-y, plus a boundary (not a reason to, not an excuse to, not medical advice). Planted 11, windows 0.
- `A-comma-not-tail`: looser. More instructions (Use warm water, not hot), not a promise or a cure, a sentence that opens on he, she, I or we, and a proper name after `not`. Planted 14, windows 6. It also lets through: I trained my body, not my mind.
- `A-did-not-echo`: looser. It needs a link word after the object (for, to, as, in ...), and a reason in the pair (because, since) passes. Planted 5, windows 0.
- `A-not-verb-echo`: looser. I or we do not know, think, see, remember, believe, understand, recall or hear, and a next sentence that opens on nobody, no one, none, nor or neither. Planted 9, windows 9.
- `A-stop-start`: looser. The two words must be the same, or both sentences three words or fewer. Planted 6, windows 0. It also lets through: Stop chasing women. Start building the man you were meant to be.
- `A-all-along`: looser. It dropped "with you" (The ring was with you all along). Planted 3, windows 0.
- `B-to-be-honest`: looser. A stop or a short list of openers must follow (To be honest with a child passes). Planted 4, windows 0.
- `B-first-second-third`: looser. Each first point must open on why, what, the, we ... so plain steps pass (First, boil the water). Planted 4, windows 0.
- `C-nobody-tells-you`: looser. Past tense with us, and most people never with because or since, pass (Nobody told us the bridge was out). Planted 6, windows 0.
- `C-everything-changed`: looser. A stop, forever, for you, about, or a person's knowing must follow (changed everything in Ireland passes). Planted 8, windows 0.
- `D-crucial`: looser. Crucial to turn off, shut, check, cut and the like passes. Planted 5, windows 0.
- `D-elevate`: looser. A person or an abstract noun from a list must follow. Planted 6, windows 0. It also lets through: Fasting elevates mood.
- `D-revolutionary`: looser. Revolutionary war, army, papers, movement, era, press and the like pass. Planted 4, windows 0.
- `D-something-in-you`: looser. Something in him of his grandfather passes. Planted 3, windows 0.
- `E-quote-straight`: looser, the widest of them. Words in straight or curly double quotes said by I, he, she, we, you, a family member or a common role (teacher, doctor, coach ...) no longer hold for a person. Planted 10, windows 26. A named source a sentence earlier is enough to open it (Seneca wrote about this from exile. He said, "..."). The claims gate still asks any quotation of four words or more for a source that holds it word for word (`claims.rs:148`, `house/claims`); on those sentences that second net was read, not run.

Looser, and outside what the body check can see (code, or `crates/juju-script/rows/extra-tells.json`):

- `A-split-not-it-is`: both ways. Looser by the proper-name, looks-like and kind-from-kind exits (planted 13, windows 9; it also lets through: The enemy was not Babylon. It was the mirror). Stricter: it now reads was never the, was never a (planted 2).
- `A-never-the-problem`: looser. He, she, I, we or they as the subject passes (He was never the problem in class). Planted 4, windows 0.
- `D-scare-quoted-buzzword`: looser, in `lint.rs` (`NAMED_AFTER`): a naming noun right after the quoted word passes (the "windowpane" test). Planted 6, windows 0. It also lets through: the "miracle" method.
- `E-comma-anaphora`: looser, in `lint.rs` (`PLACE_OPENERS`): with your fingers, with your palm. Planted 5, windows 0. It also lets through: With your fear, with your shame, with your hunger.
- A denial is allowed when one of the three sentences before it states a belief (it was one sentence), and when a source passage holds the contrast word for word (`lint.rs`, `BELIEF_BACK` and `sourced`).
- A stated belief counts as a first-minute turn, and a passage shorter than the seed's plant-by time is not asked for link notes (`story.rs`; both are named in its output for a person).
- In `claims.rs`: the ledger may say that two amounts are one (three days, 72 hours) with a reason, `a day` answers for `one day`, and Nobody, Everyone, People and fourteen more sentence openers are no longer names. Many more words ask for a source now, so the gate as a whole asks for more.
- The rights check (`reliquary/src/pixels.rs`, `agency`): looser than main's. An agency name inside an XMP namespace, right after `<`, `</` or `xmp.`, or before `gift`, is software and passes; main's copy flagged every occurrence. A credit with a colon (`Getty Images: J. Smith`) still hits, as on main.

Neither way, or stricter:

- `B-sit-with-that`: stricter. It also reads sit with it, sit with this, and for one breath. Planted 2 more hits, none lost.
- `E-triple-comparative`: both ways. Stricter by seventeen more words and far, much, even. Looser when three physical comparatives end on than and a thing (stronger, lighter, and cheaper than chain). Planted 1 gained, 3 lost, windows 0. It also lets through: stronger, faster, and harder than the world.
- 21 new healer rows: stricter.
- Round 1 tightened six of the rows above again (commits ee7558c, 37f8662); the four sentences the reviewer found hit again (run).

Other thresholds and gate files:

- `max_still_s` in juju-stage's `gates.rs`: looser, 7 to 20 seconds. The brief says 20 (line 1244) and docs/STAGE-FORM.md line 42 says so now. No test of `gates()` is in this branch; the patch for the Films fleet has one.
- `scripts/prices.py`, `scripts/purse.py`: stricter. A paid body is read to its last field; a field, part, address, resolution or plugin that is not named is refused; a picture is a picture only as an `image_url` part that carries its own bytes; what is sent is the JSON that was priced (40 planted bodies in `test_money.py`, red on ba9b9b1). Two rounds of one review found the class; the second is closed by naming every field, not by another list of exceptions. Lead's exception to ADR 0020 rule 3: this pull request only carries the trunk, so it is repaired in place.
- New gate files, all stricter (from #11): `scripts/exit-predicate`, `scripts/test_contract.py`, `scripts/pins-check.py`, `scripts/decide`, `scripts/kickoff-line.py`; `scripts/pr_state.py` is new in #9. `.gitignore` hides the spend ledger `runs/meter/*.jsonl`; it was never tracked on main and stays on the Mac.
- A whole new skill pack: looser. It warns where it used to stop the app (two old tests that asserted the stop now assert the warning).
- juju-next's own cap of 0.06 US: looser. It is a UTC day's now and was a life's (`scripts/prices.json`).
- `gate.yml`: lines removed, and stricter in effect. `on: [pull_request]` became pull requests and main; the one `rust` job became two halves side by side, `--exclude juju-conduct --exclude juju-stage` in one of them because the other runs exactly those two; the old `--exclude juju-shell` is gone, so the shell is tested too. The `rust` check is still one name, red when any part is.
- `gate.sh`: stricter. The line removed is `--exclude juju-shell`.
- `gate_checks.py`: stricter. New on main; the lines the check flags in it are its own pattern for loosening lines and its own words about ignored tests.
- `speed.rs`: neither. A timing print marked `#[ignore]`; main's copy did not compile. It asserts nothing, so the fast drawing pass has no test.
- `pins.txt` is new in git. Its pins are of the whole skill file now, and its header says who has not read which packs.
- Stricter: every audit that compared modelled fields compares the whole file; `impeccable-juju-ui/R2` is a gate at 30 words (24 on a phone), was craft at 40; the drawn gate (`max_bare`) is new.

Rows and pins written here for a person to read: `crossroads-chain-outliner` R9 to R15 (the ladder, builder only, off for titles in its own data), `evergreen-brand`, `idea-before-picture`, `no-tell-frames` and `pr-gauntlet` (builder only); `pins.txt` lists at its head what nobody but its builder has read.

## How it was checked

- GitHub's machines ran the Rust tests: 409 passed, 0 failed, 1 ignored (a timing print) on 2c640bd. Rounds 1 and 2 of this set were green; 37f8662 was red on one test that had been a coin toss: a time read back one step off, so juju-next refused its own file (fixed at the root in 2c640bd; how often it happened was not measured, and the rate in that commit's message is a guess). On the Mac only `cargo check` and builds of juju-conduct: `pins` prints exactly the pins of `pins.txt`, and `plan` answers with no error and no warning.
- Python, on this Mac and in the gate: 29 tests of the book, the gate and the paid door (made-up keys, stand-in servers, no cost), 47 of the freshness meter, 6 of the gate's own checks. `route_proof.py` was not run against a real service.
- The old and the new linter side by side on 9,584 texts (the counts under THRESHOLD CHANGE). Rust, on the Mac, by the reviewer; every changed row and every unchanged one.
- `gate_checks.py tree`, `diff` and `body` against origin/main: open. Each commit's staged diff was searched for key shapes; none.

## Not verified

- juju-next: `deal` on a fixture and the reading of recorded listings ran on GitHub. `read` and `add` still call yt-dlp and ytlocal by paths of one Mac, and a real `deal` also needs `runs/meter/cap.json` (not in git), the gate on port 4610 and the keys. Its Python glue imports `runs/packaging/check.py` and `runs/fresh/meter.py`. The live folder's juju-next has moved on since (17:43).
- **The money fixes protect nothing until the gate is started again from them**: the purse on 4610 is the copy of 16:50.
- **juju-stage is the copy of 16:29 and still has the render blocker** (a lawless film passes when it is rendered again). The patch is for the newer live copy, in `runs/pr/for-films.md`; it type-checks there and none of its tests has run. The same copy has no lock on its pieces folder, waits for ever when a drawer panics (the comment in `Cargo.toml` line 16 says otherwise), and writes `--part` over the finished film.
- 13 packs cite files under `runs/` that are on the maker's Mac only; each says so at its end now.
- **The rooms are drawings made before the laws of this pull request, and break some of them**: 16 of 20 pages carry or draw from the first film (ADR 0012.7), `pact.html` and `cauldron.html` open on a 50 minute length (ADR 0014.1), sample tags and sentences remain (ADR 0009), 494 of 653 controls are cut (ADR 0014.16), their pictures come from git-ignored `runs/stage-y`, and `shot.py` reads a page's first state only. The lines are in `runs/pr/for-app.md`.
- No pack places itself today: all four packs that had no row got rows here, and only made-up packs in tests take that path. `evergreen-brand` (stage `crossroads`, with a fragment) would have placed itself at stage 1; its row makes it builder only, because no stage asks for its form. That is the lead's to accept or reverse.
- `crates/juju-stage/fixtures/fonts/OFL.txt` was put together from the font's own name table and the standard licence text.
- The four critic holes were not reproduced on the old code; the tests ran only against the new.
- **Not in this branch:** juju-cli and juju-serve (both began after 16:50 and are being written; neither has ever compiled on GitHub). `spirit-tongue` was being edited at 16:56; this holds the 16:46 state.
- Over 1 MB, so left out: `mockups/r2/light.js` (make it with `python3 mockups/r2/build/pack.py`; without it the rooms draw no light maps) and `design/looks/sources` (one map of 1875).
- No film was rendered and no screen was looked at here. `scripts/gate.sh` (screens and truth checks) was not run.
- juju-absorb reads on-screen text with macOS Vision and uses the hardware encoder on the Mac only; GitHub runs neither.
- A pack that places itself has its fragment sent to the writer before anyone reviewed it. If its words ask for fields the stage's shape refuses, the film is repaired and can hold on the shape. Today the only provider is a Mock.
- New conduct rules with no code yet, listed on receipts as not enforced: ladder, narrators and looks (`ghost-onions/R10` among them), and four more that film stages meet: `crossroads-chain-outliner/R8`, `diviner-12-equation-mint/R11`, `shadow-sieve-flop-differ/R12`, `voice-vm01-elder-brother/R8` (`rising-river-tam-expander/R15` has code since round 1).
- The body check reads `skill.json`, a few named Rust files and the gate's own files. It does not see `lint.rs`, `story.rs`, `claims.rs` or `extra-tells.json`, so a loosening there is named only because a person looked.
- The live folder still holds the old juju-conduct, juju-next and five `SKILL.md` descriptions; the fixes of this branch reach it only when main is brought into it. A fleet's next save must not undo them.

🤖 Generated with [Claude Code](https://claude.com/claude-code)




## 9. PR gauntlet: merge train, gate checks without a model, review states

## What it adds

- **Merge train** (`.github/workflows/train.yml`, `.github/scripts/train.py`): on every pull request update, push to main, or on demand, it merges main plus every open non-draft head in number order and gates the result on GitHub's runners. Cargo runs per crate; a crate that does not compile on main is known red, one that stops compiling on the train is a break. When the train is red it leaves suspects out (in parallel) and names who broke it. Each head gets a commit status `train`; a new commit has none, by construction.
- **Checks with no model** (`.github/scripts/gate_checks.py`, job `checks` in `gate.yml`, `gate-body.yml`): flows, skills and copy list are valid JSON; every Python file compiles; every skill pack is valid and links into both harnesses (real `link-skills.sh`, throwaway HOME); every workspace crate has a test; no file over 1 MB; no key shapes on the added lines; the body has the three headings; a loosened skill threshold or gate needs the words THRESHOLD CHANGE.
- **State labels** (`scripts/pr_state.py`, `pr-state.yml`): needs-review, reviewed-1, reviewed-2, train-green, ready, computed from review comments that carry the head they reviewed. A pull request that touches the gate, the train or `pr_state.py` is ready only with the lead's approval. CI runs main's copy of the script.
- **Merge log** (`docs/MERGE-LOG.md`): one line per merge, written by `pr_state.py merge` (the lead runs it); `--fixes` marks a repaired one; `streak` counts towards the 20.
- **Skill** `pr-gauntlet`: how to review in two lenses, answer findings, close, and stay fast.

**THRESHOLD CHANGE.** Two allow lists are new: `no-test-ok.txt` lets `apps/juju-shell` have no test, `size-allow.txt` starts empty. This branch also carries PR 1's looser `gate.yml` (stage and reliquary block only a PR that touches them). `gate.yml` here only gains a job; nothing in it is removed.

## How it was checked

- `gate_checks.py tree` and `diff` on main and all eight open heads: only `juju-shell` has no test (now on the allow list). `body` on all eight: headings pass; the threshold check flags every one of them, because each carries PR 1's looser gate without the words THRESHOLD CHANGE.
- `train.py plan` on the live repo (read only, from a scratch clone): all eight merge cleanly in order. `run` without cargo: no new red. `decide` and `report` with injected failures: the right PR is blamed, innocents come out green, a trigger that broke the train exits 1.
- `pr_state.py status` on the open pull requests (read only), comment parsing, log lines and the streak count.
- The checks of this pull request.

## Not verified

- The merge train's cargo steps on GitHub before this run; `merge` beyond a dry run (the lead's to run); `sync` writing labels.
- `pr-state.yml` and the train on other pull requests start only once this file is on main, because those events run main's workflow files.
- "Different reviewers" are different names, all posting through one GitHub login. Nothing proves they are different minds.
- A threshold can be loosened in Rust constants, flows or prompts without the words; the check reads `skill.json` numbers and gate files only.
- Screens and truth checks still run only in `scripts/gate.sh` on the Mac, not in CI.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

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
