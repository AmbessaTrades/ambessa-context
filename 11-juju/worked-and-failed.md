# What worked, what failed, what it taught

As of 08:15 EAT, Wed 25 November 2026. Covers 24 Nov 13:45 to now. Newer: [../10-now/now.md](../10-now/now.md), every run: [../10-now/films.md](../10-now/films.md), every measured attempt: [../10-now/attempts.md](../10-now/attempts.md).
Pictures: library sections "Juju — films it made by itself", "Juju — worked", "Juju — refused or failed", "Juju — the app, pressed for real".

## The short answer

Juju now makes a whole one-minute silent film by itself, from one command. **None is good enough to publish.** No voice in a real film, nothing at 10 minutes or longer. The finish check is 2 of 23.

## Breakthroughs

| When | What | How we know |
|---|---|---|
| 24 Nov 15:24 | Map and space clips drawn by the engine | **Ambi:** "they're both great". He named jump cuts, plain type, text habit |
| 24 Nov 15:27 | `juju-stage`, the drawing crate, passes its tests again (33 tests) | Measured |
| 24 Nov 22:50 | Pull requests 1 to 12 in main after a day of none | Measured. 13, 14, 16 to 20 followed; 15 closed |
| 24 Nov 23:45 | Ambi names the real hole: we cannot take a film apart | He sent the repo rea-video; ADR 0021 |
| 25 Nov 02:34 | Skill `film-harvest`: a fresh agent took a 20 s cut apart with the skill alone | 6 of 6 on its self test, scored by its maker |
| 25 Nov 03:39 | The 60-film study found **why our films are weak**: the engine can draw 12 of the 40 picture moves those films use, 12% of the galactic-empires film's own argument | Measured over a judged match. Ten missing primitives are ranked in [engine-gaps](engine-gaps.md); the top seven reach 79% |
| 25 Nov 03:41 | Our own eye sees motion: 35 of 35 drawn events against rea-video's 10 of 35 | Measured on the windows it was built on; weaker on unseen film. [harvest-score](harvest-score.md) |
| 25 Nov 05:18 | A written film language with closed fields, so a cheap model can fill it | 64 of 64 hand-marked rows expressible. [harvest-language](harvest-language.md) |
| 25 Nov 06:45 | **First real film out of `juju make`**: Ottoman Empire, 60 s, silent, 11 of 11 stages, 0.068 US, 17 machine minutes | Picture 200. Lead: works, not good |
| 25 Nov 07:40 | Second one with words on screen (`otto-chron-2`), 14 minutes | Picture 199. Lead: not good |
| 25 Nov 08:08 | **First new subject reaches a file**: Mughal Empire, 60 s, 0.009 US, 16 minutes | Picture 252. Read from its own report; looked at only by the writer of this page: same tiny words and bare grey land for the first 14 seconds |

## Failures and refusals

| When | What | Why | What changed |
|---|---|---|---|
| 24 Nov 13:51 | Storyboard pictures made of code shapes | **Ambi:** "Both of them are garbage", "Claude made this" | ADR 0012: no stand-in drawings |
| 24 Nov 13:54 | The Jade Rabbit Hole drawn style | **Ambi:** only Claude could make it; the software runs on cheap models | Dropped. Looks are chosen by leverage |
| 24 Nov 14:20 | Blind test: two judges marked 53 of 53 of our frames machine-made and 0 of 40 published | Narrator line at the bottom, text on busy pictures, hard map edges, all-sepia | ADR 0014 locks |
| 24 Nov 14:33 | Sheet of 36 palettes | **Ambi:** "Just like some slideshows. 2017" | Cut to 11 |
| 24 Nov 14:57 | Rip-any-video job | Too wide, too early | Stopped; map and space engines first. Came back at midnight as the harvest |
| 24 Nov 16:38 | The app: he pressed it for two minutes and found the PIN fifth circle, the floating cat, cut cards | Rooms were static pages; nobody had pressed them end to end | ADR 0017, button census: 573 controls, 112 real ([buttons](buttons.md)) |
| 24 Nov 16:44 | Agent counts told to Ambi were inflated | 40 said, 8 to 12 live | Law: live, open and queued stated plainly |
| 24 Nov 18:35 | **Audit of the day**: 2.44 billion tokens, about 2,600 US of model work at assumed list prices, 3.26 US on Juju's own models, 0 finished films | Studies ran before the chain existed; checks nothing called; long-lived agents re-reading | [audit](audit-2026-11-24.md) |
| 24 Nov 20:57 | Script line "the sun gave nothing" | **Ambi:** "What kind of slop is that?" The lead and two Claude listeners had praised it | Job stopped, no voice bought. [ambi-ear](ambi-ear.md): a judge is trusted only after it refuses that line |
| 24 Nov 22:19 | The job queue starved itself: 36 jobs behind one | A "wait if the Mac is busy" rule | Rule removed; eight side by side with a memory guard |
| 24 Nov 23:17 | The McDonald's dot strip | **Ambi:** "the worst looking thing ive ever seen". Later: no trace of the film it was meant to learn from | [ambi-eye](ambi-eye.md): judges must refuse it unprompted. Take apart first, draw second |
| 25 Nov 01:15 | Eleven films decomposed at once; load 158 to 190, 10 GB swapped | A limiter that did not limit | One film at a time |
| 25 Nov 02:35 | Facts lane: 2 of 15 facts wrong, 6 pins misplaced (Paris near the Danube's mouth) | Weak own check: accepted 6 of 8 planted errors | Repaired; 101 of 101 planted faults refused, but its full bar is not called true |
| 25 Nov 03:41 | rea-video as the whole answer | 59 minutes for 40 s of film; blind inside code-drawn motion; 0 of 9 on a silent map | Kept for looking at short windows only |
| 25 Nov 04:15 | Fast runner promised 3 times faster | Measured 1.2 times | Said so |
| 25 Nov 06:45 | House strips: Orion refused by four judges, lungs partly, Egypt showed modern lakes under "1400 BCE" | | Repaired by 08:05, waiting for fresh eyes |
| 25 Nov 07:40 | Nine new subjects tried, one file (Mughal) | Titles that break their own rule, scripts with lines no fact supports, too few dated events with a place, camera faults | Owners on each |

## Laws this produced

1. Films come out of Juju, with Juju's own models. What an agent makes by hand is only a measuring stick.
2. Take the film apart before drawing anything that claims to learn from it.
3. A judge earns trust by refusing what Ambi refused, planted, unprompted. No judge shares the maker's taste.
4. A check that passes easily is the first suspect.
5. One unit, one pull request, one review round (ADR 0020).
6. The proof is a whole film of 10 minutes or more with a voice, never a clip (ADR 0021).
