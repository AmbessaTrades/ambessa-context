<!-- copied from the Juju repo: docs/STACK-STATUS.md, last changed 14:10 EAT, 24 Nov 2026. Private lines removed. Do not edit here. -->
# Stack status: what each paid route really does and costs

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.
> 24 Nov 2026, 09:50 to 10:03 UTC. **Measured** = a call made today, in `runs/meter/ledger.jsonl`. **Listed** = a vendor page or price list. **Said** = Ambi's word. **Assumed** = neither.

**Route proof, first 20 ledger rows: $0.0926** of its own $0.60 cap. The ledger is now shared by four jobs with separate caps; the whole total is in the ledger, not here. (20 lines: OpenRouter 9 calls $0.0718, DeepSeek 7 calls $0.0207, Google 4 refusals $0).
OpenRouter's own usage moved by 0.071847612, the ledger's sum to the last digit (measured). DeepSeek's cost is tokens times listed price; its balance fell from 16.95 to 16.93 some minutes later, which agrees to the cent (measured). Re-run: `scripts/route_proof.py`.

| Service | For | Sign-in (said) | Balance, US | Ids that answered today |
|---|---|---|---|---|
| OpenRouter | GLM, Jev (Neon only as a stand-in today) | "most of these I signed up with GitHub", which ones not said | 18.53 live at 11:07 UTC (measured); 18.82 before, 18.75 after, measured (said 18.82) | `z-ai/glm-5.3`, `typesafe/jev-1.14`, `typesafe/jev-router`, `google/gemini-4-neon` |
| DeepSeek direct | daily scripts, forms, checks | his email | 16.49 live at 11:07 UTC (measured); 16.95 before, 16.93 after, measured (said 16.96) | `deepseek-flash` |
| Google AI Studio | flagship scripts | same sentence | not visible to the key (said: prepay) | `gemini-4-neon` direct since 13:08 EAT (measured; before that refused, 429) |
| WaveSpeed | thumbnails only | same sentence | 12 measured (said 10) | no paid call made |
| Inworld | voice | same sentence | 41.58 said; not visible to the key (24 Nov 13:51 EAT: no balance call for an API key in the docs) | `inworld-tts-2`, `inworld-tts-2-flash` (measured 24 Nov; see 7) |

## What needs Ambi

1. ~~Google~~ **fixed 13:08 EAT: Ambi linked billing.** Before that: the key was on the Free Tier. All 4 direct Neon calls: 429, `free_tier` metrics, limit 0 (measured). The prepaid money is not attached to the project that owns this key. In AI Studio, Projects: check the Billing Tier of that project, then "Set up billing", or make the key inside the prepaid project (listed steps). Then: `route_proof.py neon`, then `neon-cache` (about 2 cents).
2. ~~Inworld key~~ received; it lists 407 voices (measured, free call). Speech tested 24 Nov 13:51 EAT (see 7). Open: his Inworld balance, which only the signed-in Billing page shows.

## 1. DeepSeek `deepseek-flash`
- Valid JSON mode at off, low, high, max (measured, 4 of 4). One small call (1,151 in, about 40 out): $0.0004 peak.
- Cache fields are reported. First four calls, 1 s apart: 0 cached. Eight seconds later: 896 of 1,151 cached (measured).
- Peak is 01:00-04:00 and 06:00-10:00 UTC, Monday to Friday, double price (listed). The small calls fell inside it; the forms after it.
- The saved doc has no prices, levels or peak hours; those came from DeepSeek's live pages, read today. The price page is now saved as `docs/stack-txt/deepseek-pricing-live.txt` (24 Nov, 10:55 UTC).
- **A whole 20 minute script at low** (24 Nov, measured, `money script ds low 20min`): 686 in, 4,544 out (751 thinking), **$0.0028** off-peak, 33 s, 3,185 words back for 2,800 asked. One call, finished.
- **A 917 word form span at low** (measured, `money form ds low 917w`): $0.0061, 47 s, 5,888 of 6,510 input cached. **Not valid:** 0 schema errors, 5 pacing faults (a scene still for 22 to 30 s), and `heal` fixed none. n=1. The checker and test pack were changed by another job at 14:03 to 14:06 EAT: under it the 142, 426 and 917 word low forms all fail (1, 3 and 8 law faults), so no span is shown valid today and old and new results do not compare.

## 2. OpenRouter `z-ai/glm-5.3`
- 200 on 5 of 5 calls (measured). The old 403 did not come back. Effort high accepted; strict JSON schema worked.
- **Default routing is not the 0.0699 price.** It went to Together (precision listed "unknown") at 1.40 / 4.40, then InferenceNet (listed fp4, 4 bit) at 0.084 / 3.60, which also wrote the form below. The 1.40 output price is Wafer only. Output price is what matters.
- Same question, pinned: Wafer fp4 (cheapest listed) $0.000028, Z.AI fp8 $0.000106, 3.8 times more on that 38-token question (measured); by list about 20 times on input and 3.1 on output. No seller lists above fp8; several list "unknown". Pin with `provider.order` + `allow_fallbacks: false`.
- The question was too easy to show what effort high buys.

## 3. TypeSafe Jev
- **Jev 1.14 works with the OpenRouter key at 0.042 per million** (measured). It is `typesafe/jev-1.14` on `POST /api/alpha/decisions`. It was missed because the plain model list hides decision models; add `?output_modalities=decisions`. No TypeSafe key needed.
- One 512 px picture, one score + one yes/no: 1,116 tokens, **$0.000047**. I looked at the picture: a contact sheet, nine rows of scenes, ours beside real films. Right brief 2.24 of 3 and 0.85 yes; wrong brief 0.52 and 0.08 yes (two calls, so a sign, not a calibration; confidence 0.25 and 0.5). Each side must be at least 256 px (listed).
- `typesafe/jev-router` is not a scorer: it picks a chat model. It sent the picture to DeepSeek Flash and answered "3" ($0.00004). The plan should name `jev-1.14` and drop the router.

## 4. Gemini Neon (updated 13:17 EAT, after Ambi linked billing to the JUJU project)
- Direct key works, Tier 1 (measured: 200 on 7 of 7 calls after linking).
- **Implicit cache: 0 of 3 repeat calls hit** (measured, one prefix of 4,866 tokens and one of 9,851, calls 6 to 11 s apart; the field was absent). The listed minimum is 4,096. A saving from the cache is **not proven**, and changing the level could not be tested. Not tried: longer gaps, the batch route.
- The form job, direct, level low: valid, 0 errors (measured with `juju-stage check`): 5,103 in, 293 visible out, 3,234 thinking, **$0.0682**, 60 s.
- Listed price 3 / 15, cached 0.15. Thinking is billed as output.
- **A whole 20 minute script at low**, its lowest level (24 Nov, measured, `money script neon low 20min`): 709 in, 3,237 out plus 2,062 thinking, **$0.0816**, 67 s, 2,759 words back for 2,800 asked. That is 29 times DeepSeek's price for the same outline. Quality was not compared.

## 5. The real job: the form for 60 s of act 1 (same bytes, `juju-stage check`)

| Model | Valid first time | Tokens in / out (thinking) | Cost | Seconds |
|---|---|---|---|---|
| deepseek-flash, high | yes with a 40,000 ceiling; blank at 12,000 (my ceiling, still thinking) | 5,599 (5,376 cached) / 18,228 (17,937) | $0.0110 off-peak (+ $0.0080 for the blank) | 88 |
| glm-5.3, high, InferenceNet | yes | 5,067 / 11,771 (11,349) | $0.0428 | 171 |
| gemini-4-neon, low, OpenRouter Flex | yes | 5,102 / 2,794 (2,575) | $0.0286 (Standard would be 0.0572, computed) | 27 |

- All three pass, 0 errors, 0 laws. **All three produced a form the checker accepts.** One fill each, 60 s, one script: not proof for a film.
- **The checker passed a wrong picture.** GLM and DeepSeek show page 323 of the Republic under "his body was found unaffected by decay". I read the scan: that line is not on it. `document_page` with only `author` and `whole` is never checked against the words. Neon: nothing found by the checker; it shows the same page under "at the end of his Republic", right book, later passage.
- Supply: no pictures exist for this script, so the test borrowed `stage-y`'s (four afterlife paintings under a battlefield script). A hand-written form also passes, so a valid answer existed; taste was not judged. DeepSeek ran on high, not the max ADR 0006 asks for: max on this job is not measured. GLM on high as ADR 0006 says.

## 6. WaveSpeed (no paid call)
`POST https://api.wavespeed.ai/api/v3/openai/gpt-image-2.6-flare/text-to-image` with `prompt`, `aspect_ratio` "16:9", `resolution` "1k", `quality` "low" or "medium", `output_format` "jpeg"; poll `/api/v3/predictions/{id}/result`. Low $0.027, medium $0.045 (listed after 10% off; list 0.03 and 0.05). Sunburst prices are not in the saved page. 12 US is about 266 medium or 444 low.

## Money map, corrected (candidate)
- **24 Nov, 14:00 EAT: replaced by `docs/adr/0010-twenty-minute-films.md` and `runs/money/plan-20min.json`.** Those give voice, CAD totals and film counts from ledger rows. The 60 day, 3 channel plan at 20 minutes uses 82.43 US (115 CAD of 135) with a 20% reserve, if a form works on the first try (not shown). Inworld runs dry first, on day 56. The lines below are the earlier 50 minute map, kept as history.
- 50 minutes as 50 one-minute fills (straight multiplication, assumed; longer spans per call are untested): DeepSeek $0.55 off-peak, $1.10 peak. GLM $2.14 unpinned as measured, about $0.84 pinned to Wafer fp4 and $2.94 to Z.AI fp8 (same tokens, computed). Neon $1.43 Flex, $2.86 to $3.41 Standard (n=1 each). ADR 0006 guessed $2.00 for a whole Crafted film.
- **Not yet shown to fit 135 CAD:** this is US dollars a film, with no voice, no CAD total and no film count. Treat it as a warning, not a map. So the form alone on GLM would end the OpenRouter wallet in about 8 films unpinned, about 22 on Wafer; on DeepSeek off-peak 16.93 lasts about 30. **92 to 98% of output is thinking**: effort and span per call are the knobs. "DeepSeek on max, GLM on high" (ADR 0006) is the costly line for this job; low and max are not measured.
- Picture checker: 1,125 pictures a film (ENGINE-2 candidate) is $0.053 at 512 px with two questions (larger pictures not measured). Sixty films about $3.2, under the 14 CAD set aside.
- Not proven: Neon direct and its cache, GLM and DeepSeek on low, Jev against human picks, spans over 60 s, any picture, any voice. (24 Nov update: DeepSeek low is measured for cost; no low form passes the 14:06 checker. Voice is measured, see 7. Neon direct is measured. Still not proven: the cache, GLM at low, Jev against human picks, and any paid picture.)

## 7. Inworld voice (24 Nov, 13:51 EAT, measured: `money voice inworld-tts-2 60s`, `money voice inworld-tts-2-flash 60s`, `money voice batch probe tts-2`)
- Stock voice `Winston`, marked `isCustom: false` in the voice list. The same 864 characters (160 words) went to both models: TTS-2 gave **50.7 s** for $0.0216 in 14 s, and Flash gave **50.2 s** for $0.0130 in 11 s. Both returned word timestamps for all 160 words. That works out to 5.4 characters a word and **189 words a minute**, faster than the pack's 142. At `speakingRate` 0.845: 60.4 s and 60.1 s, 159 words a minute, same price (measured). Files: `runs/money/audio/`.
- The plan is probably **On-Demand** (inferred: the custom voice capacity call returns a limit of 100, the On-Demand number on the pricing page). On-Demand lists up to 70 free minutes; costs here are charged at list, so real charges may be lower. Rates listed: TTS-2 $25 and Flash $15 per million characters. Creator would be $20 and $10, but it needs a subscription. Saved: `docs/stack-txt/inworld-pricing-live.txt`.
- **The batch route is open to this key on TTS-2, at 20% off** (listed). Two one-item batches (52 and 864 characters) were done at the poll 15 s later; the second returned a word timestamps file. Listed target is 24 hours. Flash was refused with "not supported for batch synthesis". On-Demand caps one batch job at 10,000 characters (listed), so a 20 minute film needs 2 jobs. The 41.58 balance is not visible to the key; `inworld login` would show it, and that was not done.
