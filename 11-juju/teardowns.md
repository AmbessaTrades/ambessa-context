# Teardown of five films: pacing, palette, quotes, motion, sound, thumbnails, hit pattern

As of 13:11 EAT, 24 Nov 2026. Source: teardown job, `runs/teardown` (five film folders). The job is still running.

## In short

- **Tried:** for five films Ambi named, measure length, views, pacing, palette, quote style, motion, sound, thumbnails, and the channel's hit-and-follow-up pattern.
- **Worked:** Milky Stellar's film (G4w-a8NgnnQ) has frame-level data: 240 shots, a 16-colour palette, motion counts, and a hit pattern over 101 uploads.
- **Failed:** captions were blocked (HTTP 429) for two films, so there is no word-level voice timing. Sound for Milky Stellar is still marked pending.
- **Open:** palette, motion, sound and thumbnails are not measured for most films. Ink Of The Past (HmuQoak_IAg) has only titles and view counts read so far.
- **Owner's rule:** the 90/70/50 echo rule is only partly seen. The data does not show a 90 then 70 then 50 run after any of the 12 hits.

## What was done

Ambi named the five films. Each was matched to a folder by video ID. Only small JSON and Markdown files were read; the 74 KB ASR word list and the image strips were not. The Milky Stellar identity was checked against a similar-titled film (4R7VcBGVLH4), which is different.

## Film 1: "AI's Strange Obsession with Enlightenment" (channel "hands", ZgpMtombn9A)

- **Title, channel, views, length:** 1,257,209 views in the followers record (the channel file rounds to 1.2M). Length 24:29.7. 7,920 subscribers. Upload date 13 Nov 2026 is read from the same record, not from the video record.
- **Type:** faceless essay on AI behaviour. Built from archive paintings and engravings, document cards, quote cards and code-drawn charts. Judged from the sheets.
- **Pacing:** 29 sheets, each spanning about 45 to 70 seconds. Each new picture opens as black line work, then fills in. A chapter card, "Where the Words Run Out", appears at 2:42 with a timeline dot reading "387 — 2026". The film dips to full black at 19:02 while the voice carries on for about 7 seconds.
- **Palette (sampled):** navy base #16163C and #17173D; near-black transcript ground #06071A; mint accents #8ABAA0 and #90C0A5; cream split #EBE3CC; book tan #9B865D. The spiral is orange, mint and cream, and turns red at 18:02.
- **Quote structures (estimated, about 25 quotes):** full quote card on navy, bold white sans, two or three lines in curly quotes. Its grey caps source appears about 6 seconds later. Also dark pill quotes in serif italic; mono transcript cards that type in one phrase at a time; word lists in serif that build word by word, with one orange accent word ("bliss" at 14:54); and single large serif words ("documented", "claimed", "unknown") that stand in for pictures that cannot be shown. The maker notes a rule: machine speech in mono, human speech in bold sans.
- **Motion:** slow push-ins on archive art. A tilt-up across three crops of a Botticelli at 15:43. A shatter transition at 18:58. The CRT pair returns as a call-back at 0:00, 10:04, 11:00, 13:47 and 21:24. Colour changes carry meaning: the red family is removed from the paired-figure drawing at 8:36.
- **Sound:** not measured (the audio logs hold only a framework warning).
- **Thumbnails:** not in the inputs.
- **Hit pattern:** one hit at 52.17 times the channel median of 23,000. The sample is three videos. No dated follow-ups.

## Film 2: "Would You Board a Ship to Another Star?" (Orange Scarf, oRBu7wYuOSo)

- **Title, channel, views, length:** 782,501 views in the video record (785,000 rounded in the outliers file, 786,789 in the shorts list). Length 1,172 s (19:32). 5,236 likes, 659 comments. Uploaded 8 Nov 2026.
- **Ratio:** 4.58 times the channel median of 171,500 (four videos sampled).
- **Type:** narrated science fiction, animated (per tags). Part 1 of a series called "Leaving Earth". The narrator is an engineer who knows he will not arrive. The description says the science is sourced (Tau Ceti f, from the NASA Exoplanet Archive).
- **Pacing:** the description gives 10 timestamps. Section lengths: intro 0:56; 2:14; 2:15; 1:43; 2:16; 1:21; 2:31; 2:48; 3:04; and a final 0:24. Most sections run about two minutes.
- **Palette, quote structures, motion, thumbnails:** not measured.
- **Sound:** the creator's note says there is no sound in space and that the sounds are there for feeling. This is the creator's claim, not a measurement.
- **Hit pattern:** the 8 Nov film was followed 14 days later (22 Nov) by a video at 112,712 views, 0.65 times the median. Only this one follow-up was checked. Two files give different titles for the same ID. Part 2 of the series is not in the inputs.

## Film 3: "Something Is Strange About Where We Live in the Milky Way" (Milky Stellar, G4w-a8NgnnQ)

- **Title, channel, views, length:** 330,470 views at pull on 24 Nov (5 days old). The channel list shows 330,561. 9,404 likes, 303 comments. Length 38:01 (2,281 s). Uploaded 19 Nov 2026. About 66,094 views per day. Channel median 19,092 across 101 uploads. Ratio 17.31. 79,600 subscribers.
- **Type:** documentary explainer with three layers. Borrowed archive (stock, ESO, NASA, Wikimedia); code-drawn diagrams (the maker estimates about 35% of running time); and on-screen text. The tone is calm and hedged, with 69 different footnotes.
- **Pacing (measured):** 240 shots, 209 hard cuts, 30 soft changes. Median shot 8.0 s, mean 9.5 s, 90th percentile 15.75 s, longest 71.25 s. The opening runs 11 to 12 shots a minute and the late film falls to 0 to 1. The longest holds are a NASA zoom-out (71.2 s, starting 33:46) and a galaxy fly-in (38.5 s, starting 36:59).
- **Palette (measured, median of sampled pixels):** ground #000100 and #000405. Lower-third title #FEFFFD, subtitle #E2DBAB, rule #F0DF8C. Header grey #868B8A. Cool data series #94A4A5 and #B9D1D7; warm series #BDB59F and #D7B77A. Median frame luma 31.8 of 255, with 58% of frames below 40. The one white chart (22:19 to 22:46) and the white flash at 21:24.5 are the only bright moments.
- **Quote structures:** no spoken quote is shown on screen. The number format has eight shapes; the maker's own limit is three.
- **Motion:** photos get a slow push-in, about 1.05 to 1.15 times. Orion at 1:58 reaches about 1.4 times over 13 s. Diagram lines draw on. Counters step rather than roll: flux 0.55x to 0.08x (2:11 to 2:20); race 253 years to 17,600 years (8:02 to 8:15); decay 99% to 13% (26:23 to 26:47). Text fades in once and does not move.
- **Sound:** design data is marked pending. The remake notes report silence after heavy numbers and no speech under -40 dB for more than 1.2 s. That is the maker's claim, not checked here. Captions were blocked (HTTP 429).
- **Thumbnails:** the locator device is a white arrow and a small white circle on a dark void, with three words in one weight right of centre. No top band. Likeness to earlier thumbnails was judged by eye. The baseline for random consecutive thumbnails is 0.18 grey correlation and 40.2 median colour distance.
- **Hit pattern:** 12 of 101 uploads reached 10 times the median, this film included. Next upload after a hit: +1 median 1.82 times (50% reach 2 times or more); +2 median 0.75 times (18%); +3 median 2.68 times (55%). The base rate for 2 times or more is 35%. The next upload, "Why the Universe Is Emptier Around Us Has a Troubling Answer", reached 2.98 times at 2 days, the one 90% echo seen.

## Film 4: "The Grand Canyon Wasn't There in 1540??" (Ink Of The Past, HmuQoak_IAg)

- **Title, channel, views, length:** 51,018 views, 603 likes, 138 comments. Length 550 s (9:10). Uploaded 23 Nov 2026. Channel median 11,000 across 79 videos sampled. Ratio 4.64.
- **Type:** question-title history video. Judged from the title only; the transcript was not read.
- **Pacing, palette, quote structures, motion, sound:** not measured. Captions were blocked (HTTP 429). Frame and ASR outputs are in the work folder but were not read.
- **Thumbnails:** saved, but none was read here.
- **Hit pattern:** the channel's top outliers are "Is THIS the Reason Greenland IS Making Headlines Right Now?" (838,000 views, 76.18 times) and "What Was Here Before the Grand Canyon?" (581,000, 52.82 times). Five of eight dated uploads from September 2026 use the title pattern "What Was Here Before ...?", with 6,620 to 49,371 views (third column of the date file, read as views). This film does not use that pattern. Whether it follows the 581,000 hit is unknown, because that hit's date is not in the inputs.

## Film 5: "The Ancient Test of a True Friend" (The Ancient Logos, sJiaWNxYFUA)

- **Title, channel, views, length:** 159,863 views (159,000 in the outliers file). 1,870 likes, 87 comments. Length 681 s (11:21). Uploaded 10 Nov 2026. Channel median 13,500 across 14 videos sampled. Ratio 11.78.
- **Type:** narrated history essay on friendship. A tyrant in Syracuse tests a friendship. Cites ancient sources and two modern studies: a 2018 study on hours to become close friends, and a 2021 survey on men with no close friends.
- **Pacing:** intro "The Experiment" 0:00 to 2:07; Chapter I 2:07 to 5:34 (3:27); Chapter II 5:34 to 7:32 (1:58); Chapter III 7:32 to 10:01 (2:29); Chapter IV 10:01 to 11:21 (1:20).
- **Quote structures:** the creator says the quotes are their own simplified translations. The source list is in the description. Frame-level quote style was not measured.
- **Palette, motion, sound, thumbnails:** not in the inputs.
- **Hit pattern:** 11.78 times the median. Other channel outliers: "The Ancient Philosophy of Having No Fear" (501,000 views, 37.11 times) and "How the Romans Controlled Their Anger" (65,000, 4.81 times). No dates for these, so the follow-up is unknown.

## Numbers

| Film | Measure | Value | Status |
|---|---|---|---|
| 1 hands | Views / length | 1,257,209 / 24:29.7 | Measured |
| 1 hands | Ratio to median (3 sampled) | 52.17 (median 23,000) | Measured |
| 1 hands | Sheets / span per sheet | 29 / about 45 to 70 s | Measured (by eye) |
| 1 hands | Quote count | about 25 | Estimated |
| 2 Orange Scarf | Views / length | 782,501 / 1,172 s | Measured |
| 2 Orange Scarf | Ratio to median (4 sampled) | 4.58 (median 171,500) | Measured |
| 3 Milky Stellar | Views at pull / length | 330,470 / 2,281 s | Measured |
| 3 Milky Stellar | Ratio to median (101 uploads) | 17.31 (median 19,092) | Measured |
| 3 Milky Stellar | Shots / hard cuts / soft changes | 240 / 209 / 30 | Measured |
| 3 Milky Stellar | Median / mean / p90 shot | 8.0 s / 9.5 s / 15.75 s | Measured |
| 3 Milky Stellar | Median frame luma | 31.8 of 255 | Measured |
| 3 Milky Stellar | Diagram share of running time | about 35% | Estimated (maker) |
| 3 Milky Stellar | Hits (10 times median or more) | 12 of 101 | Measured |
| 3 Milky Stellar | After a hit, +1 / +2 / +3 median | 1.82x / 0.75x / 2.68x | Measured |
| 3 Milky Stellar | Base rate, uploads at 2 times or more | 35% | Measured |
| 3 Milky Stellar | Thumbnail baseline (grey / colour) | 0.18 / 40.2 | Measured |
| 3 Milky Stellar | Thumbnail likeness | Judged by eye | Judged |
| 4 Ink Of The Past | Views / length | 51,018 / 550 s | Measured |
| 4 Ink Of The Past | Ratio to median (79 sampled) | 4.64 (median 11,000) | Measured |
| 4 Ink Of The Past | Title pattern share (8 dated uploads) | 5 of 8 | Measured |
| 5 Ancient Logos | Views / length | 159,863 / 681 s | Measured |
| 5 Ancient Logos | Ratio to median (14 sampled) | 11.78 (median 13,500) | Measured |

## Breakthroughs

None claimed. The inputs record measurements and the maker's notes, not a tested result. The Milky Stellar hit-pattern figures are the only ones tested against a baseline (35% of uploads at 2 times or more).

## What critics found

- **The 90/70/50 echo rule does not show up as a run.** Back-to-back repeats scored 2.1, 0.4 and 0.3 times. No 90 then 70 then 50 run was seen after any of the 12 hits. Shown by the Milky Stellar hit analysis. Status: **open**.
- **The remake broke its own design limit.** The number format has eight shapes against a limit of three. Diagram cards use three or four text sizes against two. The remake notes plan to cut to three shapes and two sizes. Shown by comparing the design file with the remake notes. Status: **open**; the plan exists, the change is not made.
- **Licence risk.** One film claims a broadcast authorisation with no record. Space-simulator captures carry leaked interface text. The remake notes avoid both. Status: **open**, pending per-clip records.
- **Two shots cannot be reproduced.** The smoke-render volume and the continuous NASA zoom-out are beyond the current render path. Status: **open**.
- **Font not named.** Diagram text matches an Arial-class face by eye; no licence page names a font. Status: **unknown**.
- **Voice timing missing.** Captions were blocked for Milky Stellar and Ink Of The Past (HTTP 429). Status: **open**.

## Still open

- Sound for all five films. Film 3's audio folder is not summarised here.
- Thumbnails for films 1, 2, 4 and 5. Film 4's image strips are not read.
- Palette and motion for films 2, 4 and 5. Quote style for films 2, 4 and 5 is not measured frame by frame.
- Film 1 rests on three sampled videos, with no dates for its hit or its follow-ups.
- Film 2's Part 2 is not checked, and two titles for one video ID are unresolved.
- Upload dates for films 1 and 5 are not confirmed from the video record.
- All view counts are as pulled. Recent uploads are still rising.
