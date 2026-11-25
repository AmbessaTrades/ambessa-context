> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

# 0010. Twenty minute films on three channels: does the money work?

> **25 Nov 2026:** map films are about 30 minutes and cost what `docs/COSTS-MAPS.md` says (ADR 0022 item 6).

**Status:** NOT decided. Ambi's question plus the lead's recommendation. If accepted it would replace the 50 minutes in 0004 and, for forms, "DeepSeek on max" in 0006 (priced here at low). It keeps TTS-2 and pauses in the edit (0005) and the fixed 135 CAD (0008).

**Asked, 24 Nov 2026:** "if we were to move all of our channels to like 20 minutes of video, and have one that has no audio, would the payment work? [...] no more than 25, or we can even do 15 [...] three channels posting every day and one of them doesn't have audio."

**Priced:** 60 days, 2 narrated and 1 silent film a day: 120 + 60 = 180. US dollars unless marked. Every number and label: `runs/money/plan-20min.json` (rebuild: `runs/money/work/plan.py`).

## One 20 minute film, 2,840 words (the pack's 142 a minute, not the voice's own pace)

| Part | Narrated | Silent | Wallet | Label (ledger purpose) |
|---|---|---|---|---|
| Script | 0.0840 | 0.0025 | Google / DeepSeek | measured, scaled by words: `money script neon low 20min` / `money script ds low 20min`; the silent length is assumed |
| Outline | 0.0014 | 0.0014 | DeepSeek | assumed |
| Form | 0.0527 | 0.0527 | DeepSeek | measured once, scaled: `effort ds low 426w`; first-try success is NOT shown, see below |
| Picture checks | 0.0211 | 0.0211 | OpenRouter | price measured `jev-1.14 matching brief`; 450 pictures assumed |
| Voice, batch | 0.3067 | 0 | Inworld | characters measured `money voice inworld-tts-2 60s`; rate listed, 25 a million less 20% |
| Thumbnail | 0.0450 | 0.0450 | WaveSpeed | listed; one a film assumed; no paid call |
| **Film** | **0.511** | **0.123** | | 15 min: 0.395 / 0.104. 25 min: 0.627 / 0.142 |

## 60 days with a 20 percent reserve

| Minutes | US | CAD of 135 | First dry | Every wallet fits |
|---|---|---|---|---|
| 15 | 64.32 | 90.05 | WaveSpeed, day 74 | yes |
| 20 | 82.43 | 115.40 | Inworld, day 56 | no, Inworld short 2.79 |
| 20, narration capped at 2,660 words | 78.12 | 109.37 | Inworld, day 60 | just, nothing spare |
| 25 | 100.52 | 140.73 | Inworld, day 45 | no, Inworld short 13.84, Google 0.39 |

| Wallet | Now | Left after 60 days at 20 min | Pays for |
|---|---|---|---|
| OpenRouter | 18.53 measured | 13.97 | 878 films |
| DeepSeek | 16.49 measured | 4.61 | 299 films, if a form works first time |
| Google | 14.74 (said 15, less ledger) | 2.64 | 175 narrated scripts |
| WaveSpeed | 12.00 measured | 2.28 | 266 thumbnails |
| Inworld | 41.37 (said 41.58, less ledger) | minus 2.79 | 134 narrated films, no reserve |

"Pays for" leaves out the reserve. Spent on tests so far, all jobs: 1.25 (DeepSeek 0.48, OpenRouter 0.29, Google 0.26, Inworld 0.21); this job 0.178. The wallets hold 103 US, about 144 CAD at 1.40 (assumed, from his CA$21 for about 15 US); 135 CAD is 96 US. Money cannot move between wallets.

## What is weak

- **The form.** 0 of 3 DeepSeek low forms (142, 426, 917 words) pass today's checker, and `heal` fixed none. The checker and test pack changed at 14:03 to 14:06 EAT, after the forms were written against an older schema. At 13:52 the 917 word form already failed 5 pacing laws; the lead recorded 142 and 426 as valid before the change. DeepSeek can pay about **1.4 tries a form**; at two it runs dry. At 0006's high (one 60 s span, 0.0110) forms alone are about 40 against 16.49; max is not measured.
- **The pace.** Winston reads 189 words a minute by default, 159 at `speakingRate` 0.845 (both measured); 2,840 words is 15.0 or 17.9 minutes of speech, the rest is pauses or pictures. 142 needs about 0.75, below the 0.8 the docs advise; untested.
- **Batch** works with word timestamps (one 864 character item, 15 s); target 24 hours (listed), so voice a day ahead. Realtime goes dry on day 45.

## Recommendation (the lead's)

1. Take 20 minutes for all three; the total fits 135 CAD, and voice alone decides the length.
2. Voice on TTS-2 batch, a day ahead, narration capped at 2,660 words; 15 minutes is the safe fallback.
3. Scripts on Neon low, forms on DeepSeek off-peak, but first prove a form passes within 1.4 tries.

**Would change it:** Inworld's real balance; 2 thumbnails a film (16.20 against 12); DeepSeek at peak (double); long script prompts on Neon (measured on 709 tokens; about 6,000 more a script uses Google's spare); whether YouTube pays a film with no narration (not tested).
