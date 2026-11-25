> **State of 24 Nov, 13:10.** Later facts win: [worked-and-failed](worked-and-failed.md), [../10-now/now.md](../10-now/now.md).

# Juju script gates: lint, story, claims, and four attack rounds

As of 13:10 EAT, 24 Nov 2026. Source: workflow a workflow (juju-script build, then attack and fix rounds 1 to 4).

> **Read with this:** rounds 3 and 4 are in pull request 2 (`10-now/pull-requests.md`).

## In short

- **Tried:** a new Rust crate, `juju-script`, with five gates: lint, story, claims, newthing and order. They ran on one trial script, lot-r01. Then writers, a fact forger and a false-alarm hunter attacked them in four rounds, each followed by a fix round.
- **Worked:** the claims gate flags numbers, dates, named sources and quotes that have no ledger entry. Honest sentences cleared it in rounds 2 to 4 (6 of 6, 7 of 7, 7 of 7). Each lint rule ships with a must-hit example and three clean sentences.
- **Failed:** planted false facts got past claims in all four rounds (1, 5, 7 and 5 of 8). Lint flags real reversals, and the story turn check passes on single words such as "wrong".
- **Open:** 12 ordering conflicts are undecided, and no health sign-off exists. Three pack rows (7-word fragment, word map, seed windows) are undecided.

## What was done

**Build.** The crate has five commands. Each prints JSON. Exit 0 means pass, 1 means auto-heal or a hold with the exact defect named, and 2 means bad input. One additive function in the skills library returns a skill's raw JSON, because the existing type dropped a key. 29 tests passed. Nothing was committed or logged.

- **Lint** declares 100 rows: 79 from the clean-calabash skill, 6 added by the build in a separate rows file, and 15 banned voice words. Each hit names the sentence id, the row and a positive rewrite rule. Nothing rewrites the text.
- **Story** is ported from the story law. It checks a question in the first 90 seconds, a turn in the first 60 seconds and in every part of 10 or more lines, no 300-second stretch without a question, the title's capitals said in the first minute, a seed planted and later paid, and causal links. A link must quote words that stand in the two lines it joins.
- **Claims** needs a ledger entry for each sentence with a number, date, named source or attribution verb. The entry gives the exact sentence, a passage holding its numbers and names, and a source with book and page or a URL. Health subjects hold until a sign-off exists whose hash covers the exact script and ledger.
- **Newthing** needs one new thing per film, checked against the last 15 films by plain text and shared 7-word runs. The trial shelf was empty.
- **Order** ranks 24 rules: owner locks, then story law, then the voice skill, then the brief. It decided 7 conflicts, left 12 open with both candidates named, and dropped 7 losing rules.

**Trial script (lot-r01).** 124 lines, 475 sentences, 3,591 words, about 25.3 minutes at 142 words per minute (an estimate, no voice clock). At build, lint held on 18 hits in 17 sentences, plus 32 more under open rows. Story held: no seed, no links, no turn in the first minute. Claims held on 96 sentences needing a link. Newthing held: no new thing declared.

**Rounds.** Each attack round had three writers drafting short scripts (222 to 387 words where a count is given, against a brief of about 350). A forger planted 8 false items among honest ledger entries. A hunter tested honest lines for false alarms. Fix rounds added, loosened and tested rules. Test counts after fixes 1 to 4: 39, 51, 59 and 67. The lint row count rose from 100 at build to 137 by round 4.

## Breakthroughs

Two results count as real. Everything else in the rounds is a fix.

1. **Honest sentences clear claims.** The round 2 forger's honest entries cleared 6 of 6 (4 linked, 2 waived). Round 3 cleared 7 of 7 and round 4 cleared 7 of 7. Lint alone flagged none of the round 2 plants. These counts come from the forger's own honest ledger.
2. **Teacher passages pass lint.** The round 2 hunter found 0 of 3 teacher passages passing lint. The round 3 hunter found 2 of 3 passing (human1 and human2), with new drafts each round. Round 4 drafts passed 0 of 3 at the attacker's run; the maker reports 2 passing after fix 4.

Caveat on the round 1 result: claims held 7 of 8 plants because they had no link, but 3 of those 7 were held only by accident (a side trigger, not the rule meant for them).

## What critics found

1. **Forged facts passed claims.**
   - *Round 1:* a fraction written in words ("a third of") and ordinal words were not read as numbers. Fixed: a fraction trigger was added. The round 2 forger no longer lists it.
   - *Round 2:* 5 of 8 passed: an invented "scientists" claim, "a quarter more", a quote put in an ancient author's mouth in straight double quotes, "an hour and a half" where the source says forty minutes, and a paraphrase presented as a quote. Fixed in fix round 2 by quote and fraction triggers and wider attribution lists. The maker reports this.
   - *Round 3:* 7 of 8 passed: "science tells us", "half the men", a saying given to the wrong famous name, a quote whose first sentence had three words, a book title made of common words, and an ordinal hour. Fixed in fix round 3. The maker reports this.
   - *Round 4:* 5 of 8 passed: a spelled-out decade, "an hour and a quarter" for a sourced forty minutes, a saying given to a famous name, "most first-timers" and an invented palm-leaf book. All 3 catches in this round came through side triggers. The maker's fix flagged all 8 planted lines on its rerun. No attacker has retested this. Open: single guillemets and some other quote marks are not read. Double guillemets are read.
2. **Lint punishes the film's own turn.** The trial's central line, that most of the noise is not hunger, trips the denial row. The round 1, 2 and 3 hunters all found this. In round 1 story could not see the same line as a turn, so it failed the turn check. That was fixed by adding a narrow turn list. A sentence the writer marks as a turn now clears the hit, up to two per part. In round 3 lint also marked denial hits as safe to delete. That was fixed. Open: an unmarked reversal still fails lint, and the tool cannot tell a reversal from a tic without the mark. The round 3 hunter judged 4 of lot-r01's 23 hits to be false alarms.
3. **Story's turn check passes on single words.** The ported list holds but, yet, already, half and wrong. Round 3 passed a line that uses "wrong". Round 4 passed "half an hour" and "but". Real reversals with no listed word failed, such as a round 3 opening that corrects an expectation, and a round 4 belief overturned. Partly fixed: fix round 4 counts a stated belief followed by a correction as a turn. Those passes are now listed as "unproven". Open: a judge or a turn mark must decide.
4. **Voice-word rows punish plain uses.** Hunters flagged "rather than", a kettle on a stove, pressure in a cooker or tank, a paper map, "quite", and "would rather". Partly fixed by an allow-list of neighbour words, widened twice. Open: round 3 still flagged a plain kettle instruction. The voice owner decides the list. The hunter also noted that "lift" is a British usage the list does not ban.
5. **Fragment rows double-counted and held scripts.** In round 1 the open fragment row hit lot-r01 30 times, and one run of four was counted twice. Fixed: fix round 1 cut the open hits to 12, and fix round 2 counts each run once. Undecided: the row is still open in the pack, and its effect on a script that obeys the reading lock is unknown.
6. **Taste faults no row sees.** Writers listed 25, 28, 30 and 27 hollow lines that lint did not flag, by round. Examples: stock metaphors, quips after facts, station endings that tease the next station (8 of 9 in lot-r01), and aphorisms. Each fix round refused these as taste. Unnamed authority ("old teachers") was missed by lint. Round 4 found about ten such lines in lot-r01. Fix round 4 widened the rule, and the maker reports all ten caught. No attacker has retested this.
7. **Story holds short, honest passages.** The teacher passages (about 350 words, 155 to 173 seconds) held on question timing and undeclared links. Fixes added a format-fit field (fix round 1), made seed not applicable on short scripts (fix round 2), and made links not applicable on short scripts that declare none (fix round 3). Round 4: human1 and human2 passed story; human3 held on its first-minute turn and question timing. Open: at film length, a missing link still holds.
8. **Probe counts are not rates.** Hunters wrote probe lines to test row edges. Round 2 found 24 of 31 good probes flagged and 0 of 25 hollow probes flagged. Round 3 found 49 of 58 good probes flagged and 27 of 28 hollow probes passing. The hunters say these show where a row is too wide, not how often it fires on normal prose.

## Numbers

| Measure | Value | Basis | Source |
|---|---|---|---|
| Build tests passing | 29 | Measured | build report |
| Tests after fix rounds 1 to 4 | 39, 51, 59, 67 | Measured | fix reports |
| lot-r01 size | 124 lines, 475 sentences, 3,591 words | Measured | build report |
| lot-r01 runtime | about 25.3 min at 142 wpm | Estimated | build report |
| lot-r01 lint at build | 18 hits on 17 sentences; 32 more under open rows | Measured | build report |
| lot-r01 lint later | 21 hits, 14 open (round 2); 23, 4 open (round 3); 30, 4 open (round 4) | Measured | hunter reports |
| lot-r01 claims needing a link | 96 at build; 85 after fix 1; 86 after fix 2 | Measured | build and fix reports |
| Ordering rules | 24 rules; 7 conflicts decided; 12 open; 7 dropped | Measured | build report |
| Planted items passed by claims | R1 1 of 8; R2 5 of 8; R3 7 of 8; R4 5 of 8 | Measured | forger reports |
| Honest sentences cleared | R2 6 of 6; R3 7 of 7; R4 7 of 7 | Measured | forger reports |
| Writer misses (hollow, lint passed) | R1 25; R2 28; R3 30; R4 27 | Judged | writer reports |
| Writer false alarms | R1 9; R2 6; R3 3; R4 7 | Judged | writer reports |
| Hunter false alarms / misses | R1 20 / 10; R2 25 / 11; R3 19 / 10; R4 11 / 6 | Judged | hunter reports |
| Hollow probes flagged | R2 0 of 25; R3 1 of 28 | Measured | hunter reports |
| Draft length | 222 to 387 words (brief: about 350) | Measured | writer reports |
| lot-r01 station endings that are teasers | 8 of 9 | Judged | round 4 hunter |
| Planted items flagged after fix 4 | 8 of 8 | Measured (maker's rerun, not re-attacked) | fix round 4 |

## Still open

- **Pack rows:** the build report says the 7-word fragment row, the word map and the seed windows block a PASS for channel scripts. Some round 3 drafts passed lint anyway, so this is not settled.
- **Owner decisions:** 12 open ordering conflicts, including the seed clock windows, the 7-word fragment row, the named-source cap, the 7-word repeat window, the word map, and whether the narrator may say "I". Ambi decides these.
- **Health sign-off:** none exists. This is correct by design. Code checks a name, date and hash in a file, and cannot prove a person wrote it.
- **Quote marks:** single guillemets and some other quote marks are not read by the quote rules.
- **Judgement items:** stock imagery, rhythm across lines, station teasers and quips have no row. A judge is needed, and none has been built.
- **No heal step:** lint names the rewrite rule, but nothing rewrites.
- **Reading level:** the 7-to-12 reading lock is not measured.
- **Extra rows:** the 6 added rows live in the crate, not the live skill file. Promoting them is the skill owner's call.
