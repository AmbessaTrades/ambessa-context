# Master brief, sections 11 to 22, summarised

This is Ambi's pasted spec of 24 Nov 2026. Later decisions (ADRs 0001 to 0009) outrank it. Prices, rates and scores below are the spec's own targets and assumptions, not measured results.

## §11 — Capability classes and the production router

The spec defines nine deterministic visual rigs, C1 to C9: cartographic theatre, tier-ladder HUD, scale flight, crowd swarm, engineering cutaway, group chat, painterly essay, four-colour atlas, and node or lineage chart. The aim is that 80 to 95 percent of frames render locally in Rust or come from free archival sources. Paid image calls, at about $0.019 to $0.027 each, are kept for hero moments. Part two is the production router, which must run with no Anthropic API dependency at runtime. Its tiers are: DeepSeek V4.1 Flash plus the TypeSafe Jev 1.14 scorer for extraction and visual checks; GLM-5.3 and GLM-5.3 Flash through OpenRouter for daily and longform prose; Gemini 4 Neon as the flagship writer; and Inworld TTS-2 for voice. Gemini gets implicit caching only when a byte-identical prefix of at least 4,096 tokens sits at the top of the request, so the static material goes first and the per-act instruction last. Thinking budgets are 6,144 tokens for the outline and 2,048 per act. Local models and local TTS are banned.

## §12 — Scanner, absorber and outlier economics

The scanner is ytlocal.py, a local tool with nine commands and no API key. It reads channels, outliers, transcripts, comments and related videos. A candidate niche must pass five axes before it earns a slot: a yield floor of 1,000 views per day per minute of runtime; a repetition proof of two to five independent channels with at least three outlier hits each; a compute ceiling of $0.45 USD marginal API cost per film; a legibility test at 160 pixels; and a durability test of at least 30 distinct topics with buyer appetite in comments. Seven instant disqualifiers include needing on-camera charisma, needing copyrighted studio clips, and one viral fluke carrying 90 percent of views. When a donor channel is absorbed, nine format measurements are recorded, plus a list of donor flaws to drop on purpose. A new pack unlocks only after its rules predict held-out videos 6 to 8 within 15 percent on runtime and 20 percent on beat count. The spec's 19 Nov checks range from 422 (fail) to 4,149 (pass) on the yield score.

## §13 — The dynamism gate (V0)

The spec's argument: viewers subscribe for a fixed trust spine (voice, world authority, clarity) and click for novelty. Novelty comes from five closed decks dealt per upload: S, six 160-by-90 silhouettes; O, six cold-open moves; R, four pacing ramps; T, title equations; and P, four visual plate mixes. Before any spend at the V0 stage, a solver checks six rules, H1 to H6. No silhouette or opening may repeat back to back. No silhouette or opening may appear more than twice in any seven-upload window. Every card must be dealt at least once per ten uploads. No exact five-part tuple may repeat within 25 uploads. No seven-word phrase may recur across the last 30 scripts. Quotes, sources and props rest on a 15-upload shelf. The problem being solved is feed blindness: the spec says LOT stopped registering after 37 uploads that looked alike. The check runs before the Stage 3 spend, so a repeat is caught before money is committed. The section reports the rules only; no result is given.

## §14 — The Offering: companion products

The Offering turns audience requests into a sold companion artifact. The spec's claim is that a deterministic dialect, plus framing built into the story, outsells a generic prompt. The lifecycle has four states. DORMANT_OBSERVING logs comment requests quietly. DEMAND_DETECTED starts once a Vessel passes 10,000 cumulative views or eight artifact-intent comments. FORGED_READY compiles a landing page, checkout and delivery email in under 60 seconds, then waits for operator approval. LIVE_ARMED places one 12 to 17 second diegetic bridge at the 50 to 58 percent mark and pins the link. Six dialects, O1 to O6, each name a build tool and a CAD price range: a typeset illustrated codex, a 300 DPI wall chart exported from the video's own canvas, an interactive simulation sandbox, a scenario bible, a declassified case vault, and a numbered relic waitlist. The spec examples are a coin offered inside a story and a wall-poster offer made inside a chart video. The bridge rule is strict: same voice, no sales tone shift, at most 38 plain words.

## §15 — Eleven-stage pipeline and the Rust workspace

Each run writes immutable, content-hashed JSON per stage, so an interrupted run resumes where it stopped. The target is under 90 seconds of wall-clock pre-render time before GPU encode. Stage 0 locks the V0 deck. Stage 1 deals titles and thumbnail variants. Stage 2 is the one human tap (the pact), which shows audio mode and exact cost before any spend. Stage 3 builds the master outline. Stage 4 drafts four to eight acts in parallel, then runs a linter with a short healing pass on each sentence. Stages 5 (audio) and 6 (visual retrieval and scoring) run side by side. Stage 7 renders act chunks under 580 MB with -14 LUFS audio and three anti-slideshow gates. Stage 8 is a span-checked review. Stage 9 exports a publish kit. Stage 10 measures day 1, 7 and 30, and triggers the echo-decay chain at 2.0 times median or more. The workspace is ten Rust crates with trait boundaries, plus a Tauri shell for Mac, web and Android. Legacy code is reused only as four named tools and formulas.

## §16 — Software and API budget

Only API lines are kept here, and all of them are superseded by ADR 0008 (135 CAD, the split in `money-and-stack.md`). In the brief: Google AI Studio gets 22 CAD for Gemini 4 Neon, which the spec says covers more than 120 flagship scripts at about $0.07 to $0.11 USD each. OpenRouter gets 12 CAD for GLM, and DeepSeek direct gets 11 CAD. TypeSafe gets 10 CAD for Jev scoring. Inworld gets 45 CAD for TTS-2 and Flash batch voice. WaveSpeedAI gets 44 CAD for image plates and Mischief 1 motion. A dev spend fuse caps paid test calls at $0.75 USD. Test runs default to a zero-cost dry run, and a live call needs an explicit switch. Per-film voice cost is about $0.24 USD for a 14-minute flagship narration, $0.14 for a 14-minute fleet episode, and $0.00 to $0.03 for silent or sparse-radio films.

## §17 — Computer-use self-setup and the smoke gate

The spec tells the lead builder to act, not ask. Before creating accounts, it must reuse valid keys already on the machine for OpenRouter, DeepSeek, GitHub and Pexels. For missing services (Google AI Studio, TypeSafe, WaveSpeedAI, Inworld, Turso, Cloudflare, Lemon Squeezy and Resend), it drives browser or CLI setup through the operator's signed-in sessions. It then asks the operator once, in a batched two-minute window, for any two-factor or payment click. All keys go into one local secrets file with restricted permissions, never committed. Before Milestone A (Wed 25 Nov 2026, 20:00 EAT), the stack must pass a smoke test run with Anthropic variables stripped from the environment. The test must draft a script on Gemini 4 Neon or GLM-5.3, show cached tokens above 4,000, build a 60-second 1080p clip at -14 LUFS plus a sample Offering PDF under 580 MB, pass the three anti-slideshow gates, and cost under $0.18 USD in total.

## §18 — Swarm architecture and SkillForge

The operating model is one overseer and parallel sub-agents. An Opus-class lead holds the master contracts and reviews diffs. A stronger model is used only for hard borrow-checker and shader work. Work runs in four waves of eight to twelve concurrent workers. Wave 1 harvests reference material into JSON. Wave 2 writes the 32 permanent skills. Wave 3 builds the dual-viewport UI loop and the Rust crates in parallel. Wave 4 compiles the Mac and Android builds and pre-stages the first slates. Each wave writes receipts to a shared memory store before and after. SkillForge is the self-extending part. When the system absorbs a new donor channel, or sees a winner at 2.5 times or more, it writes new skill packs to disk with no human step. A new skill goes live only after a holdout check on three unseen donor videos and the linter. The 32 skills are listed in Appendix B.

## §19 — The 24 mental models

Every agent and skill must reason from 24 named mental models, listed one line each in Appendix A. They cover speed over polish, cutting extra parts, tracing consequences three steps forward, causal story structure, rising-trend topic choice, copying proven shapes across settings, and craft limits. Several work as cost rules: silent or sparse audio is a lever on margin, and a rule forbids fake faces of real people. Others set the finish line. A build counts as done only when a stranger watches past minute ten and buys. The models are meant as checks, so each one maps to a gate in sections 12 to 15.

## §20 — Vocabulary and the decision register

The spec fixes names for the UI, the crates and the docs. The vocabulary is in Appendix C. The register has 24 decisions, D1 to D24. The intro above says later ADRs outrank them. D1 to D5 set scope: a private tool for two operators, a version-free workspace, the Vessel as the atomic unit, a dual viewport with an offline PIN and sync, and a zero-timeline editor. D6 to D12 set models and cost: no local LLMs or local TTS, the $0.75 dev fuse with a zero-cost calibrated clock, Gemini 4 Neon as paid pay-as-you-go, GLM and DeepSeek as the other brains, the three Inworld audio modes, TypeSafe as the visual gatekeeper, and the Earshot sound engine (ADR 0001). D13 to D20 set craft: fonts and the animated mark, sigil dialects, the linter and resting shelf, rising-river and echo-decay, the world-log voice, the C1 to C9 rigs, the offering, and the 32 skills. D21 to D24 set operations: autonomous setup, the zero-key smoke gate, the 25 Nov 2026 launch, and a cap of 10 questions per batch and 30 in total.

## §21 — Stack reference harvester

A shell script fetches 19 vendor reference documents into a local docs folder. The list covers Google AI Studio, Gemini pricing and caching, OpenRouter, Z.ai, DeepSeek, TypeSafe, Inworld, WaveSpeedAI for two models, Mischief 1, Tauri v2, Turso, Typst, the impeccable design skill, the Earshot skill and a TubeLab niche skill. The purpose is that sub-agents read current specs rather than guess endpoints. It runs in wave 1. Each download uses curl with fail-on-error. A failed download does not stop the script; it prints a warning to check the page by browser. The script does not retry or verify content, so a failed download leaves a gap the agent has to fill by hand. The spec describes the script's behaviour and does not reproduce its text here.

## §22 — Day-1 builder launch prompt

The last section is a prompt to paste into the Day-1 builder. It casts the lead as chief architect over a swarm of eight to twelve parallel workers. It sets a fixed boot sequence: query the shared memory store, read the full brief, run the harvester, install the design and skill tooling, then fan out harvesters over local reference sets. Those sets are video captures, UI screens, the gallery plates and a ported engine. Iron laws: no local LLMs or local TTS, with Earshot's listening models as the one exception; protect paid credits with dry-run mode and the fuse; design every screen at 1440 by 900 and 390 by 844 in two passes, the second adding house fonts, skins and sound; build all 32 skills on Day 1; and set up accounts with minimal interruption. The prompt also requires a readiness report, at most 10 grill questions per batch, and a credentials and runbook registry with every key checked by a live ping.

## Appendix A: JM_01 to JM_24 mental models

- JM_01 Asase Velocity: shipped iteration beats perfectionism; slow pipelines die.
- JM_02 Machete Razor: when unsure, cut the extra moving part at once.
- JM_03 Ripple Sight: trace each script beat and each budget dollar three steps forward.
- JM_04 Crossroads Chain: every beat links by "therefore" or "but", never "and then".
- JM_05 Rising River: pivot from small to big, widening the audience, never narrowing.
- JM_06 Echo Decay 90/70/50: milk a 2.0x outlier through three decaying sequels, then rest.
- JM_07 Graft to Bloom: copy proven outlier bones early; mine own comments after upload 12.
- JM_08 Crown Weight 70/20/10: title and idea 70 percent, silhouette 20, polish 10.
- JM_09 Root Bending: bend a proven format across places, eras and pantheons.
- JM_10 Mirror Bend: turn a winning thumbnail geometry into three variants.
- JM_11 Shadow Sieve: words that appear in a channel's flops are poison, not alpha.
- JM_12 Pre-Installed Map Violation: break a concept most people already picture, with one impossibility.
- JM_13 Spirit Tongue: ban generic AI phrasing with a fast linter and switch voice per channel.
- JM_14 Resting Shelf: any repeated quote, hour or prop becomes wallpaper; rest it 15 uploads.
- JM_15 Ancestral Breath: deep thinking on the outline, lean rhythm on prose, pause after numbers.
- JM_16 Visual-Load Inversion: speak less when the visuals are busy, more when they hold still.
- JM_17 Ghost Onion Separability: version each design axis separately so a fix is surgical.
- JM_18 Calm Room Theatre: at most 40 resting words on Home, three doors, one big forward button.
- JM_19 Frame-Truth Honesty: no fake faces of real people; deliver the thumbnail's promise by 0:40.
- JM_20 Silent and Diegetic Leverage: voice is a choice, not a tax; silent films carry the margin.
- JM_21 Value Alchemy: an artifact shown inside the story converts better than a shouted ad read.
- JM_22 Cohort Desync: keeps two channels in one niche distinct in look and opening.
- JM_23 Destination-Only Proof: compiling is not progress; a stranger watching past minute 10 and buying is.
- JM_24 Mind-Touch Test: every film is judged by where the viewer's mind travels and what lingers.

## Appendix B: the 32 skills

Group A, builder and UI craft:
1. impeccable-juju-ui: UI craft rules and the house font lock.
2. doop-dual-viewport-loop: twin 1440 by 900 and 390 by 844 mockups, two passes.
3. jujulogov01-svg-animator: 60 fps motion for the witch-cat mark; no human characters.
4. earshot-sound-engine: make, build, fit, listen to and level every sound effect.
5. zero-spaghetti-rust-contract: trait boundaries, integer shot joins, memory caps, spend fuse.
6. gemini-neon-implicit-cache: static prefix rule and the 6,144 and 2,048 thinking budgets.
7. autonomous-portal-provisioner: browser and CLI playbooks for service setup.
8. memoir-swarm-handoff: structured receipts to the shared memory store per wave.

Group B, ideation and anti-fatigue:
9. rising-river-tam-expander: small-to-big audience check for titles and pivots.
10. shadow-sieve-flop-differ: winners minus flop tokens, keeping only strong lifts.
11. echo-decay-90-70-50: the three-step sequel chain and 10-upload cooldown.
12. graft-to-bloom-comment-miner: outlier grafting early, comment mining later.
13. diviner-12-equation-mint: title equation compiler with a bad-idea killer.
14. v0-cohort-desync-solver: keeps two channels in one niche distinct in look and opening.

Group C, script and voice:
15. clean-calabash-42tic-healer: 42-tic linter and single-sentence healer.
16. crossroads-chain-outliner: four-pass cause-and-effect outline with scenario forks.
17. voice-vm01-elder-brother: direct, first-person counsel voice.
18. voice-vm02-jacopist-dispatch: dated world-log voice on three scales.
19. voice-vm03-polyphonic-stage: two-voice faction debates and group-chat drama.
20. voice-vm04-05-guide-and-atlas: deadpan walkthrough and visual-load pacing.
21. resting-shelf-15video-guard: 15-upload cooldown and audio clock modes.

Group D, packaging, visuals and offering:
22. mirror-bend-thumbsy-transmuter: spatial extraction into three thumbnail variants.
23. sigil-d1-d2-photoreal-and-desk: archival photo and broadcast-desk dialects.
24. sigil-d3-d4-cutaway-and-simframe: cutaway prompts and live sim frame capture.
25. sigil-d5-d6-tableau-and-4color: stage blocking and four-colour map dialect.
26. feedsight-otsu-g1-g6-critic: squint gate and multi-device preview.
27. reliquary-jev-archival-hunter: museum and NASA public-domain search with scoring.
28. c7-painterly-and-quote-rig: progressive paint and word-synced quote canvas.
29. c8-c9-atlas-and-nodetree-rig: map theatre and node chart, video and print.
30. offering-o1-o6-typst-forge: codex, sim export, relic waitlist and storefront builder.
31. diegetic-bridge-weaver: 12 to 17 second in-story offer at the retention peak.
32. skillforge-meta-autolearner: writes new skills to disk from breakouts and new donors.

## Appendix C: Juju vocabulary

- Juju: the private channel-manufacturing and companion-product software.
- jujulogov01: the official witch-cat icon and avatar; no human or character generation.
- Vessel: a portable channel pack holding onions, spine, voice, audio mode, dialect and offer.
- The Altar (or The Shelf): the multi-Vessel portfolio cabinet, per operator PIN.
- The Canopy: a per-Vessel skill and telemetry tree.
- Crossroads: the outlier scanner, flop differ, comment miner and card dealer.
- Mirror Bend: one-click transmuter of a winning thumbnail into diversified variants.
- Feed Sight: live preview of the thumbnail on desktop, mobile, rail and TV.
- Diviner: the ideation and script engine, including Crossroads Chain.
- Spirit Tongue and Clean Calabash: channel voice archetypes and the fast linter.
- The Resting Shelf: the automatic 15-upload anti-repetition memory.
- Sigil: the thumbnail and plate dialect compiler with its gate chain.
- Reliquary: the free museum and space-agency archive router, scored by Jev.
- The Pact and INCANT: the pre-flight receipt that locks audio mode, offer and cost.
- CONJURING and Spell Strip: the build stage and the scene-card review.
- The Offering and Publish Kit: the companion-product synthesizer and the one-tap publishing drawer.
- Voodoo: reserved for a future architecture; not assigned to any current crate.
