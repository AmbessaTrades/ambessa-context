# Test film run: minting, voting, research and script writing

As of 13:10 EAT, 24 Nov 2026. Source: test-film workflow e65c58b0 (mint, vote, research, outline, outline critics, act writing), file G.

> **Stopped.** Ambi said software comes first, and the job was stopped. The files from this run stay only as test material. No film was finished, voiced or pictured.

## In short

- Three mint runs produced 17 title cards. Three voters ranked them. One voter killed two cards; the other two killed none.
- Research gave 75 entries across three agents. A script matched quotes to downloaded texts. Most modern-evidence entries rest on abstracts only.
- Two critics attacked the first 11-act spine with 24 findings (7 blockers). The maker rewrote it as 8 acts at 52:00. Acts 1 to 8 were written (5,892 spoken words). Act 9 was skipped because the spine has no act 9.
- What worked: quote checks by script, a claim id on every line, and a critic pass before acts were written. What failed: the middle sagged, the cold open told the story, and several lines said more than their sources.
- Open: no voice, no pictures, licences unchecked, and the 30-fact count was never built. At 142 words a minute the script runs about 41 minutes, not 52 (our arithmetic).

## What was done

### Minting

- Mint runs gave 6, 5 and 6 cards. Each card has a title form, a donor video from the outlier list, one new claim, a thumbnail idea and a reach estimate.
- Each card passed two gates the maker set: the title and thumbnail share no words, and the subject is one a stranger can picture.
- Each card cites a YouTube search run on 24 Nov with a result count, a median view count and a channel count. Searches returned 13 to 40 results.
- Reach tiers (4 or 5) are estimates. None was measured.

What it taught:
- Check donor numbers on the live page, not the library file. One donor showed 38,128 views in the library but 147,159 live, about 3.5 times the pool median. The library row had made it look like a flop.
- A title that keeps the donor's frame but swaps the subject is a grey area. Voters split on it (see below).
- Demand evidence was thin for most cards. The strongest pool signal came from a crowded pool with high medians, not from a niche with low supply.

### Voting

- Three voters ranked all 17 cards. Voter 2 killed card 7 (a Buddha rival title) and card 10 (Oppenheimer). Voters 1 and 3 killed none.
- Voter 2 said six of card 7's nine title words matched a donor title, with only the subject swapped. Voter 1 called donor frames sanctioned grammar. Card 7 sat mid-field for voters 1 and 3.
- Voter 2 also flagged that cards 11 and 16 both use "The ENTIRE ... in 52 Minutes", so only one should ship.
- Card 2 (Pharaoh's day) sat in the top five for all three voters. Card 11 (Journey after death) was first or second for two voters.
- Card 10 was last for voters 1 and 3.
- Voter 3 ranked from card text only. It says it did not open the brief, the decision records or any source. Its ranking therefore carries no evidence weight.

What it taught:
- Voters need the brief and the sources. A ranking from card text alone reflects wording, not proof.
- Kill rules need one agreed reading. The brief allows a shared frame; one voter read that as copying.

### Research

- Three research agents wrote 25 entries each.
- Research 1 covered classical and sacred texts. A script checked each quote word for word against the downloaded text. Quotes are 20 to 80 words.
- Research 2 covered 25 modern studies. Twenty rest on abstracts read through the PubMed record. Five were read deeper.
- Research 3 covered ancient and medieval deathbed and afterlife accounts. Twenty-three matched exactly by script. One was cleaned of line-break hyphens. One was read by eye from a scan.
- The Project Gutenberg site failed or returned a maintenance page for part of the run. Mirror copies were used, and the maker says the mirror URLs are given.
- Four searches did not show the Er and Achilles pairing. The maker wrote "not found", not "never seen". An 1927 work already set the Er tale beside a Tibetan rebirth choice.
- Disputed findings were kept disputed. A 1994 regret study (84 percent regret inaction) was not repeated in 2023 (51 percent action, 49 percent inaction). Near-death cause figures from different groups were not averaged.

What it taught:
- Quote checks by script work when the source text is local. They fail silently when the host is down, so check the source copy first.
- Stay with "not found" for novelty claims. Four searches are a sample, not a proof.

### Script writing

- The first spine had 11 acts and 40 seconds of cold open. The maker checked 56 ledger rows and 33 exact quotes. 41 new passages matched the Gutenberg texts word for word.
- Two critics read the spine. Findings: 24, with 7 blockers and 17 important. Full findings are under "What critics found".
- The rewrite gave 8 acts, 52:00 exactly, 76 timed picture states and 38 exact quote spans. The maker's delete test put 0.89 of links as causal. Six links failed and were kept, each with a reason.
- Acts were written with 716, 753, 704, 746, 747, 727, 752 and 747 spoken words. That is 361 lines.
- The juju-script lint returned 0 hits on 125 rows. It ran on a scratch copy of the pack, because the built binary rejected a newer field. A fresh build failed offline.

What it taught:
- Writers drift past their sources. Several lines added claims no ledger row holds. A critic pass caught them only when it read each line against its row.
- Lines should carry a claim id. Lines with no number, name or quote may carry none, but the count should be reported.
- Set spoken words per act against the act's time slot. Act 3 had 704 words for a 220-second slot, about 4:57 at the pack's rate.

## Breakthroughs

- **Plato's text limits the film's core claim.** Research 1 found that Plato says "the greater number" of those who chose badly came from heaven, not all of them, and that chance sets the lot. The spine adopted the softer wording. Evidence: exact-match check of the quote.
- **Plato knew the Achilles line.** He strikes it out at 386c and uses it again with approval at 516d. Evidence: exact-match check. It does not prove he meant it at 620c, where he gives "recollection of former toils" as the reason.
- **The critic pass caught seven blockers before any act was written.** Evidence: two critic runs, 24 findings.

None of these is proof of a film's appeal. The pool data is a search sample, not a test audience.

## What critics found

Critic findings and the maker's status claims. "Fixed" means the maker says the rewrite fixed it. No critic re-checked the rewrite.

1. **Cold open told the story.** It named the book, the payoffs and the last man's pick in past tense. A critic found the words ran ahead of the pictures. Status: fixed (maker reports present tense, stopping at the paradox).
2. **Acts 4 and 5 sagged.** The road stopped for 9 minutes 30 seconds, 18 percent of the run, with no person moving. A delete test showed no event would break. Status: fixed (maker reports act 5 removed and the struck line folded into one 60-second proof).
3. **Act 1 was a topic.** The hospital count and a Roman board game ran 4:20 before the road started. A critic said a 2021 study was used as judge over a tale. Status: fixed (maker reports the road starts at 2:40, with the hospital count and Kanus cut).
4. **The climax's last shot contradicted itself.** Odysseus lifts the bundle, then the last shot says the same bundle is still lying there. Status: fixed (maker reports a second plain bundle).
5. **The act 8 to 9 hinge had a causal hole.** Pain made Ajax bitter, yet the spine used pain to explain Odysseus's better choice. Status: fixed in part (maker marks the difference as our reading; no re-check).
6. **Act 2 made Ani prove the opposite of his book.** The ledger row has the gods pass him. Status: unknown.
7. **Act 3 claimed four things the text does not hold.** These covered tyrants, feeling what they had done, the wait saving them, and an exit from the lower road the text denies. Status: unknown.
8. **Act 5 cherry-picked the Apology.** Socrates lists Odysseus as someone to test, not as a model. Status: unknown.
9. **Act 10 cancelled its own stake and introduced a second Er.** Drythelm was cut. Status: fixed (Drythelm cut); the act 10 question no longer exists in the 8-act spine.
10. **The final dusk-to-dawn reveal was spoiled three times.** Status: unknown.
11. **Overclaims in the closing lines.** A critic said the closing promise drops Plato's condition of wise and diligent choosing. Status: unknown.
12. **The causal score was self-graded.** Seven links were "and then" by the delete test. Status: partly fixed; six links were kept with reasons.
13. **Each act had one world and one moving thing for 220 to 320 seconds.** Status: fixed (maker reports 76 timed picture states, one silent walk over 60 seconds).
14. **Lint false hit.** A raw-ledger check flagged the Achilles line in act 3 because the lint straightens apostrophes in the script but not in the passages. Status: open.

## Numbers

| Measure | Value | Basis |
|---|---|---|
| Title cards minted | 17 from 3 runs | Measured |
| Voters and kills | 3 voters; kills 0, 0, 2 | Measured |
| Pool medians (search samples, 24 Nov) | 143 to 285,281 views across 10 pools | Measured |
| Donor views, Routine video | 147,159 live vs 38,128 in library | Measured |
| Top comment on the lead donor | 272 likes | Measured |
| Research entries | 75 (25 + 25 + 25) | Measured |
| Research 2 abstract-only | 20 of 25 | Measured |
| Research 3 exact matches | 23 of 25 | Measured |
| Spine ledger rows checked | 56 | Measured |
| Exact quote spans in rewrite | 38 | Measured |
| Passages matched to Gutenberg text | 41 | Measured |
| Critic findings | 24 (7 blockers, 17 important) | Measured |
| Spine change | 11 acts to 8; 52:00 exactly | Measured |
| Timed picture states | 76 | Measured |
| Acts written | 8 (act 9 skipped) | Measured |
| Spoken words, acts 1 to 8 | 5,892 across 361 lines | Measured |
| Sag in acts 4 and 5 | 9 min 30 s, 18 percent of run | Measured (from spine timeline) |
| Lint result | 0 hits on 125 rows, scratch pack | Measured |
| Runtime at 142 words a minute | about 41 minutes | Estimated (our arithmetic) |
| Reach tiers | 4 or 5 on all cards | Estimated |
| Causal share after delete test | 0.89 | Judged (maker's own test) |
| Card ranking | card 2 top five for all voters | Judged |

## Still open

- No voice. Spoken pace is unmeasured, so the 41-minute figure is an estimate.
- No pictures. Several Met and Getty objects were named but not opened. The Getty licence and the other picture rights are unchecked.
- Act 9 does not exist. The 8-act spine ends at the river and the waking.
- The 30-fact target was never built. The film clock allows about 10 named sources in 50 minutes, so most research is a bench.
- Two cited works (Bloom 1968 and Planinc) were not read. The novelty claim depends on them.
- James Clay's work is dated 2025 in one file and 2026 in another.
- Second review is missing for act 2, act 3 (the reviewer was rate-limited) and act 8 (not called).
- The act 3 lint false hit is unresolved. A fresh build failed offline.
- Research 3 overwrote a build script that another agent had written in the shared scratchpad. A copy was recovered from that agent's transcript and kept outside the repo. Whether an earlier version existed is unknown.
- The film was stopped at software-first. Nothing here has been voiced, pictured or uploaded.
