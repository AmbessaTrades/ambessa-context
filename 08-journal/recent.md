# Recent journal, last 7 days

Rolling window rebuilt on every sync. Newest day last. This is what was actually done and decided, not a summary of intentions.

---

## 2026-11-15

> Message-level context for this day. Auto-logged.

---

## 2026-11-15 02:19 EAT — MUNGURA — Daily journal generated for 2026-11-14; status=success; db_length=13869; source_hash=8f1024d7d047.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-14; status=success; db_length=13869; source_hash=8f1024d7d047.

---

### [02:19] Exchange: Daily journal worker run for 2026-11-14

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `scheduler` mode.

**Actions:**
- Target date: `2026-11-14`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-14.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-14.md`.
- DB row length: `13869`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-14.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-14.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-14.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db.
**Journal Dates Repaired:** 2026-11-14.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `scheduler`.
**Verification Results:** files written, SUMMARY mirror written, DB length=13869, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-15 02:26 EAT — MUNGURA — Day opened: Memoir pass, disk at 98%, LOT silent since 2 Nov

- **Changed:** today's record opened and checked end to end. New `loop` state written (the page still described 31 Oct–2 Nov). Backup and disk nuance appended to `backup`. LOT dormancy appended to `lot`. The one `find` miss of this pass (`lot revenue snapshot`) added to `vault/project-maps.json`. Saved to GitHub as `21511e599e` via `tubeloop-commit`.
- **Why-verdict:** every beat is a real read, not a summary. `map-check` = 292 paths, 0 failed before the add and 298 after it. `sync-topics --since 2026-11-15` = nothing pending, `--apply` mirrored 0. `df /System/Volumes/Data` = 875 Gi of 926 Gi used (98%), 27 Gi free. `auh-git status tubeloop` = last save 96c848994f on GitHub, 8 files unsaved. `public/latest.json` (collected 2026-11-14T23:17Z) = latest LOT upload 2026-11-02T23:15Z "He Used Black MAGIC for Revenge, Then Became a Saint" at about 2,100 views, uploads7d 0, uploads28d 12, sourceCount 100.
- **Status — open:** four things, in order of risk.
  1. Disk. `auh-git` hit `No space left on device` twice on 14 Nov (13:04 on a snapshot dir, 21:19 on `state.json.tmp`). Nothing has trimmed since; a big commit can fail the same way. Free space came back on its own (27 Gi now), which means something purged — not that we cleaned.
  2. CloneEngine. Backup holds the last saved copy because the folder "lost 174 of 175 files"; on disk today it holds 1 file (`logs/`). Checked against `project-maps.json`: this is the 10 Nov retirement of the CloneEngine service, not a loss — the map says the folder now holds only watch state and clone work runs in Loop's profile runs. So the safety hold is correct and no restore is wanted; the noise is Mungura's warning firing on an intended shrink every autosave.
  3. LOT has not uploaded since 2 Nov — 12 days, 0 in the last 7. `loop-onefile` video 1 still waits on Ambi: the 6-GIF test, the voice click, the Genspark sends.
  4. The cron ticker was not running at 02:00; both 02:00 jobs (LOT Revenue public snapshot, nightly journal) were dispatched at 02:17:47, lateness 1066 s. Both completed ok. Cause not investigated in this pass.
- **Related:** topics `loop`, `backup`, `lot`, `memory`.

## 2026-11-15 06:10 EAT — MUNGURA — VMake daily study: LOT thumbnails vs performance
<!-- type: event -->
**From:** MUNGURA

- What happened: LOT 277,000 subs · last 21d 5 uploads · median 3,500 views · views/sub 0.0126
- Style that wins now: S1 mean 1.06x best 1.29x — dark, high-contrast, saturated, warm, no face, split left/right, clean/simple
- Own outliers: 14.29x “Your SEM3N Is SPIRIT You Can Spend”; 11.71x “Your SEM3N Is What Your AURA Is Made Of”; 4.57x “When You DON'T Ejaculate, Your Nerves Go QUI”
- Competitor Beyond The Alchemy (84,000 subs, median 26,000): 26.15x “Why Women Sense Your Energy Instantly (A”; 4.08x “Escaping the Edging Trap: The Dopamine P”
- Competitor Masculine Theory (122,000 subs, median 15,000): 21.6x “Semen retention is nervous system evolut”; 4.73x “It wasn't about semen retention. It was ”
- Competitor The Aligned Men (16,200 subs, median 4,350): 46.9x “I Did PURE Semen Retention For 1 Year, H”; 28.28x “SEMEN RETENTION BENEFITS  | 13+ MIND BLO”
- Competitor Captain Sinbad (554,000 subs, median 11,500): 4.61x “Act like a "hot girl" for success in lif”; 2.78x “You Can Have Everything You Want in 90 D”
- Competitor Semen Retention Club (162,000 subs, median 15,000): 50.0x “Captain Picard - Semen Retention”; 9.6x “She Can't Seduce A Man IMMUNE TO TEMPTAT”
- Competitor Sexual Kung Fu (196,000 subs, median 9,600): 25.1x “Angion Method For Penis Growth and Harde”; 24.48x “Orgasm Without Ejaculating By Retraining”
- Competitor Astral Doorway (308,000 subs, median 3,850): 22.6x “How to Observe Yourself | Key I — 01 • T”; 20.26x “The Spiritual Future of Humanity & End T”
- Competitor Regal Change (26,700 subs, median 3,100): 2.77x “Why You Give Hot Chicks PTSD On Semen Re”; 2.48x “I Couldn't Handle All The Female Attract”
- Competitor Taylor Johnson - Integrative Sexual Health for Men (114,000 subs, median 5,150): 28.93x “Sex Transmutation Explained ✨🔥 (How-To G”; 21.17x “Multiple Ejaculations for Men (Technique”
- Style to borrow: from Semen Retention Club best 50.0x — dark, high-contrast, muted, neutral, figure present, clean/simple
- Errors: annel/UCboJ1avpnorCXLDU5UauVzg: yt-dlp failed for https://www.youtube.com/channel/UCboJ1avpnorCXLDU5UauVzg/video
- Files changed: /Users/Mungura/AUH/VMake/out/study/study_c44deb7c.json, out/study/study_latest.json
- Verification: 40 videos with real view counts; 40 thumbnails on disk; 2 style clusters
- Catalog re-TN queue (views × ad slots × velocity; basis previous snapshot): #1 11.5% “MONEY is Actually a FLOWING SPIRITUAL ” TN DRAFT STOP CHASING; #2 6.4% “THE 7 STAGES OF SEMEN RETENTION” TN DRAFT KEEP IT; #3 5.9% “You’re “A GOD” Having a HUMAN Experien” TN DRAFT IT'S YOU
- Fastest movers (v/day): 1000 “MONEY is Actually a FLOWING SPIRIT”; 1000 “You’re “A GOD” Having a HUMAN Expe”; 1000 “How GOD Worships itself THROUGH YO”
- META (last 90d, 38 outliers): thumbs are cleaner / simpler · split left/right · big text at bottom ; titles start with WHY · ask a question ; outliers run 0–32 min
- META shift vs last quarter: shorter titles (~8 words vs 9) -1.2→-0.8; warn (don't / never / banned) +0.07→-0.11; speak to YOU +0.13→-0.05
- LOT vs meta: winners are more muted · one field · flatter than LOT's last 12
- Status: complete


## 2026-11-15 06:23 EAT — TEHUTI — TubeLoop backup left out 7 file(s) that contain keys
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup left out 7 file(s) that contain keys
- Left out (secret found, value not shown): home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/research/study-1108/vidrush/pages/builtin.html [google api key]; home/AUH/Loop/jobs/verse/_config/active-hotkeys.json [a live key value]; home/AUH/Loop/src/components/AudioDashboard.tsx [a live key value]
- Left out (over size cap): home/AUH/Loop/loop/revival/bygone/bygone-highest-state.webm (71 MB); home/AUH/Blacksite/data/packages/ep-mvfpm7ln-770d0be167.zip (104 MB); home/AUH/Blacksite/data/wedjat-adsb/2026-10-21.json (134 MB)
- Fix: move the key into the folder's .env (the keys backup picks it up) or add the path to secret_allow in ~/.auh-git/projects/tubeloop/project.json if it is not a real key.
- Status: blocked — needs an agent to look

---

## 2026-11-15 06:23 EAT — TEHUTI — TubeLoop backup kept the last saved copy of a folder that shrank or vanished
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup kept the last saved copy of a folder that shrank or vanished
- Kept last saved version (safety): home/AUH/CloneEngine — lost 174 of 175 files
- Status: blocked — needs an agent to look

---

## 2026-11-15 18:56 EAT — TEHUTI — TubeLoop backup left out 7 file(s) that contain keys
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup left out 7 file(s) that contain keys
- Left out (secret found, value not shown): home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/research/study-1108/vidrush/pages/builtin.html [google api key]; home/AUH/Loop/jobs/verse/_config/active-hotkeys.json [a live key value]; home/AUH/Loop/src/components/AudioDashboard.tsx [a live key value]
- Left out (over size cap): home/AUH/Loop/loop/revival/bygone/bygone-highest-state.webm (71 MB); home/AUH/Blacksite/data/packages/ep-mvfpm7ln-770d0be167.zip (104 MB); home/AUH/Blacksite/data/wedjat-adsb/2026-10-21.json (134 MB)
- Fix: move the key into the folder's .env (the keys backup picks it up) or add the path to secret_allow in ~/.auh-git/projects/tubeloop/project.json if it is not a real key.
- Status: blocked — needs an agent to look

---

## 2026-11-15 18:56 EAT — TEHUTI — TubeLoop backup kept the last saved copy of a folder that shrank or vanished
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup kept the last saved copy of a folder that shrank or vanished
- Kept last saved version (safety): home/AUH/CloneEngine — lost 174 of 175 files
- Status: blocked — needs an agent to look

---

## 2026-11-15 23:09 EAT — MUNGURA — Profile picture de-AI prompt pack (V4 base)

**Changed** — `~/AUH/STUDY/profile-pic-deai-2026-11-15/`: `V4-BASE.jpg` (1984², the
version Ambi picked), `V3-OLD.png`, `REF-finn.png`, `REF-blue-drape.png`,
`PROMPT.md` (the edit prompt + the law), `README.md` (remaining tells + handover).

**Why-verdict** — Two corrections from Ambi, both now law in `PROMPT.md`: (1) a pro
headshot has NO cast shadow on the wall — the volume comes from a soft shadow under
the jaw, a backdrop that darkens to the corners, and a rim light; (2) on an EDIT you
must never describe what is already in the image — describing the shirt/beard/hair is
read as an instruction to redraw them. Only light, surface and lens may be described.
The earlier "add grain" idea was wrong and was discarded: it is the flat light and the
plastic skin that read as AI, not grain.

**Status-open** — No render yet: this box has no image route wired (no OPENAI key;
Paper MCP key present, Genspark route documented in the home-image-prompting skill).
V4 still carries four tells: no shadow, flat backdrop, uniform sharpness, mirrored
front locks.

**Related** — Large brief lands 21–23 Nov (Ambi), to be run on Hermes or Claude Code
on T3; whoever takes it reads `PROMPT.md` first. Register bar: Alex Finn shot +
blue-drape press photo.

## 2026-11-16

> Message-level context for this day. Auto-logged.

---

## 2026-11-16 00:08 EAT — MUNGURA — Daily journal generated for 2026-11-15; status=success; db_length=14799; source_hash=229981586cda.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-15; status=success; db_length=14799; source_hash=229981586cda.

---

### [00:08] Exchange: Daily journal worker run for 2026-11-15

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `scheduler` mode.

**Actions:**
- Target date: `2026-11-15`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-15.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-15.md`.
- DB row length: `14799`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-15.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-15.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-15.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db.
**Journal Dates Repaired:** 2026-11-15.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `scheduler`.
**Verification Results:** files written, SUMMARY mirror written, DB length=14799, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-16 00:21 EAT — MUNGURA — Daily journal generated for 2026-11-15; status=success; db_length=14799; source_hash=dca0339b3248.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-15; status=success; db_length=14799; source_hash=dca0339b3248.

---

### [00:21] Exchange: Daily journal worker run for 2026-11-15

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `scheduler` mode.

**Actions:**
- Target date: `2026-11-15`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-15.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-15.md`.
- DB row length: `14799`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-15.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-15.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-15.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-15.md.pre-sonnet5-repair-20261116_002056.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-15.md.pre-sonnet5-repair-20261116_002056.bak.
**Journal Dates Repaired:** 2026-11-15.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `scheduler`.
**Verification Results:** files written, SUMMARY mirror written, DB length=14799, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-16 06:51 EAT — MUNGURA — VMake daily study: LOT thumbnails vs performance
<!-- type: event -->
**From:** MUNGURA

- What happened: study FAILED — yt-dlp failed for https://www.youtube.com/channel/UCMApI8KY-eOXqi4_mx6uePw/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UCSpV4LdFbvrBi88HYNmM70g/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UCkEg2hYI7rm5zqRyoGF22iA/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UC5lazMp8-tBYOXZfAazDe8w/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UCboJ1avpnorCXLDU5UauVzg/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UC8XKyvQ5Ne_bvYbgv8LaIeg/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UCxTYD_ycrBfhCK_cH-QrPBA/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UC2u82QDTLE_sm42t2uGItQg/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UCy86ub1XvSLlgrTe8wQw_lw/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UCQ-egwf_sKkZo5cTesgjc_Q/videos: ost='www.youtube.com', port=443): Fai; yt-dlp failed for https://www.youtube.com/channel/UC1VcMOExq4okNAco-yiCBiw/videos: ost='www.youtube.com', port=443): Fai
- Catalog re-TN: FAILED st='www.youtube.com', port=443): Failed to resolve 'www.youtube.com' ([Errno 8] nodename nor servname provided, or not k
- META: FAILED yt-dlp failed for https://www.youtube.com/channel/UCMApI8KY-eOXqi4_mx6uePw/videos: ost='www.youtube.com', port=443): Fai
- Status: blocked


## 2026-11-16 10:49 EAT — TEHUTI — TubeLoop backup run failed
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup run failed
- Error: could not read /Users/Mungura/AUH/Blacksite: fatal: unable to stat 'research/signal/state/.hdr14795': No such file or directory
- Status: blocked — needs an agent to look

---

## 2026-11-16 15:33 EAT — TEHUTI — TubeLoop backup left out 7 file(s) that contain keys
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup left out 7 file(s) that contain keys
- Left out (secret found, value not shown): home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/research/study-1108/vidrush/pages/builtin.html [google api key]; home/AUH/Loop/jobs/verse/_config/active-hotkeys.json [a live key value]; home/AUH/Loop/src/components/AudioDashboard.tsx [a live key value]
- Left out (over size cap): home/AUH/Loop/loop/revival/bygone/bygone-highest-state.webm (71 MB); home/AUH/Blacksite/data/packages/ep-mvfpm7ln-770d0be167.zip (104 MB); home/AUH/Blacksite/data/wedjat-adsb/2026-10-21.json (134 MB)
- Fix: move the key into the folder's .env (the keys backup picks it up) or add the path to secret_allow in ~/.auh-git/projects/tubeloop/project.json if it is not a real key.
- Status: blocked — needs an agent to look

---

## 2026-11-16 15:33 EAT — TEHUTI — TubeLoop backup kept the last saved copy of a folder that shrank or vanished
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup kept the last saved copy of a folder that shrank or vanished
- Kept last saved version (safety): home/AUH/CloneEngine — lost 174 of 175 files
- Status: blocked — needs an agent to look

---

## 2026-11-16 15:34 EAT — TEHUTI — TubeLoop backup recovered: backup run working again
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup recovered: backup run working again
- A complete backup run succeeded; push state is tracked separately.
- Status: complete — the recorded backup fault is resolved

---

## 2026-11-16 18:55 EAT — MUNGURA — Africa-CARICOM pain base built and gated

- What changed: new lane folder ~/AUH/AMBESSA/intel (nothing existed before). Built pains.db + check.py gate + build_page.py + index.html. Collected 69 pain points across four buyer groups (CARICOM gov, African gov, African firms $10M-$5B, diaspora firms $10M-$1B); 56 machine-verified against their live source, 13 unconfirmed because the sites block re-reading, 8 explicit deal-blockers. Captured 141 accounts Ambi follows and 417 X posts with URLs.
- Why / verdict: the deal does not die of mistrust, it dies of payment rails, trade finance gap ($74bn Africa, 23% bank intermediation vs 80% global), logistics (no direct Africa-CARICOM link, 12-21% of import value in freight, 3-week port dwell) and state behaviour (Kenya Sh511.75bn pending bills, Namibia cannot enforce foreign arbitral awards). Institutions never post pain on X - documents only. Therefore the offer reframes from 'verified deal room' to a deal desk answering four questions per live deal.
- Status/open: unconfirmed 13 need a non-blocked route; first real deal pair unnamed; memoir topic not yet written; page counts per group still show collected not verified.
- Related: ~/AUH/AMBESSA/intel/BRIEF.md, index.html, pains.db, check.py, x/following.json

## 2026-11-16 19:40 EAT — MUNGURA — Prep intel: East Africa, China, India, settlement, contracts

- What changed: ~/AUH/AMBESSA/intel now holds 140 findings, 130 machine-verified, across 10 groups (4 buyer, 6 competitive). New files: APPENDIX-16NOV.md (Notion-pasteable), SEARCH-PLAYBOOK.md (tested queries). Appended the same evidence to the afribbean topic with explicit lineage (Afribbean dropped 8 Nov; thesis moved to the Ambessa Saul lane).
- Why / verdict: East Africa is politically engaged with the Caribbean and commercially absent (CARICOM chair: never been trade; $300m ACTIF deals had no East African counterparty; 2021 Kenya-Barbados air services produced no route). China buys the tender before it opens ($2bn+ financed surveillance, 11 countries). India wins by being the non-Chinese option (Ghana 5G >$200m, UPI licensed to Namibia, TCS sovereign cloud Kenya). Chinese/Indian apps buy distribution at preload and ad spend, not resident teams. PAPSS live in 30+ countries but Nigeria settled only N5.6bn (~$3.6m) H1 2025. Conclusion: the gap is the trusted middle for one mid-market cross-border deal, not a rail and not a tender.
- Status/open: Ambi corrected direction mid-run - this is prep only, no software design, coding sprint is 22 Nov on Claude Code. First real deal pair still unnamed. 10 findings unconfirmed (blocked/JS/PDF sources).
- Related: ~/AUH/AMBESSA/intel/{APPENDIX-16NOV.md,BRIEF.md,SEARCH-PLAYBOOK.md,index.html,pains.db,check.py}

## 2026-11-16 20:20 EAT — MUNGURA — Startup layer: who is shipping into these markets

- What changed: evidence base grew to 214 findings / 204 verified / 15 groups. New groups: startup_cohort (Google Africa Applied AI Lab 2026), small_ai_startups, offer_teardown, crossborder_startups, how_they_sell, faceless_and_caribbean. New file REVERSE-ENGINEER.md (mechanics worth borrowing, mechanics to avoid). Fixed a real gate bug: kwanex.com matched "x.com" as a substring and was misrouted to the X-capture route; host is now parsed exactly.
- Why / verdict: the Africa-Caribbean corridor is live but unserved - WapiPay is the only licensed live startup corridor (BoJ approval, JN Money payout), Knova runs a Jamaica-Ghana trade corridor, and Zeepay's Barbados arm was suspended by the central bank and wound up. Pricing that works here is flat per seat with all modules (Cirquu N9,000 ~ $7), seat-not-AI (Knowlix $24.90, Bujeti N17k-35k), credits for heavy users (Decide $7/500), local currency + mobile money (Meditect 50,000 XOF/yr). Selling is founder-DM-the-principal plus one public artefact; WhatsApp is the checkout (Bill Express J$55/bill). Faceless brands win the commodity end but never show a named client; the face wins the trust end.
- Status/open: this remains PREP ONLY per Ambi - no software design, no product decision. Unverified 10 of 214. Still open: which mechanics we adopt for our own funnel, and the first named deal pair.
- Related: ~/AUH/AMBESSA/intel/{REVERSE-ENGINEER.md,APPENDIX-16NOV.md,index.html,pains.db,raw3/}

## 2026-11-16 21:17 EAT — MUNGURA — Ambessa venture registered as the North Star, context pack published

**Changed.** Two Memoir project pages written and registered in `topics.json` and `project-maps.json as one project `ambessa`: `ambessa-venture` (the North Star, chosen, unnamed) and `ambessa-context` (the public context pack). Map screen works: `memory_cli.py map ambessa`; `map-check` 314 checked, 0 failed. State notes set on both topics. Mission topic appended with the North Star move. `~/.hermes/SOUL.md` gained "How We Think — the models" (thirteen lenses) plus an income line inside Money Urgency; gericho, electrika and titus SOULs point at it. Public pack at https://github.com/AmbessaTrades/ambessa-context rebuilt to 36 files, idempotent (second run `changed: 0`), daily cron `Context pack sync` 07:00 silent unless something moved.

**Why-verdict.** Ambi called the venture the single North Star and told me to stop stating open items as decided. Every hand-written doc in the pack now says "exploring / candidate / open"; the generated digest and the Genspark blocks were rewritten the same way. The rule is now in SOUL for every bot, not just in a repo file.

**Status-open.** No name, no first paying client, no chosen first offer. Thirteen image slots in the brief are still empty — only the portrait reached disk as a file; the rest arrived as literal `!image.png` text. Pack journal window is seven days.

**Related.** `10 Projects/Ambessa Saul venture.md`, `10 Projects/Ambessa Context Pack.md`, `~/AUH/AMBESSA/sync_context_repo.py`, memory topic `mission`, `10 Projects/Afribbean`.

## 2026-11-17

> Message-level context for this day. Auto-logged.

---

## 2026-11-17 04:29 EAT — MUNGURA — Weekly summary failed
<!-- type: event_bus -->
**From:** mungura

Weekly summary generation failed after 1 attempt(s): attempt 1/5: Weekly summary generation failed on every route: DeepSeek Flash: session_id: local-4be983dd6d3eb9622e1d4caa37c10e9aeca9d50ff1b0ad5ea053311eb517568a | DeepSeek V4 Pro: session_id: local-40e1d551a57fa92d85c66319f75c2519c33280260a426238639d5340b9fbde27
Component: weekly-summary-gpt55
Severity: error
Tags: prompt4, longterm-weekly

---

## 2026-11-17 08:45 EAT — TEHUTI — TubeLoop backup left out 7 file(s) that contain keys
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup left out 7 file(s) that contain keys
- Left out (secret found, value not shown): home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/research/study-1108/vidrush/pages/builtin.html [google api key]; home/AUH/Loop/jobs/verse/_config/active-hotkeys.json [a live key value]; home/AUH/Loop/src/components/AudioDashboard.tsx [a live key value]
- Left out (over size cap): home/AUH/Loop/loop/revival/bygone/bygone-highest-state.webm (71 MB); home/AUH/Blacksite/data/packages/ep-mvfpm7ln-770d0be167.zip (104 MB); home/AUH/Blacksite/data/wedjat-adsb/2026-10-21.json (134 MB)
- Fix: move the key into the folder's .env (the keys backup picks it up) or add the path to secret_allow in ~/.auh-git/projects/tubeloop/project.json if it is not a real key.
- Status: blocked — needs an agent to look

---

## 2026-11-17 08:45 EAT — TEHUTI — TubeLoop backup kept the last saved copy of a folder that shrank or vanished
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup kept the last saved copy of a folder that shrank or vanished
- Kept last saved version (safety): home/AUH/CloneEngine — lost 174 of 175 files
- Status: blocked — needs an agent to look

---

## 2026-11-17 08:43 EAT — MUNGURA — VMake daily study: LOT thumbnails vs performance
<!-- type: event -->
**From:** MUNGURA

- What happened: LOT 277,000 subs · last 21d 3 uploads · median 3,600 views · views/sub 0.013
- Style that wins now: S1 mean 0.95x best 1.25x — dark, high-contrast, saturated, warm, big face/figure, clean/simple
- Own outliers: 13.89x “Your SEM3N Is SPIRIT You Can Spend”; 11.67x “Your SEM3N Is What Your AURA Is Made Of”; 4.44x “When You DON'T Ejaculate, Your Nerves Go QUI”
- Competitor Beyond The Alchemy (84,100 subs, median 26,000): 26.15x “Why Women Sense Your Energy Instantly (A”; 4.08x “Escaping the Edging Trap: The Dopamine P”
- Competitor Masculine Theory (122,000 subs, median 14,000): 23.14x “Semen retention is nervous system evolut”; 5.07x “It wasn't about semen retention. It was ”
- Competitor The Aligned Men (16,200 subs, median 4,350): 46.9x “I Did PURE Semen Retention For 1 Year, H”; 28.51x “SEMEN RETENTION BENEFITS  | 13+ MIND BLO”
- Competitor Captain Sinbad (554,000 subs, median 11,500): 4.61x “Act like a "hot girl" for success in lif”; 2.78x “You Can Have Everything You Want in 90 D”
- Competitor Semen Retention Club (162,000 subs, median 16,000): 46.88x “Captain Picard - Semen Retention”; 9.0x “She Can't Seduce A Man IMMUNE TO TEMPTAT”
- Competitor Sexual Kung Fu (197,000 subs, median 9,700): 24.95x “Angion Method For Penis Growth and Harde”; 24.64x “Orgasm Without Ejaculating By Retraining”
- Competitor Astral Doorway (308,000 subs, median 3,550): 24.51x “How to Observe Yourself | Key I — 01 • T”; 21.97x “The Spiritual Future of Humanity & End T”
- Competitor Regal Change (26,700 subs, median 2,900): 2.97x “Why You Give Hot Chicks PTSD On Semen Re”; 2.66x “I Couldn't Handle All The Female Attract”
- Competitor Taylor Johnson - Integrative Sexual Health for Men (114,000 subs, median 5,200): 28.65x “Sex Transmutation Explained ✨🔥 (How-To G”; 20.96x “Multiple Ejaculations for Men (Technique”
- Style to borrow: from The Aligned Men best 46.9x — mid-tone, flat, saturated, warm, big face/figure, clean/simple
- Errors: annel/UCboJ1avpnorCXLDU5UauVzg: yt-dlp failed for https://www.youtube.com/channel/UCboJ1avpnorCXLDU5UauVzg/video
- Files changed: /Users/Mungura/AUH/VMake/out/study/study_c44deb7c.json, out/study/study_latest.json
- Verification: 40 videos with real view counts; 40 thumbnails on disk; 1 style clusters
- Catalog re-TN queue (views × ad slots × velocity; basis previous snapshot): #1 7.6% “The 6 Stages of KUNDALINI AWAKENING & ” TN DRAFT SHE IS COILED; #2 7.6% “THE 7 STAGES OF SEMEN RETENTION” TN DRAFT KEEP IT; #3 6.3% “The Reason Masturb*tion is Killing You” TN DRAFT DON'T SPILL
- Fastest movers (v/day): 475 “The 6 Stages of KUNDALINI AWAKENIN”; 475 “Your SEM3N Is What Your AURA Is Ma”; 475 “Why Your Body Is NOT Needed After ”
- META (last 90d, 39 outliers): thumbs are big text at bottom · cleaner / simpler · bigger face / figure ; titles start with WHY · ask a question ; outliers run 0–32 min
- META shift vs last quarter: shorter titles (~8 words vs 9) -1.3→-0.9; ask a question -0.08→+0.12; warn (don't / never / banned) +0.07→-0.12
- LOT vs meta: winners are more muted · one field · flatter than LOT's last 12
- Status: complete


## 2026-11-17 08:05 EAT — MUNGURA — The rejected-ideas log: eleven dead rounds saved as dead ground

**Changed.** New Memoir project page `ambessa-rejected` — "Ambessa — ideas explored and rejected" — registered third in Projects (after the venture and the context pack) and pointed to from the venture page. It records all eleven idea rounds with Ambi's own verdict on each, the five reasons an idea died, the numbers with trust labels, the errors that session admitted, and its reading of Ambi marked as a claim rather than canon. Same content published in the public pack as `05-offers/explored-and-rejected.md`, with personal details removed.

**Why-verdict.** He spent a long session with another AI and his verdict was "it fell short in a lot of places… it's just not it". Saving the ideas matters less than saving the rejections: the next agent must know this is dead ground and may re-propose one only with new evidence. Ambi's words outrank the other agent's summary where they disagree (price band $5k–$25k, buyer ceiling $5B).

**Status-open.** The eleventh set, led by the EU Forest-Rule File, was never judged. No idea yet has a named penalty, a finished sample and a buyer saying yes.

**Related.** `10 Projects/Ambessa — ideas explored and rejected.md`, `10 Projects/Ambessa Saul venture.md`, `05-offers/explored-and-rejected.md`, topic `ambessa-rejected`.

## 2026-11-17 11:20 EAT — MUNGURA — The visual shelf: fourteen direction images published as a permanent library

**Changed.** `09-assets/library/` in the public pack now holds fourteen images Ambi sent as direction, each named for its job, with `LIBRARY.md` (what to steal from each) and `library.json` (machine index with raw URLs). Covers X profile and pin architecture, the forty-two AI writing tells, the skills/model/design-system diagram, a private-versus-confidential payments flow, a trending panel to turn into a decision-maker panel, a serif landing hero, and the boldness-to-brains axis. Digest now points at it under VISUAL LIBRARY.

**Why-verdict.** He asked for a Pinterest that survives every session and that he can point an agent at by URL. Keeping the images in chat loses them; keeping them on disk hides them; a public folder plus an index makes them usable by any agent, any week, without him re-explaining a single picture.

**Status-open.** More images are still arriving, and the twelve `!image.png` placeholders from the founding brief remain empty — only the portrait and these fourteen exist as files.

**Related.** `09-assets/library/LIBRARY.md`, `09-assets/library/library.json`, `09-assets/ambessa-saul-profile.png`, topic `ambessa-context`.

## 2026-11-17 11:45 EAT — MUNGURA — The master brief rebuilt: 5,677 words, twenty-four sections

**Changed.** `~/AUH/AMBESSA/intel/MASTER-BRIEF.md` — the giant brain-dump reshaped, longer than the original and ordered for fan-out: twelve workstreams each with owner, artefact and check; account plumbing (which handle and email governs X versus YouTube); week-by-week sprint; the five walls with quotable numbers; reply doctrine; four-filter news digest; wide-surface/narrow-door resolution; the floor if nothing sells; eight open questions in one batch for Ambi. Same job given to a cloud agent for comparison.

**Why-verdict.** His instruction was explicit: keep every nuance, keep the machine-only references to T3 Code, Hermes, Memoir and the bots, map the links and images where they belong, and lengthen rather than compress. The value is not length — it is that a child agent can be handed one row and one law set instead of the whole dump.

**Status-open.** Eight questions await his answer, starting with the name, the first market and the first offer. The fourteen library images and the portrait are the only visual assets on disk; the twelve founding-brief placeholders are still empty.

**Related.** `~/AUH/AMBESSA/intel/MASTER-BRIEF.md`, `09-assets/library/`, topics `ambessa-venture`, `ambessa-context`.

## 2026-11-17 12:40 EAT — MUNGURA — Brief v2 merged against the cloud agent, mental models rewritten, gallery proven

**Changed.** `MASTER-BRIEF.md` is now 10,581 words and eighteen parts, merging the cloud agent's structure (authority order, decided/open/dead tables, the forty-two tics, the verified Tan detail, link and image indexes, thirty-four agents in eight units, the weakest-assumption paragraph) with what this bot had (corrected evidence counts, the five walls, account plumbing, reply doctrine, digest filters, guardrails, the visual library). Added in the merge: a ten-stage pipeline for one piece of content, a first-seventy-two-hours sequence, and a Poteto-to-our-vocabulary translation table. `01-who/mental-models.md` rewritten to fourteen named lenses with the quotes he saved. `09-assets/library/GALLERY.html` renders all fourteen images — verified 14 of 14 loaded, zero broken.

**Why-verdict.** He asked which was better and to keep the best of both. The cloud agent held length and structure; this bot held the evidence correction, the library and the machine context. Neither was sufficient alone, and the merged file is longer than both.

**Status-open.** Ten questions await his answers. Three X links are still unknown (callumhyman24 x2, Rames_Jusso), the Alexandr Wang video link was never supplied, and the short link beside the OCR note is unresolved.

**Related.** `~/AUH/AMBESSA/intel/MASTER-BRIEF.md`, `MASTER-BRIEF-v1.md`, `01-who/mental-models.md`, `09-assets/library/GALLERY.html`.

## 2026-11-17 13:20 EAT — MUNGURA — Fourteen venture skills built, the copy gate proven, tokens written

**Changed.** New `ambessa` skill group: 14 skills written to `~/.hermes/skills/ambessa` and copied into gericho-orchestrate, electrika and titus. Voice, news lane, thumb/title, video system, brand tokens, software surface, reply doctrine, X brand, decision map, offer design, dossier, morning brief, wave supervisor, and `copy-tic-check` with a working `tic_check.py`. Design system written at `~/AUH/AMBESSA/design-system/tokens.json` (accent deliberately open, two candidates). Index at `skills/ambessa/README.md` naming the lane owner per skill.

**Why-verdict.** The 496-skill library was deep on LOT/Blacksite craft and nearly empty on the venture itself. Prose rules were also being ignored, which is the exact failure Poteto names, so the copy gate ships as a script: a sloppy sample trips 15 hard hits and exits 1, a tight sample passes with one soft note. Loader verified — `skill_view copy-tic-check` returns the skill and its linked script.

**Status-open.** No pointer patches yet in `humanizer`, `title-formulas`, `xitter`; no Hermes plugin built. The `tehuti` profile no longer exists on this machine — only gericho-orchestrate, electrika and titus. Accent colour still unchosen, so every surface stays ink-on-paper until Ambi decides.

**Related.** `~/.hermes/skills/ambessa/`, `~/AUH/AMBESSA/design-system/tokens.json`, `~/AUH/AMBESSA/intel/MASTER-BRIEF.md`, topic `ambessa-venture`.

## 2026-11-17 14:05 EAT — MUNGURA — Twenty skills, the second half built for research and synthesis

**Changed.** Six capability skills added to the ambessa suite: research-sprint, synthesis, source-ledger (with a working `verify_quote.py`), content-factory, question-craft, model-benchmark. Twenty total in the default library and in gericho-orchestrate, electrika and titus. Brief gained Part 20 — the content factory, merging Riley Brown's 16 Nov article with Kallaway's systems-based thinker; now 12,922 words, 21 parts. Routing lines patched into `humanizer`, `title-formulas` and `xitter` in all four libraries.

**Why-verdict.** His correction was exact: the first pass was opinion, not capability, and he cannot answer questions that depend on next week. So the second half is machinery — source tiers, seven synthesis shapes, a quote verifier that fails a fake on contact, and a question protocol that sorts researchable / his taste / not-yet-answerable so bucket three stops reaching him.

**Status-open.** Five decisions remain genuinely open (first product, first country, accent, business-account voice, first software surface) and are recorded as open, not asked again. No Hermes plugin built — both capabilities ship as scripts inside skills instead.

**Related.** `~/.hermes/skills/ambessa/`, `MASTER-BRIEF.md` Part 20, `design-system/tokens.json`, topic `ambessa-venture`.

## 2026-11-17 14:40 EAT — MUNGURA — Scaffold MCP tested, the curve and the boring stretch, Rust recorded

**Changed.** Part 21 appended to the brief (now 13,944 words, 22 parts): the writing-scaffold MCP tested live — 4 tools, 7,262 eligible scaffolds, no key — with the rule that only its structure is borrowed and never its cadence; Wang's exponential-curve advice with the observation that the boring stretch is the moat; and Rust recorded as his instruction with the trade-offs written down (Rust core, thin shell, Python behind a boundary). `ambessa-voice` gained a "borrowing a structure" section pointing at the MCP with the same caveat. Suite recopied, 20 skills in four libraries, brief re-rendered.

**Why-verdict.** He asked whether the MCP is useful, not for an opinion about it. It answers with no key and holds real institutional shapes (S-1 risk sections, press releases, Common Sense), but its own instruction to preserve "cadence and phrasing" would smuggle another writer's voice into copy that must sound like Ambi — so structure only, tic-check after.

**Status-open.** The Wang video itself was never supplied — only the tweet — so the transcript extraction is queued, not done. Rust is a direction, not yet a locked architecture decision; the vertical slice (fetch → verify quote → ledger row → one dossier page) is the test.

**Related.** `MASTER-BRIEF.md` Part 21, `ambessa-voice`, `design-system/tokens.json`, topic `ambessa-venture`.

## 2026-11-17 15:10 EAT — MUNGURA — The self-prompting agent: Finn's model, inverted for his patience

**Changed.** Part 22 appended to the brief (14,886 words, 23 parts) with both Alex Finn posts quoted, and a new skill `ambessa-self-prompt` written, copied to all three profiles (suite now 21 each). The skill runs the interrogation: retrieve, generate a hundred questions, answer what context can settle with confidence labels, write a spec with an acceptance test, decompose into artefacts with checks, execute in waves, report in four beats. Finn's cognitive-load prompt saved verbatim as a monthly routine.

**Why-verdict.** Finn asks the human a hundred questions; a reply to his own post says that would test anyone's patience — and Ambi has four minutes and ADHD. So the hundred go to the agent and only five reach him, which is the version that actually lightens his load rather than relocating the paperwork.

**Status-open.** The monthly cognitive-load run has not been done yet. Nothing is scheduled; the first invocation is the next time a build starts cold.

**Related.** `MASTER-BRIEF.md` Part 22, `ambessa-self-prompt`, `ambessa-question-craft`, `ambessa-wave-supervisor`, topic `ambessa-venture`.

## 2026-11-17 16:05 EAT — MUNGURA — Five critics, 284 findings, the suite rebuilt to zero errors

**Changed.** Dispatched five isolated critics (architecture, executability, domain truth, routing, adversarial) against a frozen copy of the 21-skill suite. They returned 284 findings — 2 critical, 86 high. Rebuilt against them: both gate scripts fail closed (empty input and missing file exit 2, quotes under 40 chars refused, subject must appear in the quote, ledger.csv + verified-only CSV emitted, sha binds the check to the draft, coverage reported honestly as 42/42); every skill now carries a When to use / When not to use / Handoff block, a numbered procedure, a Gates section and a named Output; all 21 descriptions are triggers under 60 characters; tags normalised; an umbrella router skill added at the suite root with a precedence rule; README rewritten to 21 rows; `open-items.json` created so open decisions stop dying with a session.

**Why-verdict.** The critics found what a self-review would not: every gate passed vacuously, the dossier documented a row schema the verifier rejected, fifteen skills had no inbound reference, and the router table lived only in the one install that lacked it. Domain corrections included the $10M–$5B buyer band, the voice no longer pre-deciding an injustice, question-craft no longer parking his decisions, and wave-supervisor starting with eight children rather than twenty-five.

**Status-open.** Five decisions remain his, now recorded in `open-items.json` rather than asked again. The Wang video transcript extraction is still queued for want of a link.

**Related.** `~/.hermes/skills/ambessa/` (ARCHITECTURE.md, _tools/validate_suite.py, README.md, SKILL.md), copies in gericho-orchestrate, electrika and titus, topic `ambessa-venture`.

## 2026-11-17 17:20 EAT — MUNGURA — Both project pages rewritten for the 23rd; 274 unrelated records pruned

**Changed.** `10 Projects/Ambessa Saul venture.md` and `10 Projects/Ambessa Context Pack.md` had their hand-written heads rebuilt around what now exists: the brief (23 parts, 14,886 words), 21 skills plus umbrella with validator exit 0, the two fail-closed gate scripts, the design tokens with the accent open, the 14-image library with gallery, the 214/204 evidence base, 57 published files, `open-items.json` with the five decisions, and a "23rd — where to start" sequence. The context page's machine history was 433KB with 274 records belonging to TubeLoop/VizBatch/GenSpark; those were pruned to 32.9KB, and both pages now carry a line saying everything below the head is machine-generated continuity, not current state. Topic statuses and revisions refreshed; state notes rewritten; `map-check` 314, 0 failed.

**Why-verdict.** He asked that the preparation be visible on the 23rd so the next agent does not redo it. A page whose first screen lists what exists, where it is and what to check is worth more than a page of append history — and the append history was actively wrong, pulling another project's records in.

**Status-open.** Memoir's continuity grouping is still pulling unrelated AUH journal entries into this project; pruning fixed the file, not the cause. If it recurs, the grouping rule in the maintenance pass needs the project root tightened.

**Related.** `10 Projects/Ambessa Saul venture.md`, `10 Projects/Ambessa Context Pack.md`, `10 Projects/Ambessa — ideas explored and rejected.md`, topic `ambessa-venture`, `ambessa-context`.

## 2026-11-17 17:55 EAT — MUNGURA — The IP question answered with numbers, not a build

**Changed.** Part 24 appended to the brief (now 24 parts, 15,935 words): the IP research with costs and a verdict, the reverse-video finding, PsyopAnime as a UI reference, and the design law (software never outshines the marketing; 20–50 review passes). Nord's pricing screenshot added as image 15 in the visual library, LIBRARY.md and library.json updated, gallery rebuilt to 15 of 15, pushed. `OI-6` added to open-items for the IP choice.

**Why-verdict.** He asked whether to reverse-engineer a VPN. The honest answer is no: an IP block, an ASN and an abuse desk are a business, and the only thing needed is one static address. Checked costs: Nord dedicated IP $4.19/mo on two years, $5.89 on one, $8.99 monthly; a Canadian VPS with WireGuard $4–6/mo with our own IP; static-over-WireGuard services $2–4/mo. Also separated what is real from what vendors sell: no public YouTube trust score and no documented down-ranking for IP churn — carriers rotate addresses constantly — but verification friction, location drift and eligibility are real, so the address is worth buying as hygiene.

**Status-open.** Which route he picks (VPS or Nord), and whether the business account gets its own IP. The `reverse-any-video` skill on this machine is the HyperFrames one, gated on Pro auth, so paid Pro is a revenue decision, not a technical one. The Rames_Jusso link returned no content twice and stays unread.

**Related.** `MASTER-BRIEF.md` Part 24, `09-assets/library/15-nord-dedicated-ip-plans.png`, `open-items.json` OI-6, skill `media/reverse-any-video`.

## 2026-11-17 18:20 EAT — MUNGURA — Claude Code is one patch behind; the fix is recorded as a first step

**Changed.** Read Tekon Burns' 17 Nov post through the jina proxy (the direct extract returned nothing). Logged it as §21.4 in the brief and as step 1 of the "23rd — where to start" checklist on the venture page: update Claude Code to 2.1.326 before anything else. Checked this machine: `claude --version` returns **2.1.325**, one patch behind, so every T3 Code session is still paying the 93K-token config overhead.

**Why-verdict.** He asked for it to be appended where it belongs and for the agent to update itself. The post's numbers are operational, not conceptual — 86% overhead cut, stale-settings fix, recaps no longer billed — so it belongs in the environment notes with a verification step, not in the strategy parts. The one caveat worth carrying: opusplan compaction now runs on Opus, so compaction costs more.

**Status-open.** The update has not been run from here — it happens on the next T3 Code session, which is his to start. After updating, verify `/update-config` reads in the low thousands of tokens and log the before/after.

**Related.** `MASTER-BRIEF.md` §21.4, `10 Projects/Ambessa Saul venture.md` (23rd checklist), source `x.com/TekonBurns/status/2122598865627209940`.

## 2026-11-17 18:45 EAT — MUNGURA — The follow graph becomes an instrument; two market signals logged

**Changed.** §7.7 added to the brief — the standing instruction to scan every account on `x.com/Ambessa_Saul/following` with cheap workers (one per ten accounts, fixed JSON per handle: role, country, three items each with URL/date/verbatim quote, allusions, who they amplify, can they sign or pay) and an Opus overseer clustering against the five walls into a twenty-signal report, weekly deltas after the first full pass. §9.7 added — Stephen Deng's five-criteria DFS Ventures pattern, logged as a rubric for our own offer, and Terra's $52m SpaceX round with the reply backlash recorded as the lesson about funding headlines in this market.

**Why-verdict.** He asked for the graph to be treated as a training corpus rather than a feed, and for the two posts to be appended without adjudication. Both are now written so the next agent can act: the scan produces files, not impressions; the Deng rubric gives a pass/fail against our own wedge; the Terra thread shows what happens within hours to any company claim published without a primary record.

**Status-open.** The first full scan has not been run. Nothing in §9.7 is verified by us — Terra's funding and the allegations in the replies are recorded as posted, with attributions intact.

**Related.** `MASTER-BRIEF.md` §7.7 and §9.7, sources `x.com/mrstephendeng/status/2122593058607935` and `x.com/carter8f/status/2122394732450009498`, topic `ambessa-venture`.

## 2026-11-17 19:10 EAT — MUNGURA — Hindsight installed and configured, held off for disk

**Changed.** Installed the Hindsight memory provider (catalog 1.2.4) into the gericho-orchestrate profile and configured it at `~/.hindsight/config.json` — shared across profiles, `bank_id: memoir`, daemon profile `hermes`, LLM `openai_compatible` at DeepSeek, idle timeout 30 min — with the key in `~/.hermes/.env` as `HINDSI

_[truncated in this pack; full day log stays on the machine]

## 2026-11-18

> Message-level context for this day. Auto-logged.

---

## 2026-11-18 00:04 EAT — MUNGURA — Daily journal generated for 2026-11-08; status=success; db_length=57949; source_hash=135968598845.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-08; status=success; db_length=57949; source_hash=135968598845.

---

### [00:04] Exchange: Daily journal worker run for 2026-11-08

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-08`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-08.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-08.md`.
- DB row length: `57949`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-08.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-08.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-08.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-08.md.pre-sonnet5-repair-20261117_235908.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-08.md.pre-sonnet5-repair-20261117_235908.bak.
**Journal Dates Repaired:** 2026-11-08.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=57949, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:10 EAT — MUNGURA — Daily journal generated for 2026-11-09; status=success; db_length=77062; source_hash=2a482716af31.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-09; status=success; db_length=77062; source_hash=2a482716af31.

---

### [00:10] Exchange: Daily journal worker run for 2026-11-09

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-09`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-09.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-09.md`.
- DB row length: `77062`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-09.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-09.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-09.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-09.md.pre-sonnet5-repair-20261118_000422.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-09.md.pre-sonnet5-repair-20261118_000422.bak.
**Journal Dates Repaired:** 2026-11-09.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=77062, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:15 EAT — MUNGURA — Daily journal generated for 2026-11-10; status=success; db_length=64341; source_hash=fef9d9c09c5e.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-10; status=success; db_length=64341; source_hash=fef9d9c09c5e.

---

### [00:15] Exchange: Daily journal worker run for 2026-11-10

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-10`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-10.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-10.md`.
- DB row length: `64341`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-10.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-10.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-10.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-10.md.pre-sonnet5-repair-20261118_001025.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-10.md.pre-sonnet5-repair-20261118_001025.bak.
**Journal Dates Repaired:** 2026-11-10.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=64341, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:21 EAT — MUNGURA — Daily journal generated for 2026-11-11; status=success; db_length=32639; source_hash=4199de27d62a.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-11; status=success; db_length=32639; source_hash=4199de27d62a.

---

### [00:21] Exchange: Daily journal worker run for 2026-11-11

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-11`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-11.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-11.md`.
- DB row length: `32639`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-11.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-11.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-11.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-11.md.pre-sonnet5-repair-20261118_001506.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-11.md.pre-sonnet5-repair-20261118_001506.bak.
**Journal Dates Repaired:** 2026-11-11.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=32639, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:25 EAT — MUNGURA — Message to her checked: Kenyaplex holds, Somovibe does not, and the 22nd is a promise

- **Changed:** Verified the two marketplace claims in the drafted message against the attached pages. Kenyaplex: 50% commission, KSh 1,000 payout threshold, 48-hour review, M-Pesa — every figure confirmed on its own page. Somovibe: 75% confirmed, and the contradiction is real — the hero says free with no card, the FAQ says a one-time KES 100 verification fee by M-Pesa.
- **Why/verdict:** The message is honest and correctly refuses to promise a salary. Two things should change before it goes: (1) Somovibe asks for money before she earns, which is the pattern scam advisories in Kenya flag, so Kenyaplex should be the only one she touches; (2) "give us until the 22nd" is a dated promise, and the documented failure mode is exactly a promise followed by waiting. A trigger beats a date.
- **Status/open:** Nothing sent by me; the message is Ambi's to send. Flagged that her only device is a phone, so any note-selling path needs a phone-to-PDF step, which the draft does not mention.
- **Related:** `MASTER-BRIEF.md` Part 28 (28.8 the waiting pattern, 28.10 questions); day log; Kenyaplex sell-notes page; Somovibe site.

## 2026-11-18 00:25 EAT — MUNGURA — Daily journal generated for 2026-11-12; status=success; db_length=34508; source_hash=af815ed7e819.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-12; status=success; db_length=34508; source_hash=af815ed7e819.

---

### [00:25] Exchange: Daily journal worker run for 2026-11-12

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-12`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-12.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-12.md`.
- DB row length: `34508`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-12.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-12.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-12.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-12.md.pre-sonnet5-repair-20261118_002150.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-12.md.pre-sonnet5-repair-20261118_002150.bak.
**Journal Dates Repaired:** 2026-11-12.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=34508, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:26 EAT — MUNGURA — Daily journal generated for 2026-11-13; status=success; db_length=28807; source_hash=f189c57bf8bc.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-13; status=success; db_length=28807; source_hash=f189c57bf8bc.

---

### [00:26] Exchange: Daily journal worker run for 2026-11-13

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-13`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-13.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-13.md`.
- DB row length: `28807`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-13.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-13.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-13.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-13.md.pre-sonnet5-repair-20261118_002508.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-13.md.pre-sonnet5-repair-20261118_002508.bak.
**Journal Dates Repaired:** 2026-11-13.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=28807, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:31 EAT — MUNGURA — Daily journal generated for 2026-11-14; status=success; db_length=13856; source_hash=533202dd777f.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-14; status=success; db_length=13856; source_hash=533202dd777f.

---

### [00:31] Exchange: Daily journal worker run for 2026-11-14

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-14`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-14.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-14.md`.
- DB row length: `13856`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-14.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-14.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-14.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-14.md.pre-sonnet5-repair-20261118_002628.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-14.md.pre-sonnet5-repair-20261118_002628.bak.
**Journal Dates Repaired:** 2026-11-14.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=13856, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:35 EAT — MUNGURA — Her answer: "I'll wait for Ambi and his company… the notes idea won't get things done"

- **Changed:** Recorded her first words in `MASTER-BRIEF.md` Part 28 (28.8, plus a new question 5 in 28.10); brief 32,186 words, HTML re-rendered at 207,243 bytes.
- **Why/verdict:** The notes route asked her to produce and sell alone with no buyer guaranteed, so she is right that it would not "get things done" — it cannot reach the seven-hundred-dollar figure anyone named. But "I'll wait" is the failure pattern from 28.8 speaking in her own voice: if nothing arrives, the attempt ends without anyone having to call it off.
- **Status/open:** No lane exists that needs no build, and the one document a reader-lane would need is not on disk — the recent LOT files in `~/LOT Files/LOT/ts-p/` are visual prompt packages, not spoken scripts. First handover has to come from Notion or be exported.
- **Related:** `MASTER-BRIEF.md` 28.8, 28.9 item 3, 28.10; `2026-11-18.md` earlier entry on the marketplace check.

## 2026-11-18 00:33 EAT — MUNGURA — Daily journal generated for 2026-11-15; status=success; db_length=14786; source_hash=5ab29382c543.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-15; status=success; db_length=14786; source_hash=5ab29382c543.

---

### [00:33] Exchange: Daily journal worker run for 2026-11-15

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-15`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-15.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-15.md`.
- DB row length: `14786`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-15.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-15.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-15.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-15.md.pre-sonnet5-repair-20261118_003120.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-15.md.pre-sonnet5-repair-20261118_003120.bak.
**Journal Dates Repaired:** 2026-11-15.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=14786, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:35 EAT — MUNGURA — Daily journal generated for 2026-11-16; status=success; db_length=20194; source_hash=01b7fe121119.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-16; status=success; db_length=20194; source_hash=01b7fe121119.

---

### [00:35] Exchange: Daily journal worker run for 2026-11-16

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-16`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-16.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-16.md`.
- DB row length: `20194`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-16.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-16.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-16.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db.
**Journal Dates Repaired:** 2026-11-16.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=20194, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 00:40 EAT — MUNGURA — Tested from Kenya: Mercor is open at $40–$75/hr, Outlier is a hard block

- **Changed:** Ran the platforms from this machine's Kenyan connection instead of reading blogs about them. Results: **Mercor loads and lists live maths work — Mathematics Expert $40–$75/hr, Mathematics Domain Expert $90–$140/hr, Life/Physical/Social Science Expert $60–$120/hr, Mathematician Talent Network $60–$80/hr**; the Mathematics Expert page confirms $40–$75/hr, a standing talent pool, resume plus "confirm where you work from", then a ~20-minute AI interview reused across every later role. **Alignerr loads and hires across all domains**, $80/hr average, math experts $25–$100/hr, async, min 15 hrs/week, AI interviewer. **Outlier is a hard location block** — app.outlier.ai returns "we are not able to provide service in your location", which contradicts the Kenyan blogs claiming it accepts Kenya. CrowdGen fails at the certificate.
- **Why/verdict:** She is already inside Mercor and has been paid by them, which is the part a new applicant has to earn. At the low end of the listed maths rate, 20 hours a month is $800 — her stated floor — using the credential she already holds. The single gate is a 20-minute AI interview, believed to be voice or video, which is the one thing she has refused; that is now the only open question in the lane.
- **Status/open:** Brief Part 28 updated — 28.9 items 5–9 rewritten with the tested evidence, 28.1 corrected to record the unresolved laptop contradiction (phone-only vs a slow laptop). Brief 32,561 words, HTML 209,787 bytes. Nothing sent to her; the message is Ambi's to send.
- **Related:** `MASTER-BRIEF.md` 28.1, 28.9; day log `2026-11-18.md`; work.mercor.com/jobs/list_AAABoKMjug1fFXpwuDdIZ6TO/mathematics-expert; app.outlier.ai location wall.

## 2026-11-18 00:41 EAT — MUNGURA — Daily journal generated for 2026-11-17; status=success; db_length=46398; source_hash=082c6d4c7784.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-17; status=success; db_length=46398; source_hash=082c6d4c7784.

---

### [00:41] Exchange: Daily journal worker run for 2026-11-17

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `catch-up` mode.

**Actions:**
- Target date: `2026-11-17`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-17.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-17.md`.
- DB row length: `46398`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-17.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-17.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-17.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-17.md.pre-sonnet5-repair-20261118_003505.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-17.md.pre-sonnet5-repair-20261118_003505.bak.
**Journal Dates Repaired:** 2026-11-17.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `catch-up`.
**Verification Results:** files written, SUMMARY mirror written, DB length=46398, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-18 12:10 EAT — MUNGURA — Part 29 written: five speaking sources and the drill spec

**Changed.** Added `PART 29` to `MASTER-BRIEF.md` (now 33,833 words, HTML 218 KB, re-rendered): the five links he sent (Joseph Tsar articulate course 36:27, Kallaway S-Tier ranking formula 1:38, Victor on growth content 10:43, and two Naval posts), each with URL, runtime, what it is, and what to extract; a rule that the agent watches them rather than inheriting a summary; what each source may and may not change; and his drill design written as a spec — 50-word, 100-word, recorded story, 3-5 prompts, required structures and keywords, raw dictation kept, output a lexicon in four registers. Part 12 link index gained rows 31-35.

**Why verdict.** He did not ask for a transcript — he asked for the links to be placed where the agent will find them, with enough context to know why he wants them watched. The evidence rule from the rest of the file was applied to the viewing step: five bullets plus one timestamped quote, so a structure cannot be claimed without a timestamp.

**Status open.** No transcript taken, deliberately. The drill protocol is a proposal; the first session has not run. Whether the lexicon is read automatically by the copy lane or consulted by hand is undecided.

**Related.** Brief `.bak-part29`; Part 3.7, 3.11, 3.14, 5.6, 25.2, 27.3; X post ids 2122750358493728998, 2122915595897221548, 2122767295630213543, 2118479933530063135, 2105231982309564765.

## 2026-11-18 12:53 EAT — MUNGURA — Naming opened: four Hex terms added, Studio restarted, first round rejected

**Changed.** Added `Alfajiri`, `Medu Neter`, `Neter`, `Netarianism` to Hex through its own CLI (149 vocabulary terms, replacements 54 → 68) and started Studio AUH on `127.0.0.1:3030` (pid 14944). Read the Bible, `library.sqlite` and `studio.db`: 25 beings (5 Kemet, 8 south, 12 snow), and the IP tree's three terms — Kemet, The Two Lands, Working, "any use of power put into words, sound, number or shape".

**Why verdict.** He asked for world-building inspiration, not a product name yet. The IP tree already contains a doctrine: every working has a price.

**Status open.** Naming unresolved. First round (Per Ankh, Tehuti, Pramana, Nyaya, Terma) rejected or killed on ownership.

**Related.** `~/AUH/Studio/STUDIO-AUH-BIBLE.md`; `studio.db` ip_terms; Hex pid 3920.

## 2026-11-18 12:58 EAT — MUNGURA — Terma killed as a defence contractor; Zama and Cannae killed as endings

**Changed.** Verified Terma A/S: Danish aerospace, defence and security, founded 1949, Lystrup, owned by the Thomas B. Thrige Foundation, ~2,600 staff. Proposed Terton, Zama, Cannae instead.

**Why verdict.** He objected on principle, not taste: Zama is an existing Kenyan software company, and both battles end the general rather than crown him — "why would the end of one of our great sovereign emperors represent his last battle".

**Status open.** No name. The rule "the record ends empires, not the battle" enters the working set.

**Related.** `terma.com`; war maps in `~/AUH/STUDY/warmaps-*` (Cannae 53 mentions, Zama, Thermopylae).

## 2026-11-18 13:05 EAT — MUNGURA — Six unifications, three grades of certainty, Yaqin and Tawy raised

**Changed.** Kemet unified six times (Narmer, Mentuhotep II, Ahmose I, Piye, Psamtik I, Ptolemaic consolidation), five of them res

_[truncated in this pack; full day log stays on the machine]

## 2026-11-19

> Message-level context for this day. Auto-logged.

---

## 2026-11-19 00:09 EAT — MUNGURA — Daily journal generated for 2026-11-18; status=success; db_length=45247; source_hash=96cbdd3c51c6.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-18; status=success; db_length=45247; source_hash=96cbdd3c51c6.

---

### [00:09] Exchange: Daily journal worker run for 2026-11-18

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `scheduler` mode.

**Actions:**
- Target date: `2026-11-18`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-18.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-18.md`.
- DB row length: `45247`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-18.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-18.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-18.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db.
**Journal Dates Repaired:** 2026-11-18.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `scheduler`.
**Verification Results:** files written, SUMMARY mirror written, DB length=45247, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-19 00:25 EAT — MUNGURA — Daily journal generated for 2026-11-18; status=success; db_length=45245; source_hash=ad9f99b332d8.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-18; status=success; db_length=45245; source_hash=ad9f99b332d8.

---

### [00:25] Exchange: Daily journal worker run for 2026-11-18

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `scheduler` mode.

**Actions:**
- Target date: `2026-11-18`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-18.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-18.md`.
- DB row length: `45245`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-18.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-18.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-18.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-18.md.pre-sonnet5-repair-20261119_002055.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-18.md.pre-sonnet5-repair-20261119_002055.bak.
**Journal Dates Repaired:** 2026-11-18.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `scheduler`.
**Verification Results:** files written, SUMMARY mirror written, DB length=45245, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-19 09:05 EAT — MUNGURA — Pivot: faceless YouTube pipeline, Loop becomes the product

**Changed.** Ambi's decision after a night of deliberation, in his words: the face channel is dropped; the business is a really good YouTube pipeline leaning on ad revenue. Loop is stripped down and rebuilt as a standalone pipeline software that works for an upgraded video type — design-system led, scalable horizontally to other niches — with a mobile APK so his girlfriend can run a channel from her phone. Three channels from one codebase: two of his, one of hers. A ~$70 tier is a candidate, not a decision; 30 existing paying members prove people will pay for LOT. The Ambessa govcon/venture framing is parked and the context GitHub is to be revised before any SOUL.md is touched.

**Why verdict.** Money now beats a long build: his words, "if we focus on making the software good, LOT will be good". The last four months of LOT quality are judged mid and the proof is that the channel underperformed while the same posting cadence used to earn.

**Status open.** Everything below is unasked: what Loop is for (private tool vs product), which three faceless formats, what the IP actually is, whether LOT relaunches as itself, and what her daily loop looks like. `grill-with-docs` skill created; round 1 about to run. Notion reported not up.

**Related.** `~/.hermes/skills/software-development/grill-with-docs`; Loop at `~/AUH/Loop`; context pack to be revised before SOULs.

## 2026-11-19 12:22 EAT — MUNGURA — Loop gets its glossary and ADR 0001: private tool

**Changed.** Two new files landed in `~/AUH/Loop` at 12:14: `GLOSSARY.md` (1,028 B, six terms — Loop, private tool, IP (address), faceless, spine, niche bend) and `docs/adr/0001-loop-is-a-private-tool.md` (1,041 B). The ADR is marked accepted 2026-11-19, decision: "Loop v1 is a private tool for three channels: two of Ambi's and one run by his girlfriend from her phone. It is not sold." Consequences: no tenancy, no billing, no onboarding, no marketing site, and any feature justified by "a customer would want it" is out of scope until the channels earn. Memoir ingested it as source `6ae6079a00981e74a6b33435` (captured 12:20:46) and the Loop topic's Sources index now carries the line at `~/debate-agent/memory/vault/10 Projects/Loop.md:134`.

**Why verdict.** Ambi had already said it in chat — "it's definitely a private tool, bro." — so the round wrote it as accepted with his words quoted instead of asking again; the glossary terms are his own wording, one line each, no definition he has not used. This is the paper trail the day's 09:05 pivot needed before any build.

**Status open.** No blocking open question, no spec, no channel pick and no build plan are on disk past these two files. Both are untracked (`?? GLOSSARY.md`, `?? docs/adr/`) and the Loop repo holds 327 dirty status lines, so nothing of today is committed.

**Related.** `~/AUH/Loop/GLOSSARY.md`, `~/AUH/Loop/docs/adr/0001-loop-is-a-private-tool.md`, skill `~/.hermes/profiles/gericho-orchestrate/skills/software-development/grill-with-docs/SKILL.md` (modified 11:58), Loop topic `10 Projects/Loop.md`.

## 2026-11-19 12:23 EAT — MUNGURA — Psyop study folder holds a 404, not the post

**Changed.** `~/AUH/STUDY/psyop-2026-11-19/` was created at 12:13 and contains exactly one file: `tweet.html`, 51,770 B, whose `<title>` is `Post Not Found - X | 404 Error` and whose og metadata is X's own error shell. No notes, no images, no second capture in the folder.

**Why verdict.** Logged as a defect, not a result: a folder named for the study looks like captured evidence but proves nothing about the post, and the size of the file would pass any check that counts bytes instead of reading the page.

**Status open.** The source being studied is not captured — a live URL, an archived copy or a screenshot is needed before any claim is built on it.

**Related.** `~/AUH/STUDY/psyop-2026-11-19/tweet.html`.

## 2026-11-19 12:35 EAT — MUNGURA — Audit findings, fourth-pass skill, benchmark to log

**Changed.** Fixed the two apps: Notion 7.11.0 in /Applications was owned by another user and below the minimum build; the 7.41.1 copy in ~/Applications would not launch through LaunchServices, so it was launched directly and a durable copy installed as `/Applications/Notion 7.41.app`. Obsidian was already open on `LOT revival board.excalidraw` in the LOT+AAY vault. Created the `fourth-pass` skill (six passes; first two are what a model produces by default). Audit measurements taken: Loop has 57 Rust files and **726 TypeScript files**; 42 skills, the same set copied into all three profiles and shared; Memoir 6.3 GB with 22 project pages; two Hermes crons and two launchd jobs, neither on the money path.

**Why verdict.** The repeat failures are not model failures: the engine is small and contract-driven while the app around it is 726 files nobody can hold, and the skills are descriptions rather than gates — only a handful have scripts that fail closed.

**Status open.** Ambi's benchmark prompt to be kept for reuse: pick the most-used and most token-heavy task, ask 3 questions in one batch, freeze it as one prompt plus files, run it per model in fresh sessions at equal effort, record cost/time/tokens, put results side by side on one page, save it for the next model release. No Opus 5.5 on this harness — upgrades that need Opus belong to T3/Claude Code.

**Related.** `fourth-pass` skill; `~/AUH/Loop/GLOSSARY.md`; ADR 0001.

## 2026-11-19 13:40 EAT — MUNGURA — Documents cannot assert what Ambi has not decided

**Changed.** Ambi's rule for every document: it must carry a disclaimer at the top that it is subject to change through continued conversation and continued building, and that nothing in it is decided until he says so. Written as `staging/DISCLAIMER.md` and auto-stamped onto every staged section. He also corrected the money framing in the draft: "50k is an outcome, not a plan" is acceptable as a line, but no product, course or tier may be asserted. His order: all focus and tokens on the software so the videos get out and the views return; a moderately ticketed product is wanted but comes after, and reverse-engineering from a high ticket is a method he likes, not the current move.

**Why verdict.** He is protecting the document from becoming a plan he never agreed to; the failure mode is an agent's assumption hardening into a requirement the builder then obeys.

**Status open.** Not settled: the first paid thing and its timing; what happens to the ~30 existing members during the rebuild; whether ~$70 buys the app, a pack, or membership; what "moderately ticketed" means in numbers; and which product shape connects to the app later (SaaS, done-for-you, or teaching).

**Related.** `staging/DISCLAIMER.md`; six section writers in flight (`deleg_154f5377`).

## 2026-11-19 15:10 EAT — MUNGURA — Thirty niche references, six capability classes

**Changed.** Both playlists sampled frame by frame: playlist one (15 videos, longform realistic story) and playlist two (15 videos, "creative new niches", unlisted). New brief section 13 maps all thirty to six capability classes — dated map simulation, game HUD over a plate, screen capture, game capture, CG scene, chat UI — with the render arithmetic: 36,000 frames for a 25-minute film, 20–60 minutes of machine time for a simple three.js scene, inside Ambi's six-hour ceiling. The gallery now carries three contact sheets for playlist one.

**Why verdict.** The most expensive reference in the set is not the 3D — it is one CG interior reused across thirty minutes. The cheapest is Earthlore's screen-recorded Google Earth at 1.7M views. Throughput, not spectacle, is what three channels at ninety videos requires.

**Status open.** Playlist two's frames are downloading. The Server History channel (Discord-chat format, 253K and 245K views) is a reference, not a failure — but the abandoned chat-lane software we built a spec for is a failed project and belongs in the project audit. Ambi's instruction: every success and failure goes into the brief and into the context repo.

**Related.** `staging/master-brief/13-niche-map.md`; `meta/playlist1.txt`, `meta/playlist2.txt`; sheets `p1-1..3.jpg`.

## 2026-11-19 18:25 EAT — TEHUTI — TubeLoop backup left out 7 file(s) that contain keys
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup left out 7 file(s) that contain keys
- Left out (secret found, value not shown): home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T10-12-58-wedjat-fd34/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/dist/assets/studio-WGq3jXIg.js [a live key value]; home/AUH/Blacksite/data/lanes/2026-10-28T11-10-10-wedjat-e5a0/backup/vendor/godseye-lite/src/wedjat/studio.js [a live key value]; home/AUH/Blacksite/research/study-1108/vidrush/pages/builtin.html [google api key]; home/AUH/Loop/jobs/verse/_config/active-hotkeys.json [a live key value]; home/AUH/Loop/src/components/AudioDashboard.tsx [a live key value]
- Left out (over size cap): home/AUH/Loop/loop/revival/bygone/bygone-highest-state.webm (71 MB); home/Documents/Codex/2026-10-07/realtime-voice-chat/outputs/AUH-Studio-Research/START-HERE.html (70 MB); home/Documents/Codex/2026-10-07/realtime-voice-chat/outputs/AUH-Studio-Research/research.json (50 MB); home/Documents/Codex/2026-10-07/realtime-voice-chat/outputs/AUH-Studio-Research/research.sqlite (182 MB); home/AUH/Blacksite/data/packages/ep-mvfpm7ln-770d0be167.zip (104 MB); home/AUH/Blacksite/data/wedjat-adsb/2026-10-21.json (134 MB)
- Fix: move the key into the folder's .env (the keys backup picks it up) or add the path to secret_allow in ~/.auh-git/projects/tubeloop/project.json if it is not a real key.
- Status: blocked — needs an agent to look

---

## 2026-11-19 18:25 EAT — TEHUTI — TubeLoop backup kept the last saved copy of a folder that shrank or vanished
<!-- type: event -->
**From:** TEHUTI

TubeLoop backup kept the last saved copy of a folder that shrank or vanished
- Kept last saved version (safety): home/AUH/CloneEngine — lost 174 of 175 files; home/.codex/skills/auh-code-animation — folder missing; home/.codex/skills/auh-local-decisions — folder missing; home/.codex/skills/memoir — folder missing
- Missing folders: /Users/Mungura/.codex/skills/auh-code-animation; /Users/Mungura/.codex/skills/auh-local-decisions; /Users/Mungura/.codex/skills/memoir
- Status: blocked — needs an agent to look

---

## 2026-11-19 18:35 EAT — MUNGURA — Close-out before the build: everything saved, every agent armed

**Changed.** Harness: Hermes (deepseek-flash). Brief now 25 sections / 91,330 words with two new sections: 23 the mental models (Kallaway depth + systems, Dalio consequences, Naval status/wealth, Lauren Tan deterministic foundations, the creator mistake, laziness, Wang perception, boldness/brains, Ambi's canon) and 24 Links (28 distinct reference videos, 26 channels, 102 outliers, 34 teacher videos, Psyop post, playlists, repo). The converter now linkifies bare URLs — 262 live links, 0 before. Section 16 completed to the Part-4 shape: 1.2's 25 Who's-winning cards, an index by channel, a builder's guide, and seven edit flags (store says 12 channels, cards come from 14; strength = log10(perSub+1)/2 where perSub runs 0.2–106.9; 10 of 25 have no shape; all from the refused niche; 1–66 min runtimes).
**Also.** Claude Code given all 27 upstream skills (156 total in ~/.claude/skills) and a current-project block in ~/.claude/CLAUDE.md pointing at the brief, library, glossary, repo and ~/AUH/AMBESSA/BUILD/BUILD-BRIEF.md. Repo commits: context-repo c131b59 → 07-start-here; BOARD 5429a10; Loop c055d37 (107 files) and the auh-git backup 7854ec4354, "unsaved changes: none". Stale index.lock from 28 Oct removed.
**Why-verdict.** Everything he named is saved and pointed at: brief, gallery, glossary, repo, Loop, BOARD, profiles (69 skill dirs each), Hex 3.4.0 listening, T3 Code installed, Claude Code armed. AAY is zero-occurrence across the project; the govcon frame is archived and named closed in every handoff file.
**Status/open.** 220 untracked files in ~/AUH/Loop are media and job output (12 GB) — deliberately not committed; seven files hold live keys and are excluded by the backup script. The build itself starts in two days on the new model's tokens.
**Related.** `~/AUH/AMBESSA/intel/THE-SOFTWARE-BRIEF.html`, `~/AUH/AMBESSA/BUILD/BUILD-BRIEF.md`, `~/AUH/AMBESSA/GLOSSARY.md`, `~/.claude/CLAUDE.md`, `~/debate-agent/memory/vault/10 Projects/`.

## 2026-11-20

> Message-level context for this day. Auto-logged.

---

## 2026-11-20 00:10 EAT — MUNGURA — Daily journal generated for 2026-11-19; status=success; db_length=19357; source_hash=4c8c1cdf47a7.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-19; status=success; db_length=19357; source_hash=4c8c1cdf47a7.

---

### [00:10] Exchange: Daily journal worker run for 2026-11-19

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `scheduler` mode.

**Actions:**
- Target date: `2026-11-19`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-19.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-19.md`.
- DB row length: `19357`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-19.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-19.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-19.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db.
**Journal Dates Repaired:** 2026-11-19.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `scheduler`.
**Verification Results:** files written, SUMMARY mirror written, DB length=19357, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-20 00:27 EAT — MUNGURA — Daily journal generated for 2026-11-19; status=success; db_length=19399; source_hash=619534c76e33.
<!-- type: event -->
**From:** MUNGURA

Daily journal generated for 2026-11-19; status=success; db_length=19399; source_hash=619534c76e33.

---

### [00:27] Exchange: Daily journal worker run for 2026-11-19

**From:** MUNGURA
**Context:** Permanent daily journal worker executed in `scheduler` mode.

**Actions:**
- Target date: `2026-11-19`.
- Result status: `success`.
- Daily path: `/Users/Mungura/debate-agent/memory/daily/2026-11-19.md`.
- SUMMARY path: `/Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-19.md`.
- DB row length: `19399`.
- Status pointer: `/Users/Mungura/debate-agent/memory/daily/journal-status.json`.

**Files Changed:** /Users/Mungura/debate-agent/memory/daily/2026-11-19.md, /Users/Mungura/debate-agent/memory/daily/SUMMARY-2026-11-19.md, /Users/Mungura/debate-agent/memory/daily/evidence-digests/2026-11-19.json, /Users/Mungura/debate-agent/memory/daily/journal-status.json, /Users/Mungura/debate-agent/memory/memory.db, /Users/Mungura/debate-agent/memory/daily/_backups/2026-11-19.md.pre-sonnet5-repair-20261120_002046.bak, /Users/Mungura/debate-agent/memory/daily/_backups/SUMMARY-2026-11-19.md.pre-sonnet5-repair-20261120_002046.bak.
**Journal Dates Repaired:** 2026-11-19.
**Scheduler Touched:** status pointer only.
**Routes Touched:** dashboard API log attempted; status route verification handled separately.
**Tests Run:** `scheduler`.
**Verification Results:** files written, SUMMARY mirror written, DB length=19399, api_log_status=200.
**Failures:** none.
**Next Action:** verify dashboard routes and scheduler persistence.

**Status:** complete.
**Tags:** [memory, daily-journal, scheduler]

## 2026-11-24

> Message-level context for this day. Auto-logged.

---

## 2026-11-24 06:40 EAT — MUNGURA — Juju master brief received: saved, checked against the Mac, screens read
<!-- type: event -->
**From:** MUNGURA

Juju master brief received: saved, checked against the Mac, screens read
- Harness: Claude Code (claude-fable-5-2)
- What happened: Changed: Ambi pasted the Juju master brief (22 sections, 28,186 words) into T3 Code at 06:28. Saved byte-identical to ~/AUH/AMBESSA/intel/juju/JUJU-MASTER-BRIEF.md (sha256 8b8cdfc1…). Ran the boot it asks for, minus the steps that need his word. (1) Vendor docs: 19 of 19 saved to ~/AUH/AMBESSA/docs/stack-txt (the brief's harvester used bash 4 arrays; macOS has bash 3.2, so it was rewritten). (2) VidRush V2 walkthrough DlB0UABEawo: 1080p, 01:25 on, two ffmpeg passes, 639 frames on disk, 195 distinct screens with timed transcript. (3) Haiku 5.5 readers, one bounded unit each: 85 VidRush screenshots + the long homepage in 18 slices + 39 look references + 195 video screens, one JSON per unit in ~/AUH/AMBESSA/intel/juju/harvest/wave1/out, indexed in INDEX.json. (4) Juju added to the project map (find "Juju" now answers); topic = loop, where the software's history sits.

Why/verdict: the brief is the first record of the name Juju on this Mac. No day log exists for 21 to 23 Nov and Memoir had zero hits, so its "said by Ambi 20 to 22 Nov" lines cannot be checked here; the paste itself is taken as his word for the name and the folder. Observations where the brief and the disk disagree: the Rust engines are at ~/AUH/Loop/loop/engine (47 files, 9,791 lines, confirmed), not ~/AUH/Loop/engine. The look folder holds 39 pictures, about 35 of them Hades II; no Thumbsy screen, no YouTube feed tester screens. Missing on this Mac: rustup, Android SDK/NDK, adb, Tauri, Typst, bun, wrangler, turso; disk 95% full (51 GB free). The brief puts LOT on Inworld TTS-2; Ambi's 1 Nov voice lock is ABV V9 on inworld-tts-1.5-max, 0.95, temperature 2.0. LOT has not uploaded since 2 Nov; lot-r01 (25.3 min script, voice about $0.46) was never voiced or rendered.

Status/open: NOT done, waiting on Ambi: reading .env files to reuse keys (standing hard line), opening accounts and any payment, publishing the brief to the public ambessa-context repo (it carries his rent, debt and Mumu's details), installing Impeccable/Doop into the shared skill folders, the Android kit. No Juju code exists yet. Deadline named in the brief: first LOT film Wed 25 Nov 20:00 EAT.

Related: brief sections 15 to 18 and 22; ~/AUH/Loop/loop/onefile/START-HERE.md; ~/AUH/AMBESSA/BUILD/BUILD-BRIEF.md (19 Nov handoff, before the name). Harness: Claude Code in T3 Code, Fable 5.2.
- Files changed: ~/AUH/AMBESSA/intel/juju/JUJU-MASTER-BRIEF.md; ~/AUH/AMBESSA/intel/juju/scripts/stack-txt-harvester.sh; ~/AUH/AMBESSA/intel/juju/scripts/vidrush-v2-frame-rip.sh; ~/AUH/AMBESSA/intel/juju/scripts/dedupe_frames.py; ~/AUH/AMBESSA/intel/juju/scripts/harvest-index.py; ~/AUH/AMBESSA/intel/juju/harvest/wave1/INDEX.json; ~/AUH/AMBESSA/docs/stack-txt/; ~/debate-agent/memory/vault/project-maps.json
- Verification: cp checksum matched; harvester printed saved 19 failed 0; frames.json lists 639 files and 195 distinct screens; harvest-index.py printed 0 failed records; one reader record compared by eye against its screenshot (home composer, 13-18-32) and matched word for word; map-check shows no juju failure (2 older failures: memoir skill not found).
- Status: in-progress: boot audit and screen reading done; five decisions are Ambi's before the build starts

---

## 2026-11-24 06:41 EAT — MUNGURA — Juju brief read, 336 screens indexed, 19 vendor docs saved; waiting on Ambi's 5 calls
<!-- type: event -->
**From:** MUNGURA

Juju brief read, 336 screens indexed, 19 vendor docs saved; waiting on Ambi's 5 calls
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi pasted the Juju master brief. It is saved whole, and its claims were checked against this Mac. Juju is now registered in the shared project map.
- Harvest done: 19 of 19 vendor docs saved; 336 VidRush and look-reference screens read with 0 failures, including 195 from the V2 walkthrough video.
- Mac disagrees with the brief: no Juju memory or day log for 21-23 Nov; look folder has about 35 Hades II pictures, not the Thumbsy or feed screens; no Android kit; disk 95% full (51 GB free).
- LOT has not uploaded since 2 Nov, and a 25-minute script has sat unvoiced since 10 Nov. Proposed Wednesday 20:00 target: one LOT film from one command, with thumbnail and publish text.
- Cost $0 on paid services, about 2.2M tokens on 38 small reader agents. No Juju code built yet. Open: Ambi must reply 'defaults' or change the 5 calls before building starts.
- Files changed: /Users/Mungura/AUH/AMBESSA/intel/juju/JUJU-MASTER-BRIEF.md; /Users/Mungura/AUH/AMBESSA/intel/juju/harvest/wave1/INDEX.json; /Users/Mungura/AUH/AMBESSA/intel/juju/harvest/wave1/V2VIDEO-READER-BRIEF.md; /Users/Mungura/AUH/AMBESSA/intel/juju/scripts/harvest-index.py; /Users/Mungura/AUH/AMBESSA/intel/juju/scripts/stack-txt-harvester.sh; /Users/Mungura/AUH/AMBESSA/intel/juju/scripts/dedupe_frames.py; /Users/Mungura/debate-agent/memory/vault/project-maps.json
- Status: in-progress — research and intake complete, no Juju code built, awaiting Ambi's reply on the 5 calls

---
