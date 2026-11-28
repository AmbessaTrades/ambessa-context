# Every sheet, newest first

The last 84 two-hour sheets. Older ones are in the git history of this file.

---

# Sheet of 16:44 EAT, Sat 28 Nov 2026

## Changed since the last sheet
- Covers 22:39 Thu 26 Nov to 16:44 Sat 28 Nov EAT.
- Main: last commit 13ff4192 (15:50, 0.4.4). Two commits since the last sheet: 1f04d013 (15:45, 0.4.3) and 13ff4192 (15:50, 0.4.4). Rust: 37,598 lines (was 37,524). Decisions: 29 (was 27).
- Juju 0.4.3 and 0.4.4 shipped to the phone, web and Mac (lead, 15:52). Checked by hand only.
- Pull requests unchanged: 8 open, 19 merged, 1 closed. PR 28 still has a failing check.
- Money ledger unchanged: 10,632 calls, $36.11 in all.
- Worker's read-only audit of Juju finished at 16:11. No Juju code changed and no paid call made by the audit.
- ADR 0030 and ADR 0031 and a plan were written at 16:30. The worker says Ambi's answers are recorded there. ADR 0030 says the phone engine becomes the only engine and the Mac runs it too. This replaces the 16:14 "park the phone engine" answer.
- At 16:40 the worker reports Ambi's order: the lead decides two questions alone, no limits on the phone's looks, no more markdown files, show the whole app as a canvas. The Doop canvas started.
- Corrections: the lead's 15:38 Google and Inworld 7-day spend ($8.39, $3.80) became $9.28 and $3.92 at 15:52. The old "1% left" Claude reading became 99% left, resets 5 Dec (fresh reading, 15:45).

## What worked and what failed
**Worked (checked by hand, no automatic test)**
- Gris-gris sheet names its roles: DeepSeek writes, GLM 5.3 checks, Neon plans (lead, 15:52).
- Mojo Bag shows quota cards with % bars, 7-day spend, and Read again refreshes every card (lead, 15:52).
- Each channel card has Ideas, films, Settings or Finish, and the bin on one line at phone width (live web).
- Absorb inside a channel fills that channel. Two channels stay two (live web, 15:52).
- The Mac shows all three channels from the Door: Spiral5D, GEOTORYX, spiral 5d (lead, 15:48).

**Failed or refused**
- Absorb pays, then drops the answer. The phone waits 90 seconds. The Door waits 600 seconds and charges, nothing is saved, and each retry pays again. The worker is about 75% sure of this cause. Not fixed in 0.4.4.
- The phone's idea screen deals states cards, but the phone's film engine draws kingdoms and wealth only. The audit says a states idea was refused after a 600 MB download. Not fixed.
- Ideas are weak by construction: every kingdoms title follows one template, and two channels can get identical ideas (audit).
- Ambi refused "Deep Time" as "ugly". It is parked.
- Ambi said "forget Neon if expensive". The learn route still uses gemini-4-neon. Not reconciled.
- The worker says 13 releases (0.3.0 to 0.4.2) went out on 26 Nov with no button pressed.

## App engine and films
- Phone engine: kingdoms and wealth only. Film kinds are built twice, once for the Mac and once for the phone (audit).
- Films finished: about 2 from roughly 27 presses on the Mac. None on a real phone on record (audit).
- Film runs on disk: 4 DONE, 4 FAILED, 24 HOLD. Unchanged.
- Decided, not built:
  - Every look runs on every device, including the 3D globe on the phone. The method is picked by a race on the phone (Ambi refused limits).
  - Each thinking step (idea, bend, title, outline, script, storyboard, check) becomes a card: fixed text, required answer shape, code checks (ADR 0031).
  - Variety: code refuses an idea that repeats too much of the last five films.
  - Three formats first: "Does your state have this?", "Bigger than you think", "Why this one is the most X". Voice is a switch per channel.
  - Every film gets a free code-fault repair loop, up to 2 rounds, on the cheap model.
  - High Juju also checks its 240p take with Claude and fixes it up to 2 rounds, capped at $0.50 per film (lead, Ambi's order).

## Web app and rooms
- Web is at 0.4.4 (lead, 15:52).
- Proposed, not built: three places (Today, Make, Channel) and a command bar. Cmd-K on the Mac, + on the phone. Film as a thread with status. Review by story first. Settings hidden until set.
- Blueprint: one flow file would draw the canvas and drive a test that presses every arrow. The old flow files hold 22 files and 218 arrows, and they have drifted from the built rooms (16:40).
- Doop canvas is running. Paper's connector needs Paper.app open.
- The 19 themed rooms still stand.

## Mac app and APK
- Mac app: 0.4.4, restarted (lead, 15:52).
- Every 30 minutes the Mac signs in to the Door, deletes channels deleted elsewhere, pulls Door channels it lacks, merges its rows, and pushes its week.
- The Mac reads Claude's week at most every 2 hours.
- Mac 7-day spend (Door purse, 15:52): Google (Neon, Choice of the Seer) $9.28; Inworld (Voice of the Elders) $3.92. Inworld and Google give no balance, only spend.
- Phone: 0.4.4 live (lead, 15:52). One APK file is built.
- Phone on a real device: not tested. No test has pressed the phone or web build (audit).

## Agents running now
- The live agent page did not answer, so running agents are unknown.
- Lead: last message 15:52 Sat (0.4.4 shipped).
- Worker: last message 16:40 Sat. Waiting on three answers before building the canvas. Its 11 audit agents finished by 16:07.
- Transcripts written in the last 10 minutes: 0.
- Mac load (1, 5, 15 min): 3, 3, 3.

## Money spent on services
- Ledger: 10,632 calls, $36.11 in all. DeepSeek 11.11, OpenRouter 12.27, Google 8.39, Inworld 3.92, unsettled 0.14, WaveSpeed 0.29.
- Door spend for 27 and 28 Nov is not in the ledger (audit).
- Caps conflict: the last sheet named a $35 cap, passed, with no ruling. The audit names a 10 US ceiling. No ruling from Ambi.
- Claude is not a ledger line.

## Broken, blocked or open
- Absorb charge and states refusal: both not fixed.
- Ideas: template titles, identical ideas, and the 59 skills do not reach a model in the film path (audit).
- No automatic test has pressed the real phone or web build. The worker says GitHub has refused automatic checks since 25 Nov because the account is at its limit. Autosave pushes to main (audit).
- PR 28 has a failing check.
- Decided, not built: no shipping to a phone until a robot presses every arrow green (about 3 minutes).
- Not proven: a voiced film over 10 minutes; a film on 0.4.4; the 95 of 100 taste bar; a cheap model fills recipes at 95% legal first answers; anything on a real phone.

## Waiting on Ambi
1. Name her channel and the phone model. This blocks the first proof and the build.
2. Doop or Paper.app for the canvas. Doop is running now.
3. Yes or change: three places (Today, Make, Channel) with a command bar.
4. Remove the extra Spiral channel. Tap its bin, type DELETE, tap Delete.
5. Your one click: GitHub billing, to restore automatic checks.
6. Rule on the cap: $35, or the audit's 10 US.
7. Rule on "forget Neon if expensive" against the learn route.
8. Plug in a real phone. No real-device test is on record.

# Sheet of 22:39 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 20:08 to 22:39 EAT, Thu 26 Nov 2026. Facts as of 22:39.
- Main: last commit 446e356e (21:35, 0.4.2). Five commits since 20:08.
- Phone: 0.3.8 and 0.3.9 (20:33, engine c1f4591c), then 0.4.0 (21:10), 0.4.1 (21:25), 0.4.2 (21:39). Current phone build: 0.4.2.
- Web: 0.4.2 live at 21:39.
- Mac app: 0.4.2, restarted 21:39.
- Door: 410c250a (20:33), 5ca8b342 with the learn route (21:10), 0ff5cb31 with the export chain (21:39). Door tests 63 of 63 pass at 21:39.
- Money ledger: 10,632 calls, $36.11 in all. Up about one cent since 20:08.
- Pull requests: 8 open, 19 merged, 1 closed (unchanged). PR 28, "High Juju: two modes", is open with a failing check.
- Rust: 37,524 lines (was 37,404).
- Film runs on disk: 4 DONE, 4 FAILED, 24 HOLD (unchanged). The worker reports an 11-minute test film, zz-len11, held at room 4. It is not in the disk count.

## What worked and what failed
**Worked (as reported)**
- Length: 11 minutes asked gave 44 stops and a 9.4-minute film (worker, 20:40; TEHUTI, 20:33). Mac build only, held (see below).
- Confirm sheet before a film shows length, time, money and first download. Checked on the live web at phone size (TEHUTI, 20:33).
- Gris-gris and High Juju switch works on the live web (TEHUTI, 20:08).
- Learn from a film: Door watch of Ambi's USA maps link. 55 s, $0.20, 19 shots, 10 rules, 6 topics (worker, 21:10). In a test space, link to lesson to rules on the channel ran end to end.
- Absorb: the same handle twice opens the first channel; a video link is redirected; a bad link is refused (live web, 21:25).
- Delete a channel: 422 without the word DELETE, 200 with it (live web, 21:25).
- Upload chain: DeepSeek's real step-90 idea was "Does Your Province Have These? (15 Maps)" (worker, 21:39).
- Live sweep: nine GET routes answered; five rooms load with no script errors. Mac: nine routes answer 200 while signed in (worker, 21:38).

**Failed or refused**
- The 11-minute test was held at room 4. Twenty coloured countries had no name, and Russia and Australia shake a few pixels between frames (worker, 20:40). The last three short money films (14 stops each) were held the same way, so the fault is older than today.
- Phone films are not held by room 4, because the check is not built on the phone.
- Ambi (17:40, as quoted by the lead): "we're here to fix juju, not ... the specific video."
- Ambi refused Deep Time ("ugly") and said "forget Neon if expensive" (last sheet). Parked. The learn route uses gemini-4-neon (21:10). This is not reconciled.
- Five test runs locked Ambi's PIN for 15 minutes (19:39). The Door no longer signs in as him in tests.

## App engine and films
- juju-core and timemap.py take the film length. Each stop is 13 seconds. Stops are no longer capped at 18.
- The steer line reaches every words call (TEHUTI, 20:33).
- Learned rules go into every words call as "STYLE TO FOLLOW" (TEHUTI, 21:10). No phone film has used them yet.
- Room 4 fix (proposed by the worker): give every coloured country its name, and stop names shaking. It goes in the shared map code, so Mac and phone both get it. The worker estimates 1 to 2 hours plus a test film. Not started. It waits on Ambi's reply.
- Export 720p or 1080p redraws the film at the new size and reuses the paid script and voice (worker, 21:39). Not run on a real phone.
- The Mac sends its Claude plan reading to the Door (21:22). The last reading seen was 1% left (19:39).
- High Juju sends writing and storyboard roles to Claude Opus 5.5 (last sheet). No real film on the phone has used it.
- The debt film has not been redrawn on the fixed code. Ambi's rehearsal showed Jordan, Sudan and Congo for "biggest economies" (fixed in code, not drawn).

## Web app and rooms
- Live at 0.4.2. Five rooms load clean: Altar, New Vessel, Crossroads, Cauldron, Shelf.
- New since 20:08: the DELETE sheet on every channel card; absorb studies the best film; Learn from a film; the upload kit opens (it said "Not built yet"); "Uploaded? paste the link" in Cauldron and Shelf; Crossroads marks chain ideas "Follows your hit · 90%"; export buttons in the Cauldron.
- Still wrong: five High Juju looks (Duppy Day, City Towers, Contagion Pulse, Crude Ledger, Engraved Atlas) have no films or colours (19:39).
- Mend (fix a film) answers only on the Mac.
- Rooms missing since the last sheet, not re-reported: Bend, Fill the week, the composer, Conjuring receipt.

## Mac app and APK
- Mac app: 0.4.2. Signs in to the Door with its own key, learns from films through it, sends the Claude plan reading, and reports its version (21:22).
- Phone: 0.4.2 released (21:39). Only one APK file is on disk (FACTS).
- Phone on a real device: not tested. The one emulator run used earlier builds.
- DMG for the Mac: still next time (19:28).

## Agents running now
- Worker (TEHUTI): last message 21:39 (0.4.2 shipped). Session end logged 22:18.
- Lead: last message 18:05 (credits ran out).
- Agent transcripts written in the last 10 minutes: 0.
- The live agent page did not answer, so running agents are unknown.
- Mac load (1, 5, 15 min): 14, 15, 17.

## Money spent on services
- Ledger at 22:39: 10,632 calls, $36.11 in all. DeepSeek 11.11, OpenRouter 12.27, Google 8.39, Inworld 3.92, unsettled 0.14, WaveSpeed 0.29.
- The $35 cap was passed at the last sheet. No ruling since.
- Door cap: 5 US (lead, 15:04). No change reported.
- Learn from a film: $0.20 for the USA lesson, and about 3 cents for the first test watch (worker, 20:58). The Gemini watch is not in the ledger figures above; Google stays at $8.39.
- Claude API: one count_tokens check per hour, free. One real Opus call under 1 cent (19:39). Claude is not a ledger line.

## Broken, blocked or open
- Room 4 label fix: not started.
- Five High Juju looks: no colours or films (last report 19:39).
- juju-core high_on does not read lean.api (20:08).
- Not run: export on a real phone; the upload chain on a real upload; a phone film using learned rules; the learn route on Ambi's own account.
- Phone: no real-device test; first sign-in on a physical phone not checked.
- Door sync needs Ambi's Gate sign-in. Not done.
- PR 28 has a failing check.
- Not proven: a voiced film over 10 minutes; a film on 0.4.2; the 95 of 100 taste bar; that a cheap model fills recipes at 95% legal first answers.

## Waiting on Ambi
1. Reply "go labels" to start the room 4 label fix (worker, 20:40).
2. Install 0.4.2. Open a finished film in the Cauldron, tap 720p, and check the phone's Movies folder when it says done (worker, 21:39).
3. On the phone, paste the USA maps link under Learn from a film and wait for "Learned 10 rules" (worker, 21:10).
4. Remove the two extra channels added by accident: tap the bin, type DELETE, tap Delete (worker, 21:25).
5. Say whether the $35 cap still holds.
6. Rule on "forget Neon if expensive" against the learn route, which uses gemini-4-neon.
7. Say whether to build colours and films for the five High Juju looks now.
8. Plug in a real Galaxy. Phone tests have run on an emulator only.
9. Rule on night on two grounds: parked, no ruling.


# Sheet of 20:08 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 18:05 to 20:08 EAT, Thu 26 Nov 2026. Facts as of 20:08.
- Main at 20:08: last commit 80576db9 (0.3.7, Door-side). Newest Door fix: 5279daf3, deployed f9d2f502 (Gris-gris / High Juju sheet). The lead's 18:05 wind-down holds for agents, which have all stopped.
- Phone 0.3.0 and 0.3.1 released (18:25). Phone 0.3.3 released (18:41). Phone 0.3.4 released, then 0.3.5 to 0.3.7 (19:05 to 19:39). Current phone build: 0.3.7, engine eca22dec.
- Door: live at 19:39 (bc317ecc), then f9d2f502 at 20:08. Door tests 55 of 55 pass (lead's last check, 20:08).
- The Door no longer signs in as Ambi in tests. Five repeated test runs had locked his PIN for 15 minutes (worker, 19:39).
- Cloudflare sign-in: failed at 18:58 to 19:05, then restored at 19:19. Door redeployed.
- Money ledger: 10,626 calls, $36.10 at the last sheet. No newer ledger fact.
- Pull requests: 8 open, 19 merged, 1 closed (unchanged in FACTS). Newest merged: none reported after 17:54.
- Rust: 37,404 lines (unchanged). Rooms drawn 22, skills 59, decisions 27, APK files 1 (last sheet's FACTS; not re-read).
- Film runs on disk: 4 DONE, 4 FAILED, 24 HOLD (unchanged). No new `juju make` run reported.

## What worked and what failed
**Worked (as reported)**
- Web channel paste (worker, 19:28): pasting @RealLifeLore created the channel. Tested at 390x844 on a test space.
- Look pictures on web and phone (worker, 19:28): 10 look pictures load at 200, 480 px. Five looks still dark (see below).
- Web install with Juju cat icon (worker, 19:28): manifest 200, 192/512 and apple-touch icons present. APK already had the cat icon (checked res pngs).
- Mojo Bag shows every service (worker, 19:05, 19:39): Google and Inworld show this week's spend. Claude row shows "API open · $X used this week".
- Gris-gris / High Juju switch (worker, 20:08): pressed live at 390x844 on a test space. Chip changes, reason shows when API is off. Door test 55 of 55.
- Claude API call (worker, 19:33, 19:39): key returns 200 on count_tokens. One real Opus 5.5 call with the Door body answered. Well under 1 cent.
- juju-core money route (lead, 18:05): on saved answers only, plan file and 5 frames match the Mac. Golden SAME vs Mac on the debt film (lead, 18:05; worker 19:39 at eca22dec).
- Phone emulator (worker, 18:53, Mac unreachable): a 3 min 35 s wealth film made by the phone in 11.4 min. No crash lines. A later build (lead, 17:41) gave 215 s and -14.4 LUFS. Both reports are from earlier builds.

**Failed or refused**
- Ambi (17:40, as quoted by the lead): "we're here to fix juju, not ... the specific video."
- Ambi: the debt rehearsal showed Jordan, Sudan and Congo for "biggest economies". Fixed in code; the debt film has not been drawn on the fixed code to show it.
- Ambi refused Deep Time ("ugly") and said "forget Neon if expensive". Parked and stopped (last sheet).
- Sign-in: Ambi's PIN was asked twice and rejected (18:34 report). Fixed: one entry, then PIN only. Real-phone first sign-in not checked.
- Web channel paste failed at 0.3.5 (19:19): the code sat in the edit handler. Fixed in 0.3.6.
- Mojo Bag "Not reported" rows and "not on the web/phone yet" text. Removed in 0.3.4 to 0.3.7.
- Gris-gris switch printed "Gris-gris. null." and no button worked (worker, 20:05). Fixed in the Door at 20:08 (Door 5279daf3).

## App engine and films
- juju-core (Rust) makes money films with no Python. Covers the G7, G20 and continent groups, five colour bands, legend, names on every land (at most 24 for rates), and the wealth check for any money set (lead, 18:05).
- Each country gets its own colour, no two neighbours alike. Names pinned and visible through the end card. Not proven on a drawn film.
- Name jumps fixed by one placement rule per country (lead, 18:32). The last held debt proof (zz-debt-r4, 18:10) held only for name jumps at 2.3 to 2.6 s. Not redrawn since.
- State films (income, GDP, taxes, pay by state, BEA, keyless) and pop-up number cards added (lead, 18:32; TEHUTI, 18:36). Sound effects raised. Sound test passes (agent report). None proven on a drawn film.
- Not ported to juju-core: kingdoms, series, corrections, states. Stops in plain words. The exit predicate is still false (lead, 17:16 and 18:05).
- Earlier engine reports: the Mac chain has moved past the frozen copy (lead, 17:16). The corrections file is not in any pack (lead, 18:05).
- High Juju (phone and web): routes the writing and storyboard roles to Claude Opus 5.5 at medium effort, with caching (worker, 19:39). Covered roles per juju-core eca22dec: package, insight, ladder, direct, one, table, think, film mind, storyboard, birth pick. Not run on a real film on the phone.
- Plan path (Claude subscription) still needs the Mac. The plan had 1% left (worker, 19:39); the Mac read 3% about 90 minutes earlier (worker, 19:30).
- Money films route to the money style. Debt, tax and inflation films pass rooms 1 to 3 (lead, 18:05).

## Web app and rooms
- Web app: live at https://ambessatrades.github.io/juju-web/. Channel paste works (19:28). Gate sign-in fixed (18:34 and 0.3.1 release).
- Gate: one PIN entry for a first PIN; setup code typed first (lead, 18:33 commit 1b224ff3). Ambi could not sign in on 26 Nov (commit message).
- New Vessel: the + jar opens Absorb with the link box focused (commit 575ef820). A look with no film shows its own land and sea colours (commit f3ccecf3, 19:19). Five High Juju looks (Duppy Day, City Towers, Contagion Pulse, Crude Ledger, Engraved Atlas) still have no films or colours and stay dark (worker, 19:28, 19:39).
- Web installs as its own app ("Install app" or "Add to Home Screen").
- Rooms still missing: Bend, Fill the week, the composer, Conjuring receipt (last sheet). Full control census (24 Nov): 573 controls, 112 real. Not re-run.
- Door sync needs Ambi to sign in once at the Gate with his PIN. Not passed in any message.

## Mac app and APK
- Mac app (local server, port 4700): slider 10 to 30 minutes (default 11), held films playable with reason and never kept, Mojo Bag, upload kit (lead, 18:05). Mac version line and its update route are not built (lead, 18:07).
- Mac posting Claude % to the Door: not built. The Door reads Claude from the API key now (worker, 19:31).
- Phone: 0.3.7 live (19:39, APK bb322ec7). Previous: 0.3.6 (19:28, APK ee6e47ea), 0.3.5 (not in FACTS), 0.3.4 (19:05, APK 0e1b48b9), 0.3.3 (18:41, APK 8a7720ef), 0.3.1 (18:25, APK c5bfd716). Release key in ~/.config/juju; Ambi keeps a private copy (lead, 18:25).
- Phone screens stay bundled in the app; a bad web push must not break phones (TEHUTI, 18:53).
- Phone 0.3.0: built and signed, not released (round cut at map download, 18:05). Superseded by 0.3.1 and later releases.
- Phone on real device: not tested. The one emulator test ran on earlier builds (lead, 17:41; worker 18:53).
- First film on phone downloads about 600 MB of maps (lead, 17:41). Re-download fix in 0.3.0 (worker, 18:53); not proven since.
- Only money films draw through juju-core on the phone. Other kinds not ported.
- DMG for Mac: next time (worker, 19:28).

## Agents running now
- All workers and leads have stopped. Last message for each: lead 18:05 (credits ran out); phone worker 19:39 (0.3.7 released, stopped); Door worker 20:08 (Gris-gris fix, stopped).
- Live agent page not checked in these messages. Running agents are known only from messages.

## Money spent on services
- Ledger at the last sheet (18:05): 10,626 calls, $36.10 in all. DeepSeek $11.10, OpenRouter $12.27, Google $8.39, Inworld $3.92, WaveSpeed $0.29, unsettled $0.14.
- The $35 cap noted in the last sheet is passed. No message says whether the cap still stands.
- Door cap: 5 US (set by the lead at 15:04). No change reported.
- Claude API key: added to the Door at 19:19. Opus 5.5 at medium effort, priced per call; one count_tokens check per hour (free); one real call under 1 cent (worker, 19:39).
- Google and Inworld: no balance API. The bag shows week spend instead (worker, 19:39).
- Per call: route and place about 0.0001 US; ideas for five cards 0.00124 US; music tags 0.00105 US for three shelves (last sheet).

## Broken, blocked or open
- Five High Juju looks (Duppy Day, City Towers, Contagion Pulse, Crude Ledger, Engraved Atlas) have no films or colours. Fix about 10 minutes; not built (worker, 19:28).
- A real High Juju film on the phone has not run (worker, 19:39).
- juju-core high_on does not read lean.api. Only matters if the Mac's plan reading is fresh and the API is leaned off (worker, 20:08).
- Debt film redraw: name jumps fixed in code; zz-debt-r4 held at room 4 for name jumps at 2.3 to 2.6 s (lead, 18:10). The fixed code has not been redrawn.
- Phone 0.3.0 not released; superseded. Two-film proof on a signed build not finished.
- Mac version line and its update route: not built (lead, 18:07).
- juju-core: wasm and WebCodecs parts not built. Workspace check fails in apps/juju-shell (Tauri macro), not in this lane.
- Five films graded by the hand-kept list: no change.
- Night on two grounds: parked (last sheet).
- Not proven: a voiced film over 10 minutes; any phone build on a real phone; the 95 of 100 taste bar; that a cheap model fills recipes at 95% legal first answers; a full film on the 0.3.7 build; a debt film on the fixed code.
- Door sync needs the Gate PIN sign-in, which is not done.

## Waiting on Ambi
1. Say whether the $35 cap still holds. The ledger was $36.10 at 18:05. The Door cap is 5 US.
2. Install 0.3.7 on the phone and check the Juju cat. Tap Read again in the Mojo Bag and check the High Juju row says "API open".
3. On the phone: tap Gris-gris, then High Juju. The chip should change. If it says "null", close the app and open it again.
4. Sign in once at the Gate with your PIN, for Door sync. Needs the setup code.
5. Listen to the music picks for money-map, trade-road and war-table, and say whether they fit (last sheet; not re-reported).
6. Plug in a real Galaxy. Phone tests have run on an emulator only.
7. Approve or change the outlier and flop cut-offs (last sheet; not re-reported).
8. Night on two grounds: parked, no ruling yet.
9. Five High Juju looks: say whether to build colours and films for them now.



# Sheet of 18:05 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 15:57 to 18:05 EAT, Thu 26 Nov 2026. Facts as of 18:05.
- Ambi said "no more films" (lane log, 17:28). Agents stop making videos and filming is left to the app. No film is queued.
- Agent work stopped at about 18:05 when the credits ran out. The lead says merge and stop. Every worker reports stopped.
- Ledger: 10,626 calls, $36.10 in all (was $35.80). That is above the $35 cap the last sheet noted. No message says whether that cap still stands.
- Main moved: 15 commits from 15:26 to 17:54. Newest: one length slider, 10 to 30 minutes, default 11. A held film plays with its reason and is never kept.
- Pull requests: 8 open, 19 merged, 1 closed. #26 and #28 show failing checks. CI is blocked by billing, so checks run locally (lead, 15:57).
- Rust: 37,404 lines (was 37,007). Rooms drawn 22, skills 59, decisions 27, APK files 1: unchanged.
- Attempts logged: 433 kept (was 427), 63 reverted, 52 inconclusive.
- Finish check: 1 of 23 clauses true (not read at 15:57).
- Whole-film runs on disk: 4 DONE, 4 FAILED, 24 HOLD, unchanged. Films made in the app and in lane tests are not in that count.
- Mac load: 51, 60, 50 (was 95, 89, 86).

## What worked and what failed
**Worked (as reported)**
- Phone (lane B, 17:41): on the Android emulator with all Mac ports blocked, a 215-second money film was drawn by juju-core in 11.4 minutes. It measured -14.4 LUFS, played from the shelf, and had 0 fatal errors. Not tested on a real phone.
- juju-core (lane A, 17:16): builds green on Mac (Metal and CPU-only), Android and wasm. 18 and 7 unit tests pass. A build from the 35 packs alone gives frames identical to the Mac (0 of 255 values differ).
- Fresh-person walk to Shelf passes at phone and desktop sizes. No film drawn (lane, 17:23).
- Route: 21 test answers pass. Pulse: about 0.0009 US and 83 s for a full week.
- Parity: 40 features checked against the Mac, 0 missing (worker, 18:03).

**Failed or refused**
- Ambi: the debt rehearsal showed Jordan, Sudan and Congo for "biggest economies". The lead fixed it: a named group in the title now picks the countries.
- Ambi, 17:40, as quoted by the lead: "we're here to fix juju, not ... the specific video."
- The debt rehearsal was held at its final check (17:31). The largest-economies film looked good by eye (lead), but was held at room 4 for unnamed lands and name jitter. The fixes are built but not proven on a film.
- The 0.3.0 phone test was cut at film 1, while maps were downloading (18 of 44 MB). Not released.
- Ambi refused Deep Time ("ugly"). It is parked. He also said "forget Neon if expensive". Neon is stopped.

## App engine and films
- Ambi's rule (quoted by lead, 15:16): "our job is to allow the software juju to make any kinds videos... not to CHOOSE videos and topics for it. but to be adaptable."
- Money films route to a money style. Debt, tax and inflation films plan and pass rooms 1 to 3. Any money measure is fetched from the World Bank on request.
- Each country gets its own colour, no two neighbours alike. Names stay pinned and visible through the end card. Not proven on a film.
- juju-core (Rust): wealth films run from one sentence with no Python. Not ported: kingdoms, series, corrections. The "states" kind and the Canada sentence stop in plain words. The exit predicate is still false.
- Held films can be watched with their reason, never kept. "Again" (free redraw) is not proven.
- Music: Earshot picked tracks for money-map, trade-road and war-table. That is 3 of 16 regions. The War Room test re-mix measured -14.02 LUFS. Each film's music credit goes into its upload description. Ambi has not heard the picks.
- Mend: splices old and new design generations. "Use this one" stays hidden until takes are one generation.
- Africa 26.8-minute film: loudness not confirmed. Ambi has not heard it.
- Door has a YouTube key (worker, 18:05). No real Pulse run on it is reported.

## Web app and rooms
- The public web app was rebuilt with the new rooms and checked live at phone size in a test space (lane B, 17:41). The Gate, empty Altar, New Vessel, Crossroads and Mojo Bag are in. It cannot make films yet (worker, 18:05).
- Door sync needs Ambi to sign in once at the Gate with his PIN. Not passed.
- Idea cards show the style's sample picture, not one picture per idea.
- Not built: Bend, Fill the week, the composer, Conjuring receipt. Last full control census (24 Nov): 573 controls, 112 real. Not re-run.

## Mac app and APK
- Mac app (local server): length slider, held films, Mojo Bag with live balances, upload kit, empty Altar. Live since 17:22.
- Mac version line in the Mojo Bag is not built. The update route on the Mac server is not built.
- Phone 0.3.0: built and signed, kept on the Mac, not in git, not published. The test round was cut. One release script builds web and phone from one commit. The update sheet on both waits while a film is being made.
- Phone screens stay bundled in the app. Loading them from the web was refused (lead agreed).
- Phone: the ANR fix was made (lane B, 17:28), not re-tested. First film downloads about 600 MB.
- Only money films draw through juju-core on the phone. Other kinds are not ported.

## Agents running now
- The live agent page did not answer. Running agents are known only from messages. No transcript was written in the last 10 minutes.
- Lead: last message 18:05, stopped at credits.
- Phone lane and screens worker: stopped 18:05.
- Core lane: wound down 17:16.
- Route, place and music lane: stopped on Ambi's word, 17:28.
- App Polish: last message 17:22. Session not running.
- Door lane: last message 16:01 (last sheet).
- Worlds and Sound lanes: closed 17:28.
- The debt film redraw was still drawing at the stop. Its result is unread.

## Money spent on services
- Ledger: 10,626 calls, $36.10 in all, up $0.30 since 15:57 (156 more calls).
- DeepSeek $11.10 (6,531 ok, last ok 17:52). OpenRouter $12.27 (3,411 ok, last ok 16:38). Google $8.39 (119 ok, last 13:59). Inworld $3.92 (458 ok, last 10:54). WaveSpeed $0.29 (last 25 Nov). Unsettled $0.14 (9 failed).
- Door cap: 5 US, set by the lead at 15:04. Ambi has not named another.
- Per call: route and place about 0.0001 US. Ideas for five cards 0.00124 US. Music tags 0.00105 US for three shelves.
- YouTube: 102 units per niche; Door ceiling 9,000 units a day. No spend recorded.
- Agent credits ran out at about 18:05. No top-up reported.

## Broken, blocked or open
- Phone 0.3.0 is not released. Its two-film test must pass first. The map download was incomplete at the stop.
- Debt films: the colour, key and name fixes are not proven. Round four's result is unread.
- Mac version line and its update route are not built.
- juju-core: the workspace check fails in the app shell (a Tauri build step), not in this lane. Wasm and WebCodecs parts are not built.
- Night on two grounds is parked. The plain globe turns night lights beige at 1 degree; the plain look file must change. The seviller redraw failure is unexplained.
- Gold6 night film is missing. The canon check fails on it.
- Africa share figure: fix reported in flight at 15:50. No later report.
- Outlier and flop cut-offs (3 times and a quarter of a channel's average) are not approved.
- Not proven: a voiced film over 10 minutes; any phone build on a real phone; the 95 of 100 taste bar; that a cheap model fills recipes at 95% legal first answers; that the debt film passes room 4.
- Mac work was pushed to the private backup at 18:05 as a snapshot.

## Waiting on Ambi
1. Say whether the $35 cap still holds. The ledger is at $36.10. The Door cap is 5 US.
2. Sign in once at the Gate with your PIN, for Door sync. The sign-in needs the Door's setup code.
3. Listen to the music picks for money-map, trade-road and war-table, and say whether they fit.
4. Listen to the first 2 minutes of the 26.8-minute Africa film.
5. Say "check the debt film" when credits are back (worker's ask).
6. Plug in the Galaxy. Phone tests have run on an emulator only.
7. Approve or change the outlier and flop cut-offs.
8. Night on two grounds: parked, no ruling yet.
9. The no-tell-frames subtitle call. 18 canon faults wait on it.




# Sheet of 15:57 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 09:00 to 16:01 EAT, Thu 26 Nov 2026. Facts are as of 15:57.
- Ledger: 10,470 paid calls, $35.80 in all (was 10,145 calls, $34.33). That is above the $35 cap the last sheet recorded. No message says whether that cap still stands. The lead set a Door cap of 5 US at 15:04.
- Pull requests: 8 open (was 7), 19 merged, 1 closed. New open: #28 "High Juju". #26 and #28 show a failing check. CI is blocked by billing, so checks run locally (lead's log).
- Main moved for the first time since 11:13 on 25 Nov. 15 commits from 12:57 to 15:37 today.
- Rust: 37,007 lines in 15 crates (was 35,572). Rooms drawn: 22 (was 21). Skills: 59. Decisions: 27. APK files built: 1 (was 0).
- Attempts logged: 427 kept, 63 reverted, 52 inconclusive (was 391, 60, 52).
- Mac load at 15:57: 95, 89, 86 (was 26, 34, 45).
- Finish check: not read (was 1 of 23).
- Whole-film runs unchanged: 4 DONE, 4 FAILED, 24 HOLD. The films named in messages below are not in that list.
- Night on two grounds: round two done (09:23 to 10:35). The lead then parked it at 10:50 after its own change made the night lights worse. Round three was stopped before any spend.
- Door: built, deployed and set to live mode with five provider secrets (lead, 15:04). Paid calls stay refused until the two sign-in codes are set.
- Core: the drawer is now a library. Lane A reports identical frames to the Mac's (Measured, 14:20).
- Ambi's rule, quoted by the lead (15:16): "our job is to allow the software juju to make any kinds videos... not to CHOOSE videos and topics for it. but to be adaptable."
- Ambi called Deep Time "ugly" (14:47). It is parked.
- Neon A/B stopped on Ambi's word (14:06). About 0.24 US spent; cache 0 on 11 calls.
- The "60% of Africa ruled from outside" figure was a code fault, not a model fault (lead, 13:47). Fix in flight.
- Three afternoon mends regressed because new 4-second pieces were spliced into older takes (lead, 15:50). Fix in flight.

## What worked and what failed
**Worked (as reported)**
- Door live: test.mjs 32 of 32 on the live address (lane C, 15:04). The worker reports 38 of 38 with the pulse and video routes, run four times (16:01). Not checked by anyone else.
- Route and place: 21 test answers pass. Code answers cost 0.13 to 0.22 CPU s each (lane, 15:51, Measured).
- App walk: 38 of 38 clauses at phone and desktop sizes, 0 console errors (polish lane, 14:32, Measured).
- Mend on the Africa film drew with the film's own engine, 0.0125 US (worlds lane, 14:47).
- Sound: a camera bed sits within 3 LU of the music. Earshot picks 60% of cues against 21% by chance (sound lane, 14:46, Measured).
- Phone: the emulator made a 2-minute film with the Mac's ports blocked. It took 13.6 minutes (phone lane, 15:55). The drawing is a stand-in, not Juju's map design.

**Failed or refused**
- Night on two grounds, by the lead: round two spread 3 on the eye mark (was 5) and 1.1 on the program score (was 0.8). Beige glow on night lights rose from 4–45% to 8–61% of close frames. A clean redraw failed, and the cause is not found.
- Deep Time: Ambi, "ugly". Parked.
- Neon: Ambi, "forget Neon if expensive". Stopped.
- Gold6 night film: the file is missing from the save. The deleter is unknown. The canon check fails on it (lead, 13:37).
- The "Ambi correction" entry in the corrections log was fake and removed (lead, 15:28).
- Ambi, 15:20: "Why are you guys losing the plot... Why are you fumbling?" The lead rebuilt the app flow after this.
- Worlds: the Africa share figure, the Almoravids date and two Korean sign flips are refused by the engine lane.

## App engine and films
- `ju make` can now draw a film from a sentence. The last whole-film run list is unchanged.
- The Africa film at 26.8 minutes was redrawn on the new engine in 1,610 s. The sound is mixed. The loudness check did not finish. Ambi has not listened.
- `ju route` (which style draws a subject) and `ju place` (which sub-niche a channel is in) are built. Each uses code first and DeepSeek only when code cannot decide. Asked of the film-make lane: `ju` dispatch lines not in yet, so the app calls the scripts directly.
- `ju mend` applies corrections to a finished film. It must redraw whole when the design generation differs. Not yet working; the splicing fault is still open.
- War Room has no `ju make` kind yet.
- The scale model is 352 channels in 54 niches (Ambi, 15:38, via the lead). Scouting runs 54 times a week, not 352.
- `ju pulse` (the weekly niche scan) runs in code plus one DeepSeek summary, about 63 seconds for all niches. No real YouTube data yet.
- Gate: 10 films pass rooms 1 to 3 after a fold fix (lead, 15:16).

## Web app and rooms
- The round-three app flow is in the main branch (commits 15:26 and 15:37). No test report yet.
- Changes landed in the rooms: empty first run, New Vessel with absorb, describe and ready-made, a Cauldron composer, a running Pact, and a Juju pop-out. The pop-out is a sidebar that stays on every page.
- "Tell Juju" was given the mend command (commit 15:27, "MEND-DONE").
- Last full control census (24 Nov): 573 controls; 112 real. Not re-run since.
- Phone rooms are not checked on a real phone.

## Mac app and APK
- Mac shell: no new report since 25 Nov. The old rooms still ship. Not tested.
- One APK built, 9.8 MB, on the phone branch. It runs a stand-in engine, not the real map drawer.
- Worker's test (15:55): with every Mac port blocked, the phone signed in through the Door, drew a 2-minute film, and saved it. The AI answer was a saved reply, so $0 was spent.
- Emulator screenshots came back black. The worker took pictures from inside the app.
- ANR (app not responding) under CPU pressure is open.
- Not tested on a real phone. The Galaxy is not plugged in (last sheet; no newer message).

## Agents running now
- Live agent page did not answer. Running agents are known only from messages.
- Lead: last message 15:50 (diagnosis of the mend splice). Coordinating the lanes.
- Worker: last message 16:01 (Pulse and video lookup deployed; War Room being written).
- Door lane: last message 16:01 (scout and lookup deployed, no key).
- Core lane: last message 14:20 (planner not done; one unit test fails; packs build running).
- Phone lane: last message 15:55 (waiting for the core planner).
- Film-make lane: last message 15:54 (generation stamps; `ju make` stamping takes).
- Worlds lane: last message 14:47 (mend and tale). Worlds 2 started 15:16.
- Sound lane: last message 14:46. Night lane: last message 10:50, parked.
- Route and place lane: last message 15:55. Asked to build pulse, bend and fill.
- Screens worker: first run built, waiting for a build slot.

## Money spent on services
- Ledger: 10,470 calls, $35.80 in all, up $1.47 since 09:00.
- DeepSeek $10.80 (6,377 ok, last ok 15:44). OpenRouter $12.27 (3,409 ok, last ok 15:43). Google $8.39 (119 ok, last 13:59). Inworld $3.92 (458 ok, last 10:54). WaveSpeed $0.29 (last 25 Nov). Unsettled $0.14 (9 failed).
- Door cap: 5 US (lead, 15:04). Ambi has not named another.
- Route fallback: about 0.0001 US per call. Place fallback: 0.0001 US.
- Pulse summary: 0.00026 US per niche.
- Mend: 0.0125 US.
- Night round two: 0.10 US.
- Neon: about 0.24 US, stopped.
- YouTube: 102 units per niche, Door ceiling 9,000 units a day. Nothing spent; no key.

## Broken, blocked or open
- The engine cannot yet use War Room, and `ju` dispatch lines are not in.
- Mend splices old and new design generations. A patch is written but not built. The app hides mended takes and the "Use this one" button until it is fixed.
- The Africa share figure is wrong by code. The engine lane's fix is in flight.
- Gold6 night film missing; canon check fails on it.
- Night: the plain globe turns lights to beige blobs at 1 degree. The looks owner must fix the plain look file. The seviller2 redraw failure is unexplained.
- Core: planner port not done; one library unit test fails.
- Phone: stand-in engine; the packs are not published; the ANR is open.
- Door: no YouTube key, so no real scout or video lookup yet. Paid calls refused until the sign-in codes are set.
- Outlier and flop cut-offs (3 times and a quarter of a channel's average) are the worker's choice, not yet approved.
- Africa 26-minute film: loudness not confirmed; Ambi has not heard it.
- Worlds: the crown waits on reading seven own-record stops. The myth's opening world view has a smeared top band.
- Not proven: a voiced film over 10 minutes; any phone build; the 95 of 100 taste bar; that a cheap model fills recipes at 95% legal first answers.
- juju-maps is not in git; there is no commit id for it.

## Waiting on Ambi
1. Make the YouTube key and store it (steps in the Door's key notes, about 5 minutes). Pulse and video lookup need it.
2. Set the two sign-in codes so paid calls work, then name the live cap (5 US now).
3. Say whether the $35 cap still holds. The ledger is at $35.80.
4. Approve or change the outlier and flop cut-offs.
5. Listen to the first 2 minutes of the 26-minute Africa film with sound, and say if it feels right.
6. Night on two grounds is parked by the lead. No ruling from Ambi.
7. Plug in the Galaxy. Phone tests have run on an emulator only.
8. The no-tell-frames subtitle call (18 canon faults wait on it), per the last sheet.
9. Whether the map code goes into git without its data.





# Sheet of 09:00 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 04:47 to 09:00 EAT, Thu 26 Nov 2026 (FACTS NOW at 09:00).
- Spend rose from $32.37 to $34.33 over 9,858 to 10,145 paid calls. The cap is $35, so about $0.67 is left on the ledger. The lead's own reading meter shows 0.78 US spent on Roots against a 0.80 allowance (round seven).
- DeepSeek went from $8.12 to $9.89. OpenRouter from $12.21 to $12.23. Inworld from $3.69 to $3.85.
- Finish check: 1 of 23 clauses true, unchanged.
- Pull requests: 7 open, 19 merged, 1 closed, unchanged. Main has not moved since 11:13 on 25 Nov. Later work is uncommitted (Roots and Dates lanes, Tehuti, 08:44 to 08:50).
- Rust: 35,572 lines in 15 crates (was 35,232). Skills: 59 (was 56). Rooms drawn: 21 (was 20).
- Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD, unchanged. Newest DONE is still strip-japan.
- Logged attempts: 391 kept (was 348), 60 reverted (was 50), 52 inconclusive.
- Mac load is now 26, 34, 45 (was 6, 6, 7). The Mac is near 74 at 08:47 (worker).
- Canon lane (Tehuti, 06:20 to 08:50): skill packs countersigned in four requests. Audit of skill faults fell from 124 to 18 (all no-tell-frames). Crossroads, spirit-tongue and poteto are live. Brackets are one closed list of 8.
- Roots lane (Tehuti, 08:43, round seven): 8 of 12 undrawn Africa states now held. Sahara salt towns dated. Place index now builds in about 7 s of CPU.
- Dates lane (Tehuti, 08:47): tradition-only states draw hatched. Andes, East Asia, Nigeria and Cairo land built.
- Make lane (Tehuti, 07:51): `ju make` makes films from one sentence with no agent. Four films made; worlds refused on money.
- Night lane (Tehuti, 08:41): five first takes, spread 2.55. Not a pass.
- Latest worker lines (08:46 to 09:01): Mix for the Africa film is done (805 sounds, −14.01 LUFS). Narrated test starting at a cost cap of 0.06 US.

## What worked and what failed
**Worked (as reported)**
- Roots round seven: check.py TRUE. 24th Dynasty held at Sais, 735 to 721 BC (Tehuti, 08:43 and 08:44).
- Brackets: one list of eight, checked in code. The stories film and US film pass (Tehuti, 08:44 and worker, 09:00).
- Canon: audit of skill faults down to 18 (Tehuti, 08:22). Countersign rows 1 to 4 applied live. Pins 0 DIFF.
- Juju's own reader vs Haiku on one unit: 90 in 100 claims on shared lines, 82 same year, 96 pass the page check (Tehuti, 07:27 and Roots round six). Measured on one unit only.
- Make: four films made by `ju make` from `env -i`: wealth 6.5/10, states 5/10, Night 6/10, kingdoms 4/10 (Tehuti, 07:51). These are the lead's and worker's self scores, not a pass.
- Velocity: 1080p drawing costs 1,257 CPU s per 30 s window (Tehuti, 06:30).
- Make room: built and walked on desk and phone with no faults (Tehuti, 06:34). Not checked by anyone else.

**Failed or refused**
- Ambi's refusals still stand: stand-in drawings, the "slop" line, the dot strip, the 36-palette sheet, parchment, Moko Day, Jenny ring (not judged), and the glowing border and cheesy arrow of film 4. Ambi on Jakarta: "terribly bad", voice "AI-ish". Night round two: 4.5 and 4. The "not broken since 1992" line was false and was not caught.
- Green Sahara: marked 5 and held. It uses made-up peoples where digs show real cultures.
- Juju Poly bodies: blind test lost (2 with, 4 without, 2 equal).
- Writer lane (lead, 00:49): long form 3 of 10 with a fresh reader. Istanbul lost 0 of 3.
- Worlds: refused on money (Tehuti, 07:51).
- Night on two grounds: five first takes, spread 2.55. Worst faults: plain globe at 0.2 deg is a blur; seam offsets 3 to 33% of width. Ambi has not ruled on it (Tehuti, 08:41).
- Crossroads ladder at max effort does not fit 4,000 tokens; the lead chose option (b), max kept within today's room (Tehuti, 07:47 and 08:00).
- Drawer speed: no processor route gives 5x same-looking (Tehuti, 07:47).
- Shots check: 8 of 64 fail (worker, 04:47). Not updated since.
- US states: Hawaii and Alaska stops; seven small cessions; cards read like a database.
- Africa film: Musa and Sahara each fail one gap check (Tehuti, 06:20 and 06:45). Four drawn films still fail the bracket check because they predate the new list (worker, 09:00).

## App engine and films
- `ju make`: four films made from one sentence. Five-film bar not met (worlds refused). Last whole `ju make` run failed on a roots query (KeyError partners), per Tehuti at 07:51.
- Newest DONE is strip-japan (60 s, 0.008751 US, 25 Nov 08:34). Newest HOLD is ottoman12f (25 Nov 11:25). Newest FAILED is proof12c (25 Nov 09:47).
- Africa 1080p: a 30 s window costs 1,257 CPU s; planning 373 s of which 197 s are 24 drawer relaunches (Tehuti, 06:30).
- Gap law 6: Africa 11-minute film refused for 15 framed states plus 5 stretches; Musa refused for Kilwa; Sahara 10 plus 3; US 1 stretch (Tehuti, 06:45). Law 6 runs report-only; FINAL flag off.
- Gap closing before drawing: not yet code for all films (Tehuti 06:20). Director, stripes, finals export not yet code (worker and Tehuti, 08:50 log).
- Voices: 19 of 19 pass the hard-name check at 0.91 or better. Àṣẹ Regular V 0.3 is wired. Nobody has listened to the Ear mix.
- Africa mix: 805 sounds on 1108 events, 6 beds, −14.01 LUFS (worker, 09:01). Not listened to.
- Night: no 1080p (none earned 7). Timemap global lock makes a 100 s ground wait 8 to 9 min (Tehuti, 08:41).

## Web app and rooms
- Make room (`/r2/make.html`) built. Routes under `/api/tap` in `make.rs`. Server build passes 22 unit tests. Desk and phone click walks ran with no faults (Tehuti, 06:34). Not tested on a real phone.
- App-made wealth film was still drawing at 50% when that log ended. Live swap on port 4700 and launchd load not done.
- Earlier pressed-for-real census (24 Nov): 573 controls; 112 real, 160 sample, 131 dead. Every path ended at the practice minute. Mirror Bend and Feed Sight showed broken or empty pictures. New Vessel and the Tank are drawings. The sound room sent you back to the Altar. Not re-checked since.

## Mac app and APK
- The Mac shell still bundles the old rooms (11:06 on 25 Nov). No release build. Not tested.
- APK files built: 0. Nothing has run on a phone. Not tested. The Galaxy is not plugged in.
- Make room runs on the test server (port 4705). Not in the Mac shell.

## Agents running now
- Live agent page did not answer. Running agents are known only from messages.
- Worker: latest 09:01 (Africa mix done; narrated test starting). Watching `juju-maps/films/sty-films.log`. Five style films: three drawn, City Towers, Engraved Atlas and two redraws queued.
- Tehuti: latest 08:50 (canon brackets in land names; migration rows 7 and 10 done). Canon, dates, roots, velocity and night lanes all write under this name.
- Lead: latest 08:44 (round seven done). Roots lane has no session after 08:50 per the lead's hand-off note.
- Dates lane: two films running (mk-andes, mk-korea), 18 to 30 minutes each (worker, 08:47). mk-andes still in director call at 08:49.
- Stories lane: session gone (Tehuti, 08:44). Hand-off waits in `canon/HANDOFF-brackets.md`.
- Type lane: no live session (Tehuti, 08:39).

## Money spent on services
- Ledger: 10,145 calls, $34.33 in all, up $1.96 since 04:47.
- DeepSeek $9.89 (6,129 answered, last ok 09:00). OpenRouter $12.23 (3,392 answered, last 07:46). Google $7.94 (104, last 00:46). Inworld $3.85 (426, last 08:59). WaveSpeed $0.288 (6, last 25 Nov 11:24). Unsettled $0.14 (7 failed).
- Cap $35. About $0.67 left.
- Roots lane: 0.78 US in all, inside its 0.80 allowance (Tehuti, 08:43).
- Make lane: 0.0899 US (Tehuti, 07:51).
- Velocity: DeepSeek 0.011 US (Tehuti, 07:48).
- Night: 0.34 US (Tehuti, 08:41).
- Worker: narrated test capped at 0.06 US (09:01).
- Neon hard read: 0.023 US per two-minute film, over the 0.02 bar. Wired but off.

## Broken, blocked or open
- Africa film: turn check FAIL 1 (655 BC). Bare 8:00 rest view. Fatimid colour near the prior ruler. Kush label on Assyria.
- Africa and Sahara films: "argued", "dates about" and "from the dug site" still in drawn text until a redraw. Musa, Sahara, both Africa films.
- Roots: Agades, Bono, Bonny and Nok still unheld. Andes 12 and East Asia 16 states held by passage. 25+ only with outside Cliopatria borders. Sibiridugu and Birni Kafela unplaced. Slave Voyages and ORBIS licences unreadable.
- Dates: Baekje's name on Silla's land (East Asia, AD 500), not looked into. Hatching shows all the time; should show only while the camera rests.
- Canon: 18 audit faults left, all no-tell-frames; waits on Ambi's subtitle call.
- Juju Roots: a book build takes about 7 min per Tehuti (07:27); later about 7 s of CPU (08:44). Conflicting; latest says faster.
- Law 6 report-only.
- Shots: 8 of 64 failing.
- Not proven: a voiced film over 10 minutes; a 20- or 25-minute film; anything on a phone; the 95 of 100 taste bar; the depict card.
- Repo: `juju-maps/roots/` has never been committed; it is 1.0 GB, mostly downloaded data. The lead asks whether the code goes in without the data.

## Waiting on Ambi
1. Two grounds for Night and Day: yes or no. Night has five first takes, spread 2.55; not ruled.
2. Name for the drawer. The worker's pick is Juju Ardhi.
3. Simulations on real land: real cultures or imagined peoples. Green Sahara is held on this.
4. Voice: choose A or B, C or D. Àṣẹ Regular V 0.3 is wired.
5. Name for the voice toggle.
6. Name the two film systems, or accept "kingdoms" and "wealth".
7. Listen to the Ear mix on gold6 or marmara2.
8. Decide whether to lift the $35 cap. About $0.67 is left.
9. Plug in the Galaxy.
10. no-tell-frames subtitle call (18 canon faults wait on it).
11. Channel pick for the three map channels (Tehuti, 07:48).
12. Whether the roots code goes into git without its data.
13. Critique the Africa films, the US states film and the Night takes.






# Sheet of 04:46 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 02:43 to 04:47 EAT, Thu 26 Nov 2026.
- Spend rose from $32.34 to $32.37 over 9,839 to 9,858 paid calls. The cap is $35, so about $2.63 is left on the ledger.
- Finish check: 1 of 23 clauses true, unchanged.
- Pull requests: 7 open, 19 merged, 1 closed, unchanged. The open ones are 21 to 27.
- Main: newest commit still 11:13 on 25 Nov. Time-map, dates, roots and states work is uncommitted (Tehuti, 03:14 and 04:43).
- Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD, unchanged. Newest DONE is still strip-japan.
- Logged attempts: 348 kept (was 328), 50 reverted, 52 inconclusive.
- Mac load now 6, 6, 7 (was 52, 57, 49).
- Dates crate: 27 of 27 tests pass (Tehuti, 04:18). States are sized by the highest-ranked source, not the Cliopatria set.
- Roots: check.py prints TRUE. 264 holds, 237 placed, 99 states with a dated hold (Tehuti, 03:58). Carthage now runs 814 to 145 BC. Mali has a state row. Eighteen checked extent rows cover the first ten states (Tehuti, 04:34).
- Africa time map: the 12-minute film was redrawn at 697.4 s. Turn check shows FAIL 1 (655 BC, same holder, no drawn change). Tehuti marks it 6.5 of 10. Tehuti is its maker.
- US states film: drawn on the shared Africa path at 360.9 s. Tehuti marks it 6 of 10. The find moment and zoom-sized text are built.

## What worked and what failed
**Worked (as reported)**
- Africa film: Egypt's chain reads, and 22 of 23 flips show on drawn frames (Tehuti, 04:26).
- Dates crate: planted faults fail as they should. Carbon ranges are kept as ranges. Published checks: Cajamarca within 2 years, Great Zimbabwe within 5 (Tehuti, 03:09).
- Ambi, relayed in the 02:35 log: "solid in code ... true to indigenous accounts and carbon dating."
- States sizes, measured on 21 states: mean gap 0.97 to 0.23 on a log scale (Tehuti, 04:11).
- US states film: clock worst change 3.94, under the limit of 4. Fort Sumter dive is sharp, with islands and harbour (Tehuti, 04:43).

**Failed or refused**
- Ambi's refusals still stand: stand-in drawings, the "slop" line, the dot strip, the 36-palette sheet, parchment, Moko Day, Jenny ring (not judged), and the glowing border and cheesy arrow of film 4.
- Ambi on Jakarta: "terribly bad", voice "AI-ish".
- Night round two: 4.5 and 4 (Tehuti, 03:14). Further Night spending is held. The round-one line "not broken since 1992" was false and was not caught.
- Green Sahara: marked 5 and held. It uses made-up peoples where digs show real cultures.
- Juju Poly bodies: blind test lost (2 with, 4 without, 2 equal).
- Writer lane (lead, 00:49): long form 3 of 10 with a fresh reader. Istanbul lost 0 of 3. Max thinking took twice the time and cost for 7 of 12 votes, so low stays the default.
- Congo economics film is wrong; its redraw is not done.
- Shots check: 8 of 64 fail (worker, 04:47). Which test is being checked.
- US states: Hawaii 1898 and 1959 stops are dark or tiny. Alaska 1959 shows as a round green blob. Seven cession shots fill too little of the frame.

## App engine and films
- Juju make: newest DONE is strip-japan (60 s, 0.008751 US, 25 Nov 08:34). Newest HOLD is ottoman12f (25 Nov 11:25, stopped at Pictures and form). Newest FAILED is proof12c (09:47).
- Time maps: Africa 12-minute film at 697.4 s. US states film at 360.9 s. Names are hidden where a later land covers them. "Kush" still sits on Assyria at 663 BC.
- Find moment: built and tested on a fixture card. No real story carries a find yet.
- Juju Shots round two (scar, bristol, khovd) has no blind judge.
- Voices: 19 of 19 pass the hard-name check at 0.91 or better. Àṣẹ Regular V 0.3 is wired. Nobody has listened to the Ear mix.

## Web app and rooms
- No new web report since 22:39 on 25 Nov.
- At that report, every path ended at the practice minute. The five cards were placeholders. Mirror Bend and Feed Sight showed broken or empty pictures. New Vessel and the Tank are drawings. The sound room sent you back to the Altar.
- Census: 573 controls; 112 real, 160 sample, 131 dead.

## Mac app and APK
- The Mac shell still bundles the old rooms (11:06 on 25 Nov). No release build. Not tested.
- Juju Pots app: live balances; login not loaded (Tehuti, 23:45 on 25 Nov).
- APK files built: 0. Nothing has run on a phone. Not tested. The Galaxy is not plugged in.

## Agents running now
- The live agent page was not checked in this sheet. Running agents are known only from messages.
- Worker: latest message 04:47. Fixing the US states film (Alaska, Hawaii, framing, card rewording). Checking the 8 failing shots.
- Tehuti: latest log 04:43. Working on the time maps, dates, roots and states lanes.
- Dates lane: not running (worker, 04:34). Its handoff note was left in a file for it.
- Lead: quiet since 00:49. Writer lane closed.

## Money spent on services
- Ledger: 9,858 calls, $32.37 in all, up $0.03 since 02:43.
- DeepSeek $8.12 (5,874 answered, last ok 04:11). OpenRouter $12.21 (3,384 answered, last 01:43). Google $7.94 (104, last 00:46). Inworld $3.69 (402, last 02:10). WaveSpeed $0.288 (6, last 25 Nov 11:24). Unsettled $0.14 (7 failed).
- Cap $35. About $2.63 left.
- Neon hard read: 0.023 US per two-minute film, over the 0.02 bar. Wired but off.
- Pots: at 60 films of 22.5 minutes, short about $71 (Estimated).

## Broken, blocked or open
- Africa film: turn check FAIL 1 (655 BC). Bare 8:00 rest view. Fatimid colour near the prior ruler. Kush label on Assyria.
- Roots: unplaced holds in the queue. Sibiridugu and Birni Kafela are unplaced. 50 attestations and 37 takings have no dated end. Gazetteer names needed for the Delta, First Cataract, Mediterranean and Semna.
- Dates: no published check for Marine20. Kakapel matches IntCal20 within 1 year, but its paper says SHCal20. Render and framing not verified.
- US states: Hawaii and Alaska stops; seven small cessions; cards read like a database; the 150 px find pan is not built.
- Shots: 8 of 64 failing.
- Not proven: a voiced film over 10 minutes; a 20- or 25-minute film; anything on a phone; the 95 of 100 taste bar; the depict card.

## Waiting on Ambi
1. Two grounds for Night and Day: yes or no. The candidate is a drawer for wide views and a plain globe up close (Tehuti, 03:11).
2. Name for the drawer. The worker's pick is Juju Ardhi.
3. Simulations on real land: real cultures or imagined peoples. Green Sahara is held on this.
4. Voice: choose A or B, C or D. Àṣẹ Regular V 0.3 is wired.
5. Name for the voice toggle.
6. Name the two film systems, or accept "kingdoms" and "wealth".
7. Listen to the Ear mix on gold6 or marmara2.
8. Decide whether to lift the $35 cap. About $2.63 is left.
9. Plug in the Galaxy.
10. Tehuti's five questions are unanswered (01:41): odds in counts, hatched own record, outside dating, banners, Night keeps the globe.
11. Critique the 12-minute Africa film, the US states film and Night round two.







# Sheet of 02:43 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 00:41 to 02:43 EAT Thu 26 Nov 2026. Current time 02:43.
- Spend rose from $29.91 to $32.34 over 9,048 to 9,839 paid calls. DeepSeek +$2.14, OpenRouter +$0.12, Google +$0.04, Inworld +$0.17. Lead's cap was $35. Worker reports test spend $32.40 of $35 (02:43 worker message, 01:34 Tehuti said $30.41 of $35; the later figures differ, the ledger is used here).
- Finish check: 1 of 23 clauses true, unchanged.
- Pull requests: 7 open, 19 merged, 1 closed, unchanged.
- Main: newest commit still 11:13 on 25 Nov. Tehuti's time-map and Juju Roots work is uncommitted (Tehuti, 02:30 and 02:41). Nothing committed.
- Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD, unchanged. No new `juju make` run in FACTS. Newest DONE is still strip-japan.
- Rust: 35,232 lines in 15 crates, unchanged. Decisions: 27 (was 25). Skills 56, rooms 20, APK 0, unchanged.
- Logged attempts: 328 kept (was 313), 50 reverted (was 45), 52 inconclusive (was 50).
- Mac load 52, 57, 49 (was 42, 47, 58). Agent transcripts written in the last 10 minutes: 0.
- Writer lane closed (Tehuti, 00:52; lead, 00:49). Short two-minute scripts: DeepSeek won 6 of 8 films, 18 of 24 votes, seven films reuse version 4 drafts. Long 19-minute script judged 3 of 10 (lead, fresh reader). Max thinking: 7 of 12 votes at twice the time and cost; low stays default. Hard read wired but off (0.023 US, over the 0.02 bar).
- Juju Shots (picture-first films) started. First takes self-judged 4.5 to 6.5 (Tehuti, 01:39, 02:34). Round two: scar, bristol, khovd; no blind eye has judged them.
- Juju Roots: source shelf of 80 open sources, 12 refused, Africa world book of 435 rows (10 readers of UNESCO GHA II to IV). check.py prints TRUE (Tehuti, 02:30, 02:41). Corrections: Mehrgarh disputed, Turin papyrus counts, Native Land refused by its licence.
- Juju Roots: check.py now fails on a year that stands on no page (planted fault fired, 02:39).
- Time maps: seven-minute Africa story (43 stops, 490 s) rebuilt from proved sources; tm-sahara roads by a stated rule; tm-asia new (14 stops, 210 s). Africa turn stops: 21 of 28 quoted, 7 title only, 7 marked argued. Lead's mark on Asia 7, South America 6, Europe 5, North America held back (Tehuti, 01:11).
- Juju Kinds: seven story kinds in code; Istanbul and po3 gold unchanged to the byte (golden.py, 01:41).
- Juju Dates crate (juju-maps/dates): builds; 19 law tests pass; render and camera framing not yet checked (Tehuti, 02:32).
- Blind test on Juju Poly bodies lost: with 2, without 4, equal 2 (worker, 00:39). Models now shown only in views closer than about 250 km (Tehuti, 01:34).
- Voice Harold banned (Tehuti, 00:51). Voices: 19 of 19 pass the hard-name check at 0.91 or better (machine listener). Wired as Àṣẹ Regular V 0.3.

## What worked and what failed
**Worked** (as reported)
- DeepSeek two-minute scripts: 6 of 8 films, 18 of 24 votes (lead, 00:48; Tehuti, 00:49). Lost Istanbul 0 of 3 and Congo 1 of 3.
- Africa time map: Ambi "absolutely beautiful ... almost perfect" (relayed 00:02, earlier). Seven-minute Africa redrawn at 1.6 cents, mark 7 (Tehuti, 01:34).
- Juju Roots check.py TRUE; fires on planted faults (Tehuti, 02:30, 02:41).
- Africa world book: before 1000 BC 25 events vs 2 in old film (worker, 02:40). Measured.
- Turn stops: 36 of 36 turns on screen (worker, 02:44).
- Time-type page: blind readers 5.4 and 5.1 against 4 for old films (Tehuti, 01:34). Nobody has seen it move.
- Safety net: planted fault caught; ./ju doctor 10 of 10 (Tehuti, 00:42).
- Tile cache moved; CPU 73 to about 41 (Tehuti, 00:43).
- Stories: 5 of 6 pass check (worker, 02:43); tm-output fails one gap.

**Failed or refused**
- Juju Poly bodies: blind test lost (2 with, 4 without, 2 equal). Bar not met. Live set is the old one Ambi rated 8. Istanbul frozen.
- Max thinking: 7 of 12 votes at 0.037 US against 0.017 for low; not the default (lead, 00:49).
- Long 19-minute script: 3 of 10, fresh reader. Pockets planned one by one; no person carries the film (lead, 00:49).
- Congo economics sheet: a railway company's paperwork; two listeners preferred the old headings (lead, 00:49).
- Istanbul under the writer: lost 0 of 3 (lead, 00:48). Rule to catch pairs of towns not yet heard by a listener.
- Juju Shots first takes: 4.5 to 6.5 by the builder's own eye; no blind judge yet (Tehuti, 01:39). Night round one: quakes "the ground moved" repeats, false "not broken since 1992" line (lead, 01:xx and 02:34).
- Night round two: frame, figures from the sentence, dated shapes. Bristol, scar, khovd tested; bristol towns faint.
- Africa turn stop dates: 7 wrong against sources, shown as argued (worker, 02:44).
- Ambi's refusals still stand: stand-in drawings, "slop" line, dot strip, 36-palette sheet, parchment, Moko Day, Jenny ring (unjudged), glowing border and cheesy arrow of film 4.
- Ambi's 8 on Istanbul gold: kept as the live set.
- Ambi on Jakarta: "terribly bad", voice "AI-ish". Jakarta voice: banned Harold voice used (Tehuti, 01:34).

## App engine and films
- Juju make: newest DONE is still strip-japan (60 s, 08:34, 25 Nov).
- Time maps, newest: tm-africa (43 stops, 490 s, rebuilt from proved sources); tm-africa-long (first ~7 min of 20-min film); tm-sahara; tm-musa; tm-output (fails one gap, 39 s, one stop); tm-asia (14 stops, 210 s, passes check).
- Time-map frames: four films for critique (Asia, South America, North America, Europe, World) drawn; all decode to 125 s (Tehuti, 01:11). Asia best; North America held back (camera leaves to Siberia).
- Juju Shots round two: scar (quakes, seen 7 of 8), bristol (Black Death, seen 4 of 13), khovd (Xiongnu, seen 6 of 9). Not blind-judged.
- Juju Dates: crate builds, 19 tests pass; film render and camera framing not yet checked (Tehuti, 02:32).
- Voices: 19 on the shelf; Àṣẹ Regular V 0.3 wired; dear Àṣẹ High V 0.3. Ambi still to choose.
- Sound: nobody has listened to the Ear mix.

## Web app and rooms
- Not reported in this window. Last reported state (22:39 sheet): every path ends at the practice minute; census 573 controls, 112 real, 160 sample, 131 dead.
- No new web app report since 22:39.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone. Not tested.
- Mac shell still bundles the old rooms (11:06 25 Nov). No release build. Not tested.
- Juju Pots app at ~/Applications/Juju Pots.app (Tehuti, 23:45): live balances; login not loaded.
- Juju Maps has its own git repository; a private GitHub save runs every half hour (Tehuti, 23:57).
- Mac load 52, 57, 49 at 02:43.

## Agents running now
- The live agent page did not answer; running agents are unknown.
- Worker (02:43): stories fix file in; rewriting reader to its real shape; the 132 dates and 95 holds from Roots pass law checks; the Africa draw predates fixes and was stopped.
- Tehuti (02:44 last entry): Juju Roots, Juju Dates, Juju Shots, Juju Kinds, time-map story lane. Last reports: worker 02:44 (Persia–Egypt fix), Tehuti 02:43 (turn stops, titles, Asia pocket).
- Lead (00:52 last): writer lane closed; no new lead message after 00:49.

## Money spent on services
- Ledger: 9,839 calls, $32.34 in all.
- DeepSeek $8.08 (5,855 answered, 17 refused or failed; last 02:42). OpenRouter $12.21 (3,384, 45; last 01:43). Google $7.94 (104, 13; last 00:46). Inworld $3.69 (402, 1; last 02:10). WaveSpeed $0.288 (6, 2; last 25 Nov 11:24). Unsettled $0.14 (7 failed).
- Cap: $35. Ledger shows about $2.66 left. Worker reports DeepSeek $0.673 for its lane, $0.216 unspent; Tehuti reports DeepSeek 0.589 of 0.60 spent in time-story lane (02:18).
- Writer lane: DeepSeek about $0.72 of $0.70, GLM $0.03 of $0.05 (lead, 00:49).
- Neon hard read: 0.023 to 0.024 per two-minute film; wired but off.

## Broken, blocked or open
- GitHub billing blocks merge of seven pull requests (lead, 08:16 25 Nov). No later report.
- Main has no new public commit since 11:13 25 Nov. Juju Maps and Roots work is uncommitted.
- Writer: long form 3 of 10; a sourced sheet per pocket and one carrying person still needed.
- Istanbul under the writer: lost 0 of 3.
- Juju Poly bodies: lost blind test; houses that flood and small day boats lost; four verbs lack a still.
- Juju Shots: no blind judge yet; bristol towns faint; people, bars and years shots weak.
- Night round one quake line "not broken since 1992" was false and was not caught.
- Time-map: tm-output fails one gap (39 s, one stop); 7 Africa turn-stop dates argued; engine must draw new Roots rows (FINDS/ACCOUNT types not yet read).
- Juju Dates: render and framing not verified.
- Congo economics film wrong; redraw not done.
- Sound: nobody has listened to the Ear mix.
- Pots: at 60 films of 22.5 min, pots short about $71 (Estimated).
- Not proven: a voiced film over 10 minutes; a 20- or 25-minute film; anything on a phone; the 95 of 100 taste bar; the depict card (8 of 12, under 10); Bernal's Black Athena not on the shelf yet.

## Waiting on Ambi
1. Choose a voice: A or B, C or D.
2. Close the seven old pull requests, or fix GitHub billing so they merge.
3. The money window at login: say yes or no.
4. Name the two film systems or accept "kingdoms" and "wealth".
5. Pick a name for the voice toggle.
6. Listen to the Ear mix on gold6 or marmara2.
7. Decide whether to lift the cap above $35. About $2.66 is left on the ledger.
8. Plug in the Galaxy.
9. Tehuti's five questions (odds in counts, hatched own record, outside dating, banners, Night keeps the globe) are unanswered (Tehuti, 01:41).
10. Critique the new time-map films (Asia, South America, North America, Europe, World) and the Night round-two films.








# Sheet of 00:41 EAT, Thu 26 Nov 2026

## Changed since the last sheet
- Covers 22:39 EAT Wed 25 Nov to 00:41 EAT Thu 26 Nov 2026. Current time 00:41.
- Spend rose from $27.13 to $29.91 over 8,274 to 9,048 paid calls. DeepSeek +$2.05, OpenRouter +$0.11, Google +$0.42, Inworld +$0.20.
- Lead's own figure at 00:15 was $28.18 of $35; worker's at 00:42 was $29.97 of $35. The ledger shows $29.91. Cap now $35 (was $30). The lead says Ambi's order is 35; the ledger's cap file reads 35 (Tehuti, 23:20).
- Finish check: 1 of 23 clauses true, unchanged.
- Pull requests: 7 open, 19 merged, 1 closed, unchanged. Main's newest commit is still 11:13 on 25 Nov. Tehuti reports a private main save at 23:57 (a3010f5), not on the public list.
- Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD, unchanged. No new `juju make` run in FACTS.
- Rust: 35,232 lines in 15 crates (was 34,793 in 14). Decisions: 25 (was 22). Skills 56, rooms 20, APK 0, unchanged.
- Logged attempts: 313 kept (was 302), 45 reverted (was 42), 50 inconclusive, unchanged.
- Mac load 42, 47, 58 (was 58, 47, 37). Two transcripts written in the last 10 minutes.
- The live agent page did not answer, so running agents are unknown. Workers report six lanes running at 00:02 (engine, type, stories, kinds, writer, poly).
- Built since 22:39 (self-reported, judged only where stated):
  - Writer: DeepSeek wins most two-minute scripts blind. Haiku listeners chose it 21 of 24, stricter Opus 14 of 16 (lead, 23:56). Istanbul lost (2 of 5). Its 25-minute script scored 3.5 of 10 with false facts. The lead's stop rule was declared FALSE at 23:56. Max thinking not measured.
  - Juju Poly (ADR 0025): 28 own models, casting. Blind test on 8 ten-second pairs: with bodies 2, without 4, equal 2. Lost. Live set restored (worker, 00:39). Istanbul is frozen by Ambi (rated 8).
  - Time maps (ADR 0027): tm-africa and tm-output drawn in 26 to 34 s. Ambi on Africa: "absolutely beautiful ... almost perfect" (relayed 00:02). Wanted: less text, better fonts, no glitches, calmer clock, placed assets, 20-minute pockets.
  - Juju Ear: every move heard by count (120 of 120 on gold6); nobody has listened.
  - Juju Pots window at runs/pots/window.png; guard built but off.
  - Safety net: golden.py locks istanbul and po3; `./ju doctor` 10 of 10 OK at the worker's run.
  - Voices: 19 of 19 pass the hard-name check at 0.91 or better on the cheap model (machine listener). Wired as Àṣẹ Regular V 0.3 and Àṣẹ High V 0.3. Voice choice from Ambi still open.
  - Juju Maps: ground rules, shore ring, thin crack, painted night land on, villages off by default.

## What worked and what failed
**Worked** (as reported)
- DeepSeek writer, two-minute scripts: 21 of 24 blind votes from Haiku listeners; 14 of 16 from stricter Opus (lead, 23:56). Cost about 1.7 cents a script (lead).
- Istanbul gold: Ambi marked it 7 ("after one minute it just stops doing things", relayed 22:53). Frozen since.
- Africa time map: Ambi "absolutely beautiful ... almost perfect" (relayed 00:02).
- Safety net: planted fault caught (worker, 00:42).
- Voices: all 19 pass the hard-name check (machine listener, 00:42).
- Money window and GitHub save built (Tehuti, 23:58).
- Tic fixer: now runs all 125 rules; was silently skipping 26 (Tehuti, 23:44).
- Time-map study: blind rebuild 0.43 against 0.35 unrelated (Tehuti, 23:42).
- Mac load: 150 down to 13 (Tehuti, 23:44); later 73 down to 24 (worker, 00:42).

**Failed or refused**
- Istanbul under strict writer listeners: DeepSeek lost 0 of 2 (lead, 23:56), 2 of 5 (Tehuti, 23:57).
- 25-minute writer script: 3.5 of 10, false facts, repeats (lead, 23:56). Not sourced. Unproven.
- calabash.heal: 2 of 3 rewrites invented a person; not wired. The rule that caused it was removed (Tehuti, 23:57).
- Juju Poly bodies, blind: with bodies 2, without 4, equal 2 (worker, 00:39). Houses that flood and small day boats lost. Bar not met.
- Congo economics film: wrong Congo filled; about 3.5 by lead; redraw not done (Tehuti, 22:53).
- Writer's Congo sheet: asked twice, failed (lead 23:56).
- Ambi's refusals still stand: stand-in drawings, "slop" line, dot strip, 36-palette sheet, parchment, Moko Day, Jenny ring (unjudged), and the glowing border and cheesy arrow of film 4 (relayed 20:32).
- Ambi's 8 on Istanbul gold: kept as the live set.

## App engine and films
- Juju make: newest DONE is still strip-japan (60 s, 08:34, 25 Nov).
- Juju Maps films, newest:
  - Istanbul gold, gold6 and gold-ear: Istanbul frozen by Ambi. Mark 7 (Ambi, relayed 22:53).
  - tm-africa and tm-output (time maps): drawn 26 to 34 s; marks 7 and 6.5 (agent, 23:57). Ambi: "almost perfect" on Africa.
  - Juju Poly tests: po3 with/without; kivu2 with/without; jakarta with/without (worker, 00:15). Jakarta sea wall win.
  - marmara2 with ear sound; Congo economics film (about 3.5 by lead, not sent).
- Long films: 25-minute script not working; no sourced sheets per pocket. Not built.
- Voices: 19 on the shelf; cheap voices Àṣẹ Regular V 0.3 and dear Àṣẹ High V 0.3 wired. Ambi still has to choose (A or B, C or D).
- Sound: every move heard by count (120 of 120 on gold6); no person has listened. Ear mix about -14 LUFS (measured).
- Speed: draw 93 s for gold6 at load 55 to 75 (Tehuti, 23:24). Time-map drawer capped at 4 threads.

## Web app and rooms
- Not reported in this window. Last reported state (22:39 sheet): Juju 0.2 presses on the test copy; every path ends at the practice minute; census 573 controls, 112 real, 160 sample, 131 dead.
- No new web app report since 22:39.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone. Not tested.
- Mac shell still bundles the old rooms (11:06 25 Nov). No release build. Not tested.
- Juju Pots app at ~/Applications/Juju Pots.app (Tehuti, 23:45): live balances, not swapped into the server; login not loaded.
- Juju Maps has its own git repository; a private GitHub save runs every half hour (Tehuti, 23:57, launchd loaded).
- Mac load 42, 47, 58 at 00:41.

## Agents running now
- The live agent page did not answer; running agents are unknown.
- Lead: writer and long-form sheets (23:56, 00:15, 00:16).
- Worker (00:42): six lanes, time engine remaking Africa, kinds, writer, poly report, worlds, stories, type.
- Tehuti (00:02): engine, type and stories lanes started; writer, kinds and poly lanes also running.
- Last reports: worker 00:42 (safety net, voices); Tehuti 00:40 (bodies lost; live set restored).

## Money spent on services
- Ledger: 9,048 calls, $29.91 in all.
- DeepSeek $5.96 (5,138 answered, 17 refused or failed; last 00:41). OpenRouter $12.09 (3,333, 45; last 00:30). Google $7.89 (102, 13; last 00:39). Inworld $3.54 (381, 1; last 00:17). WaveSpeed $0.288 (6, 2; last 25 Nov 11:24). Unsettled $0.14 (7 failed).
- Cap: $35 (Ambi's order). Ledger shows about $5.09 left.
- Writer cost: about 1.7 cents a script (lead); bench round about $0.17 (lead, 23:56). Chooser spend $0.057 (Tehuti, 23:17). Bodies cast $0.182 for 52 calls (worker, 00:39).
- Neon cost on a hard read: $0.051 (lead, 23:52). Neon writer is no longer the default path.
- Inworld voice is the largest production cost per call; cheap voices now wired.

## Broken, blocked or open
- GitHub billing blocks merge of seven pull requests (lead, 08:16 25 Nov). No later report. PR 26 has one failed check.
- Main has no new public commit since 11:13 25 Nov. Juju Maps work is uncommitted; a private save is running.
- Writer: 25-minute script 3.5 of 10; long form needs a sourced sheet per pocket; hard read not wired; max thinking not measured.
- Istanbul under the writer: lost to Neon on the strict round.
- Juju Poly: lost blind test; houses that flood, small day boats, verbs in the words' own place; four verbs lack a still (open, unload, leave, wait); burn is weakest.
- Congo economics film wrong; redraw not done.
- Tic fixer: now runs; invented-people rule removed.
- Sound: nobody has listened to the Ear mix.
- Time-map worlds film: 34 s draw at the cap (bar 30).
- Pots: at 60 films of 22.5 min, pots short about $71 (Estimated). 70 CAD is $49.
- Not proven: a voiced film over 10 minutes; a 20- or 25-minute film; anything on a phone; the 95 of 100 taste bar; the depict card (8 of 12, under 10); niche facts (marked checked:false); a Neon shared-prefix cache.

## Waiting on Ambi
1. Choose a voice: A or B, C or D (the worker's ask, 00:03 and 00:42).
2. Close the seven old pull requests, or fix GitHub billing so they merge.
3. The money window at login: say yes or no.
4. Name the two film systems or accept "kingdoms" and "wealth" (worker, 00:03).
5. Pick a name for the voice toggle: Nommo 1 and Nommo 2, or Àṣẹ Tongue, or Anansi Tongue (worker, 00:24).
6. Listen to the Ear mix on gold6 or marmara2.
7. Decide whether to lift the cap above $35. About $5 is left on the ledger.
8. Plug in the Galaxy.









# Sheet of 22:39 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 20:37 to 22:39 EAT, Wed 25 Nov 2026. Current time 22:39.
- Spend rose from $24.90 to $27.13 over 7,884 to 8,274 paid calls. DeepSeek +$0.58, OpenRouter +$0.09, Google +$4.86, Inworld +$0.21.
- Cap: 30 US (Ambi's order). The lead reports $26.75 at 22:25 and "about 26.8" at 22:27 (Tehuti). The ledger shows $27.13 now, so the lead's figures are behind the ledger.
- Finish check: 1 of 23 clauses true, unchanged.
- Pull requests: 7 open, 19 merged, 1 closed, unchanged. Main's newest commit is still 11:13.
- Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD, unchanged. No new `juju make` run appears in FACTS.
- Decisions: 22 (was 20). Rust 34,793 lines, 56 skills, 20 rooms, 0 APK files, unchanged.
- Logged attempts: 302 kept (was 293), 42 reverted (was 41), 50 inconclusive (was 48).
- Mac load 58, 47, 37 (was 4, 5, 6). One transcript written in the last 10 minutes (was 0).
- The live agent page did not answer, so running agents are still unknown.
- Built since 20:37 (lead, Tehuti, Mungura, workers; judged only where stated): ADR 0023 (any niche, Night and Day lead, 28 min under 1.50) and ADR 0024 (every move heard, channel sound packs). Juju Maps: DeepSeek thinking fixed, cheap cut for a 100 s film at about $0.03; Neon cache understood (hits only in a continued conversation); flat coloured land; 19-voice shelf; living land painted into the ground tiles, off by default; a changes layer of 18 kinds, 53 niches; a depict card that did not prove better (8 of 12, below 10).
- Ambi's rulings since 20:37, as relayed: no glowing borders anywhere; countries flat, like Moko Dusk. Film 4 "cheesy, shiny border, fat arrow, 'scores four' meaningless" (20:32, relayed). Ambi's best film so far is the Istanbul quakes film with Gavin (21:15, Tehuti relays "best vid thus far tho, and good voice").

## What worked and what failed
**Worked** (as reported)
- Istanbul take 3: the lead marks it about 7 from its frames. Ambi has not marked it. Relayed as Ambi's best so far (21:15).
- Cheap cut: the lead reports a 100 s film cut in about 48 s for $0.006 (DeepSeek thinking, low). Not judged for quality. The lead's own view: first cut was as good as Neon's to about 60 s, then too still (22:03).
- Neon cache: hits in 3 of 3 test calls in a continued conversation (lead, 22:03). Not a shared prefix.
- Ground check on the lowpoly b film: 0.44% worst from the ground itself (Measured, 21:24).
- Timeline: each op's draw times read from the engine, 0 pops on six films (Measured, 22:35).
- Recorder refuses a film that does not play; a planted broken piece is caught (Tehuti, 21:15, 22:03).
- Juju Eye blind test on marmara: eye 4.8, count 5.6 (Tehuti, 21:15; Mungura, 21:21 agrees). Count is 0.8 too kind.
- Changes trial: 8 of 12 twice, inconclusive, below the 10 needed. Judged by one blind judge.
- Coast fix (Po, Dutch polders, New Orleans and others): judged by builder from stills (20:23, earlier).
- Lowpoly lake: place bug found and fixed; 22 places checked, none swapped (lead, 22:09).

**Failed or refused**
- Film 4 (North Anatolian ranked film): Ambi's words above, relayed at 20:32. Not re-judged.
- Economics film (Juju's own idea, "Why a Sack of Cement Costs Twice as Much Up the Congo"): lead eye about 3.5. Filled the wrong Congo. Fact fix started (lead, 22:37).
- Marmara: fault line never drawn; 1999 Izmit quake drawn over Istanbul at 52 s (eye, Tehuti 21:15). Istanbul take 3 fixes some of this.
- Depict card: 8 of 12 twice, reverted (Tehuti, 22:09).
- Sarygamysh lowpoly b: the critic says it suits Day, not low poly. Moko fit test returns "not fit" (worker, 21:24). The lead's mark about 5 from frames (22:09).
- Villages: the lead turned them off (22:25); the day villages at 1.6 degrees are faint (Tehuti, 22:34).
- Living land: lead does not meet the bar yet; left off (worker, 22:35).
- Ambi's older refusals still hold: stand-in drawings, the "slop" script line, the dot strip, the 36-palette sheet, parchment, Moko Day, Jenny ring (unjudged).
- Neon cache earlier: 0 hits (Tehuti 20:32). Cache now understood (above).

## App engine and films
- Juju make: newest DONE is still strip-japan (60 s, 08:34).
- Juju Maps films (not `juju make`): Istanbul take 3 (about 7, lead's eye; Ambi not yet). Istanbul seven-breaks (about 6.8, lead's eye; replaced by take 3). Economics Congo film (about 3.5, lead). Lowpoly Sarygamysh b (about 5, lead; critic says not low poly). Marmara (eye 4.8, Tehuti). Po3 (Tehuti mark 7.5; Juju Eye count 6.0). Film 4 (Ambi refused). Kazakhstan, Mississippi, kivu3 and ghosts were sent earlier; no new verdict.
- Congo: running end to end (Tehuti, 22:27). Not reported done.
- Long films: the 28-minute cost estimate is $1.40 to $1.75 (lead, 22:09). Not built.
- Voices: the 19-voice shelf is built; 56 dry casts, 14 voices used, none off the shelf (Tehuti, 19:55). Ambi asked to choose from five (Gavin, Tonya, Russell, Marek, Kristen). Ambi's best so far uses Gavin (21:15).
- Sound: the lead reports a 100 s film's sound at -14.0 LUFS, peak -0.7 dB, measured, not heard. Sound packs per channel are being built; no film has a new sound mix yet.
- Speed: a whole cut at low thinking is about 48 s (lead, 22:03). Render target 1.0 still not reported as met.

## Web app and rooms
- Not reported this window. Last reported state (20:37): Juju 0.2 presses on the test copy; no paid press run; app price button still says $0.60 a film; films over 2 minutes not built.
- Census (24 Nov): 573 controls; 112 real, 160 sample, 131 dead.
- Make-a-film room: 71 steps, 0 bad, on the practice copy (11:07). Not checked on a real film.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone.
- Mac shell still bundles the old rooms (11:06). No release build. Not tested.
- ADR 0022: Juju is map films only; the drawing engine is forked as Juju Maps. Making a film with the Mac closed is unresolved.
- Juju Maps has its own git repository. Its last commit is a merge from another project. A reset or checkout could overwrite files (16:12). Not reported since.
- Mac load 58, 47, 37 at 22:39. Heavy runs are active.

## Agents running now
- The live agent page did not answer at 22:39. Running agents are unknown.
- Last reports: lead 22:37 (economics film fact fix); worker 22:35 (living land and timeline); Tehuti 22:34 (villages off by default, one engine per film); Mungura 21:21.
- Reported running: Congo film end to end (Tehuti 22:27); sound, motion and time-map workers (Tehuti 22:27 and lead 22:09); Neon T2 for plan and script (Tehuti 22:03); Geopanda-type film and niche list (lead 22:09).
- Reported done: stack checks (test_changes and test_kit pass, 22:14); recorder safe kill (22:35); voice shelf and dry casts (19:55).

## Money spent on services
- Ledger: 8,274 calls, $27.1299 in all.
- DeepSeek $3.9136 (4,436 answered, 17 refused or failed; last 22:38). OpenRouter $11.9831 (3,301, 45; last 22:31). Google $7.4717 (95, 13; last 22:36). Inworld $3.338 (348, 1; last 22:29). WaveSpeed $0.288 (6, 2; last 11:24). Unsettled $0.1355 (7 failed).
- Cap: 30 US (Ambi's order). Ledger shows $27.13 used, about $2.87 left. The lead reports "about $26.75" at 22:25 and Tehuti "about 26.8" at 22:27; both are behind the ledger.
- Neon rules (lead, 17:33, earlier): Google credit, at most $0.16 a film; otherwise GLM and DeepSeek. Cut at about $0.03 plus $0.05 for Neon's plan (lead, 22:03). Neon spent $0.32 on the whole 100 s film before (lead).
- Inworld voice is the largest production cost: $25 per million characters (Tehuti, 17:30, earlier).

## Broken, blocked or open
- GitHub billing blocks merge of seven pull requests (lead, 08:16). No later report. PR 26 has one failed check.
- Main has no new commit since 11:13. Juju Maps work is uncommitted.
- Istanbul take 3: the crack is a fat black blob; the sound is the old mix; year labels crowd near Izmit at 53 s; the close sea view at 66 s is plain (lead, 22:25).
- Economics film: wrong Congo filled; a fact fix is in progress (lead, 22:37).
- Recorder: the 12-window day scene never got ready in 240 s; cause unknown (worker, 22:23 in the changes trial).
- Storyboard3 line 387 sends sweep a bare name ("Iraq" lit the wrong place). Fix proposed: country=1 or rings (Tehuti, 22:14).
- Two old film files were unreadable (mississippi, gB). Cause not proven (Tehuti, 21:15).
- Marmara: the count is 0.8 too kind (Tehuti, 21:15). The count fell from 6.3 to 5.6 after score.py changed; likely cause, not verified (Mungura, 21:21).
- Sarygamysh lowpoly: the lake's place rows are swapped in the atlas file; a fix exists in one file, not in the writer (worker, 21:24).
- Villages and life are off by default; day villages faint at 1.6 degrees; no daytime air photo compared (Tehuti, 22:34).
- Sound packs and the motion and time-map layers are not yet joined into a whole film (lead 22:09, worker 22:35).
- Not proven: a voiced film over 10 minutes; a 20-minute film; anything on a phone; the 95 of 100 taste bar; the depict card (8 of 12, under 10); niche facts (marked checked:false); the 0.4 s wipe-out; a Neon shared-prefix cache.

## Waiting on Ambi
1. Mark Istanbul take 3 out of 10 (the lead's ask, 22:25). Ambi's best so far, relayed at 21:15.
2. Watch the Congo economics film when it is fixed. Its wrong-place fact was found at 22:37.
3. Choose a voice from five auditioned (Gavin, Tonya, Russell, Marek, Kristen).
4. Judge the sarygamysh b film against his taste (lead's mark about 5).
5. Judge the Juju Maps films: Marmara, Po3, Istanbul take 3, Congo.
6. Decide whether to lift the cap above 30 US. About $2.87 is left.
7. Fix GitHub billing so seven pull requests can merge.
8. Plug in the Galaxy.










# Sheet of 20:37 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 18:36 to 20:37 EAT, Wed 25 Nov 2026. Current time 20:37.
- Spend rose from $19.52 to $24.90 over 7,001 to 7,884 paid calls. DeepSeek +$0.62, OpenRouter +$0.75, Google +$2.40, Inworld +$1.61.
- Cap: Ambi's order is 30 US (Tehuti, 19:30). The day log still says 20, with 25 as the hard limit. About $5 was left at 20:32 (Tehuti).
- Finish check: 1 of 23 clauses true, unchanged.
- Pull requests: 7 open, 19 merged, 1 closed, unchanged. Main's newest commit is still 11:13. Juju Maps work since 17:30 is uncommitted.
- Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD, unchanged. No new `juju make` run appears in FACTS.
- Rust 34,793 lines, 56 skills, 20 rooms, 20 decisions, 0 APK files, all unchanged.
- Logged attempts: 293 kept (was 283), 41 reverted, 48 inconclusive. Mac load 4, 5, 6 (was 27, 14, 19). Disk about 24 GB free (Tehuti, 19:30).
- Built since 18:36 (reported by workers and lead; judged only where stated): flat coloured countries and solid lines in Juju Maps; one fixed ground per film; sea squares and labels fixed; a 19-voice shelf with casting only from it; near-shore mazes removed and a coast file that decides the sea; a 9 MB land file for diked land; ranked-film skeletons; a 28-minute ranked film read frame by frame.
- Ambi's rulings since 18:36, as relayed:
  - Scripts with "character" are bad. Copy real speakers' skeletons, draw far more, change views, be fast, use the best voices (19:30).
  - Borders must be coloured, not lit: "why is it shining instead of it being colored" (19:53). Later: no glowing borders anywhere.
  - Film 4, the North Anatolian ranked film: "cheesy, shiny border, fat arrow, 'scores four' meaningless" (20:32, relayed).
  - Three voices are blacklisted (19:30 and 17:39).

## What worked and what failed
**Worked** (as reported)
- Voice shelf: 18 of 19 voices hit the target rate, 155 to 170 (measured). 56 calls cost $0.288. No one has listened; machines only reject faults.
- Ground dance check: worst second on the kokaral film fell from 12.15% to 2.42%. Mountain film about 18% to 1.3% (measured, 18:57).
- Frame-by-frame read of a 28:38 ranked film: 40 scores, one each 26 s; a property planted at 2:38 and paid at 27:35 (measured, 18:43). Not a Juju film.
- Cold landing pre-fetch: 8 s landings went from 64.5 s with 40 late to 40.2 s, and 58.5 s with 0 late (measured, 19:38).
- Coast fix: Po, Dutch polders, New Orleans, Grays Harbor, Adriatic, Caspian, Andros. Judged by builder from stills (20:23).
- Ledger: every film Ambi liked ran Neon in the thinking seats; film 4 ran none (20:32). Worker agrees with Ambi's model suspicion (20:17).
- Juju picks press played on copied test data at zero cost (17:17). No paid press run.
- Board cutter: 2 minutes in about 90 seconds for about 9 cents (16:26, 17:05). Not judged for quality.

**Failed or refused**
- Moko Day: Ambi's refusal stands (17:02). Retired.
- Film 4: Ambi's words above. Worker also found one view held 0:35 to 1:20 and the Creep score was missing (19:38).
- Ranked study: 40 one-frame flashes; 97 of 111 captions repeat the voice; 59 words a minute on screen.
- Po film (20:17, worker): land below sea level painted as sea; river name shown twice. Coast fix addresses the first. The name fix is not confirmed.
- Jenny ring and lights (Ambi, 16:12): flat fills are the reply. Not judged.
- Rogun feed 7.3 against real 11.7 (17:05). Redrawn for cause (18:52). Not judged.
- Kazakhstan faults (lead, 17:26): no sound effects, port cranes too big, "950" before the water falls, soft ground close up.
- Ambi's older refusals still hold: stand-in drawings, the "slop" script line, the dot strip, the 36-palette sheet, parchment.
- Neon cache: 0 hits. 239 Neon calls ran on OpenRouter at 0%, $9.13 (Tehuti, 17:30). Still 0 hits at 20:32.

## App engine and films
- Juju make: newest DONE is still strip-japan (60 s, 08:34).
- Ranked film 4 ("I ranked famous fault lines by how long they have stayed quiet", 2:20, worker 19:38): refused by Ambi as above.
- Po film, "The delta that engineered itself under" (1:46, worker 20:17): drawn in 77 seconds, Neon thinking seats, new voice, flat land. Baseline sent to Ambi. No verdict.
- Mississippi, kivu3 and ghosts were sent (19:30). Mississippi has a Wales bug.
- Kazakhstan (240p, 2:22, lead 17:26): no Ambi verdict. Ambi asked to watch 0:26 to 0:36.
- Dam (lead, 14:34): gold cut passes its rule check. Three faults stay open. No full take.
- Tajikistan (rogun): written and cut by Juju. Not judged.
- Long films: a 20-minute picture timeline and a 14-minute Yellow River plan on paper. None made. Ambi's aim was 20-minute films by end of day, 2-minute tests only (17:05).
- Voices: casting is from the shelf only. ABV V9 cannot be spoken yet: no price or temperature set in the door script.
- Speed: render target 1.0 not reported as met.

## Web app and rooms
- Juju 0.2 presses (17:17): channel, style and title in three presses; four windows; "Juju picks" works with "any". Clicks at 1440x900 and 390x844 on the test copy. Not on the live server. No paid press run.
- Styles: Duppy Night, Duppy Day, Moko Dusk. Moko Day retired. Spiritual is a shut door.
- Not built: Send private, raise the cap from the app, films over 2 minutes, YouTube upload.
- App price button still says $0.60 a film. A 2-minute film is estimated at $0.10 to 0.18 (lead, 17:27). Not changed.
- Money can stop a film only in Story, Voice or Edit. Think's limit is 0.80 US (Tehuti, 17:30).
- Census (24 Nov): 573 controls; 112 real, 160 sample, 131 dead.
- Make-a-film room: 71 steps, 0 bad, on the practice copy (11:07). Not checked on a real film.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone. The emulator job (lead, 24 Nov 23:14): 19 checks pass, 3 fail. Paused; needs the Galaxy plugged in.
- Mac shell still bundles the old rooms (11:06). No release build. Not tested.
- The app's one tap still draws with the old engine. Lead says the app press uses one.sh. Not confirmed on a paid press.
- ADR 0022: Juju is map films only; the drawing engine is forked as Juju Maps. Making a film with the Mac closed is unresolved.
- Juju Maps has its own git repository. Its last commit is a merge from another project. A reset or checkout could overwrite files (16:12). Git stopped listing one file; cause not found.

## Agents running now
- The live agent page did not answer at 20:37. No transcript written in the last 10 minutes. Running agents are unknown.
- Last reports: worker 20:30 (building Juju's own router for the thinking seats); Tehuti 20:32 (two films churning; claimed).
- Reported done: map powers (17:31), data layers (17:46), motion ops (18:07), ranked study (18:43), coast fixes (20:23), voice shelf (19:55, 20:06), Neon routing (20:32).

## Money spent on services
- Ledger: 7,884 calls, $24.8961 in all.
- DeepSeek $3.3445 (4,110 answered, 17 refused or failed; last 20:37). OpenRouter $11.9351 (3,289, 45; last 20:36). Google $6.0613 (61, 13; last 20:37). Inworld $3.1317 (330, 1; last 20:35). WaveSpeed $0.288 (6, 2; last 11:24). Unsettled $0.1355 (7 failed).
- Cap: 30 US (Ambi's order, 19:30). About $5 left at 20:32.
- Neon rules (lead, 17:33): Google credit, at most $0.16 a film, otherwise GLM and DeepSeek. Neon off by default except the final script and idea pick. A planted-mistake test runs before each film; lead says it passes.
- Inworld voice is the largest production cost: $25 per million characters (Tehuti, 17:30).

## Broken, blocked or open
- GitHub billing blocks merge of seven pull requests (lead, 08:16). No later report. PR 26 has one failed check.
- Main has no new commit since 11:13. Juju Maps work is uncommitted.
- Data layers need a six-line patch and a restart of the Juju Maps server (17:46). Pre-fetch needs the same restart (19:38). Not confirmed.
- Rogun cut was overwritten (worker, 18:25). Restore written (Tehuti, 18:57). Not confirmed.
- Board7 line-29 fault is suspected, not confirmed fixed. The cutter crash was reported fixed (worker, 19:29).
- Night area curtain still glows at low wide views (Tehuti, 18:52). Lead decides.
- Voices: ABV V9 cannot be spoken. The mend script still voices from the old list at 1.04. Two channel voices are off the shelf.
- Provinces need an admin-1 file not on disk. The fire layer is missing (vector only).
- Near-shore detail is about 600 m; a Pontchartrain causeway is gone; a thin spit is broken.
- Lagoon speckle at Burullus and Manzala; blurred ground under Cairo.
- Silent-film bed about -37 LUFS. No listener has heard the beds.
- Sound on main sets aside too little per call (lead, 08:06). The Kazakhstan film has no sound effects.
- Library test failed at 08:37; cause not reported.
- Not proven: a voiced film over 10 minutes; a 20-minute film; anything on a phone; a Neon cache hit; the 95 of 100 taste bar; flat fills and solid lines on a whole film; the 0.4 s wipe-out.

## Waiting on Ambi
1. Choose a voice from five auditioned (Gavin, Tonya, Russell, Marek, Kristen).
2. Watch the Po film, "The delta that engineered itself under".
3. Watch Kazakhstan from 0:26 to 0:36 and say whether the sea falling feels real.
4. Judge the Juju Maps films: Kazakhstan, Caspian, Mekong, dam4 and Yellow River. Judge the ring and lights on Jenny.
5. Judge the Tajikistan film once drawn.
6. Judge the clip2 motion test and the ten map ops (18:07).
7. Decide the 0.2 questions: raise the cap from the app, length per channel, and where niches go.
8. Fix GitHub billing so the seven pull requests can merge.
9. Plug in the Galaxy.











# Sheet of 18:36 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 16:34 to 18:36 EAT, Wed 25 Nov 2026. Current time: 18:36.
- Spend rose from $16.1197 to $19.5198 over 6,639 to 7,001 paid calls. DeepSeek +$0.2432, OpenRouter +$1.5962, Google +$1.1134, Inworld +$0.2662, WaveSpeed +$0.09.
- Lead: spent "$18.99 of $20" at 17:33. Cap still 20 US (16:02, reported). Lead says it is not raised past 20. The ledger shows 19.52 at 18:36.
- Lead (17:25): Gemini was going through OpenRouter and the cache was not used. Corrected: Neon now on Google credit, off by default. Lead (17:33): Neon gave no cache hit in 9 paid tries. Nothing may depend on a Neon cache.
- Finish check: 1 of 23 clauses true, unchanged.
- Pull requests: 7 open, 19 merged, 1 closed. Unchanged. Main's newest commit is still 11:13.
- Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD. Unchanged. No new `juju make` film run appears in FACTS.
- Rust: 34,793 lines (was 34,781). Skills 56, rooms 20, decisions 20, APK files 0.
- Logged attempts: 283 kept, 41 reverted, 48 inconclusive (was 272, 40, 48).
- Mac load (1, 5, 15 min): 27, 14, 19 (was 7, 13, 21).
- Ambi's rulings since 16:34, as relayed: "videos are tools, Juju picks its own ideas" (16:02); "I really hate Moko Day ... only one polygon" (17:02), Moko Day retired; Moko is dusk only; Juju picks the look with "any" (17:17). Ambi asked for 20-minute films by end of day, 2-minute tests only (17:05). Ambi: Neon must use the Google AI Studio credit; OpenRouter for GLM and Jev (17:20).
- Built since 16:34 (reported by workers): Juju Maps mark set (sea cut, seamount, people, pillars, detour, borders); ten river and ground acts; a 20-minute picture timeline on paper; Juju 0.2 presses with four windows; a cheap board cutter (board7, about 9 cents and 90 s for 2 minutes); relief, profile, glide, river name and spot tools; eleven data layers and real satellite years; ten map motion ops plus a credit line; a ranked-film maker. Lead: Kazakhstan film (240p, 2:22) and Tajikistan film in progress.

## What worked and what failed
**Worked** (as reported; judged where stated)
- Juju 0.2 presses: channel, style and title take 3 presses to a playing film, on web and phone sizes (clicks on test server, 15:42, 16:44, 17:17). A Juju-picks press ran the real one.sh on copied test data at zero cost and came back Ready and played (17:17). No paid press run.
- Juju cut the Yellow River map film for about 9 cents in about 90 seconds, down from 35 (worker, 16:26 and 17:05; not judged for quality).
- Kazakhstan sea fall (lead, 17:26): the Aral Sea falls along its true shoreline. Lead's own judgment: the film is "above for you to judge". No verdict from Ambi.
- Juju Maps marks and river acts: under 2 ms a frame each, seeks identical. Judged by builder from stills only.
- Five relief, profile, glide, river name and spot tools: seek equals step, 0.000 to 0.001 difference. Judged by stills only.
- Eleven data layers and real satellite years: Aral 2000 to 2024, Dead Sea 1985 to 2021, drawn and checked by eye in stills (day and night).
- Ten map motion ops and a credit line: drawn at 480p, day and night, stills checked by builder. Nothing committed.
- Dance check on ground: worst second fell from 12.15% to 2.42% (worker, 18:09).
- Ranked-film maker: first ranked film had ten fault lines and a real order, for one cent (lead, 18:21). Judged by the lead.
- Lead's cost plan: a 2-minute test film about $0.10 (script $0.01, cut $0.01 to 0.03, voice $0.06). Estimate.

**Failed or refused**
- Ambi: "I really hate Moko Day ... only one polygon". Moko Day retired (17:02, relayed). Refused.
- Ambi on the Jenny cut (16:12): "I don't understand the ring" and "what's with all the lights". Ring and lights are the hero op; marks built to replace them, not yet judged.
- Ambi's older refusals still hold: stand-in drawings, the "slop" script line, the dot strip, the 36-palette sheet, parchment.
- Ambi: Neon must use the Google AI Studio credit, not OpenRouter (17:20). Rewired (lead, 17:33).
- Neon cache: nine paid tries gave zero cached tokens. The lead states the cheaper price does not come from a Neon cache.
- Rogun film (17:05, lead's own review): feed 7.3 against real 11.7. Not drawn.
- Lead's own Moko fault list (17:26): no sound effects in the Kazakhstan, Caspian, Mekong or dam films yet; red port cranes too big; "950" shows before the water falls; 1:39 to 1:48 still; soft ground close up; voice says "wildlife" over plain water.
- The Rogun cut was overwritten by a newer cut for Duppy with no cast (worker, 18:25). Recovery not confirmed.
- Ranked-film scripts coming out with real personality (lead, 18:34); tightening length. Not judged.

## App engine and films
- Juju make: newest DONE is still strip-japan (60 s, 08:34). Unchanged in FACTS.
- Yellow River film, "Duppy Day", 240p, 2:17 (last sheet). Not judged by Ambi.
- Moko Dusk Kazakhstan, "Why Kazakhstan Got Its Sea Back and Uzbekistan Did Not", 240p, 2:22 (lead, 17:26). Idea, title, sources, script and cut by Juju. Lead's faults listed above. No sound effects. Ambi asked to watch 0:26 to 0:36.
- Tajikistan film (rogun): written, voiced and cut by Juju per lead (17:27, 18:21). Not drawn with the new powers when last reported. Feed 7.3 against 11.7 (17:05). Pending Ambi's judgment.
- Juju Maps takes: Kivu take 4 best (Ambi 15:36, relayed). Dam4 Moko Dusk: "10 out of 10" (Ambi, 17:05, relayed). Jenny: Ambi's ring and lights faults (16:12).
- Long films: 20-minute picture timeline on paper (film20.json, 174 acts dark, 165 day; 26 stations). Not boarded or drawn. A 14-minute Yellow River plan on paper (films/yellow20). The 20-minute Yellow River is 13.9 min on paper; the truth check trimmed the script to 1,742 words, needs more sources (16:59). Lead (17:05) says aim is 20-minute films by the end of the day.
- Speed: board7 cuts 2 minutes in 90 seconds at about 9 cents. Render speed target 1.0 not reported as met.
- Voice: Graham and Winston blacklisted for the Kazakhstan and dam films (lead, 17:39). Auditioning 12 others on hard names. No choice recorded.
- Lead: Graham is the same voice as Lake Kivu.
- Moko runs: a worker reports Moko runs on port 4731 with a finished take showing as watchable (worker, 16:xx).

## Web app and rooms
- Juju 0.2 presses (15:04 build, 17:17 update): channel, style, title in 3 presses; four windows; "Juju picks" works with "any" look. Clicks at 1440x900 and 390x844 on test port 4702. Not on the live server 4700.
- Styles on 0.2: Duppy Night, Duppy Day, Moko Dusk. Moko Day retired. Spiritual is a shut door.
- Not built: Send private, Raise cap from app, films over 2 minutes. No YouTube upload code exists.
- App price button still says $0.60 a film, set before rewiring (lead, 17:27). A 2-minute film now costs about $0.10 to 0.18 (lead's estimate). Not changed.
- Money can stop a film only in Story, Voice or Edit. Think's limit is 0.80 US (17:30, lead). App showed $1.21 left at 15:55. Lead (17:16 worker): cap had about $1.43 left, about two films at 0.60 US (estimate).
- Census (24 Nov): 573 controls; 112 real, 160 sample, 131 dead.
- Make-a-film room: 71 steps on web and phone, 0 bad, on the practice copy (11:07). Not checked on a real film.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone. The phone job ran on an emulator only (24 Nov, 23:14): 19 checks pass, 3 fail. Paused; needs the Galaxy plugged in.
- Mac shell still bundles the old rooms (11:06). No release build. Not tested.
- The app's one tap still draws with the old engine; no code calls Juju Maps (14:20). Lead (17:27): the app press uses one.sh. Not confirmed on a paid press.
- ADR 0022: Juju is map films only; the drawing engine is forked as Juju Maps. Making a film with the Mac closed is unresolved.
- The Juju Maps folder has its own git repository. Its last commit is a merge from another project. A worker warns a reset or checkout could overwrite files (16:12). Git stopped listing juju-maps/gl.js in status (16:12); cause not found.

## Agents running now
- The live agent page did not answer at 18:36. Transcripts written in the last 10 minutes: 0. Running agents unknown.
- Recently active by report: map-powers lane (relief, glide, river name, spot) finished 17:31; data lane finished 17:44 and 18:06; ten motion ops 18:06 to 18:07; worker lane maps-data; ground lane (dance, text timeline, arc, device list) 18:35; Tehuti lane for Juju 0.2 presses and cutter (17:17); lead lane for cutter, ranked-film maker, pocket writer, description step (18:34).
- Lead's 17:27 note: relief and travelling camera and real years are still running; the Tajikistan film gets drawn when they finish. Lead at 18:21 and 18:34: Tajikistan voice and cut started; three new films written side by side.

## Money spent on services
- Ledger: 7,001 calls, $19.5198. DeepSeek $2.7255; OpenRouter $11.1859; Google $3.6588; Inworld $1.5261; WaveSpeed $0.288; unsettled $0.1355.
- Answered: DeepSeek 3,529 (13 refused); OpenRouter 3,169 (45); Google 38 (13); Inworld 175 (1); WaveSpeed 6 (2).
- Cap: 20 US (16:02, reported). Lead's last figure: $18.99 of $20 (17:33). Ledger now 19.52.
- Neon rules (lead, 17:33): Neon on Google credit, at most $0.16 a film, otherwise GLM and DeepSeek. Neon off by default except for speaking the final script and picking the idea. A test with planted mistakes runs before each film; lead says it passes.

## Broken, blocked or open
- GitHub billing blocks merge of seven pull requests (lead, 08:16). No later report. Pull request 26 shows one failed check.
- Main has no new commit since 11:13. Juju Maps work is uncommitted.
- board7 crashed on every film from 16:59 to 17:17 (board6 line 29 single braces in an f-string). Fix suspected, not confirmed. The lead's cutter crash was fixed (17:27).
- Rift take 3 broken by a full disk (14:10). Disk: lead says 2.2 GB (17:16); 24 GB free after a film download (18:09).
- Library test failed at 08:37, cause not reported.
- Juju Maps: the lead's ring and lights faults (16:27) are not confirmed fixed. Terra not rendered (12:14).
- Aral and Dead Sea data layers: the film.js patch (6 lines) is not applied as of 17:44; the lead must apply it and restart 4720 and 4721. Lead says 18:xx the ops are in; not confirmed.
- Border layers not proven: ottoman2 has no ops and fails to load (worker, 17:45).
- Provinces need an admin-1 file not on this disk.
- Fire layers only as vector tiles; GIBS fire layer missing.
- Blurred ground under Cairo; lagoon speckle at Burullus and Manzala; sea ice ragged edge.
- Silent-film bed near -37 LUFS; music beds about 14 dB under voice. No listener has heard them.
- Sound on main sets aside too little per call (lead, 08:06). Kazakhstan film has no sound effects.
- Not proven: a voiced film over ten minutes; a 20-minute film; anything on a phone; a Neon cache hit; the 95 of 100 taste bar.

## Waiting on Ambi
1. Fix GitHub billing so the seven pull requests can merge.
2. Choose the voice: Graham and Winston are blacklisted; pick from the 12 auditions.
3. Watch the Kazakhstan film from 0:26 to 0:36 and say if the sea falling feels real (lead, 17:27).
4. Judge the Juju Maps films: Kazakhstan, Caspian, Mekong, dam4, and the Yellow River. Judge the ring and lights fix on Jenny.
5. Judge the clip2 motion test (18:06); the Juju Maps taste on the ten map ops.
6. Decide whether films that go out use Neon for the script (lead, 17:27); the lead has since set Neon on for the final script only.
7. Plug in the Galaxy.
8. Decide the 0.2 questions: raise the cap from the app, length per channel, and where niches go.












# Sheet of 16:34 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 14:31 to 16:34 EAT, Wed 25 Nov 2026. Current time: 16:34.
- Spend rose from $9.9000 to $16.1197 over 6,384 to 6,639 paid calls. OpenRouter rose $4.53 and Google $1.34.
- Cap: Ambi raised the test cap to 20 US, with 25 as the hard most (Tehuti, 16:02, reported; the message is cut off). It was 15 US at 13:55.
- Finish check: 1 of 23 clauses true, down from 2. The lead has not reported which clause fell.
- Mac load (1, 5, 15 min): 7, 13, 21 (was 77, 71, 80).
- Logged attempts: 272 kept, 40 reverted, 48 inconclusive (was 255, 39, 47). Rust: 34,781 lines (was 34,532).
- Unchanged: 7 pull requests open, 19 merged, 1 closed. Main's newest commit is still 11:13. Whole-film runs: 4 DONE, 4 FAILED, 24 HOLD. Skills 56, rooms 20, decisions 20, APK files 0.
- Ambi's rulings since 14:31, as relayed: "videos are tools, Juju picks its own ideas" (16:02); "ideate before boarding; annotation is not thought"; Tanganyika was drawn on the wrong side (14:35).
- Built since 14:31, by workers, reported: Juju Maps marks (sea cut, seamount, people, pillars, detour, borders); ten river and ground acts; a 20-minute timeline on paper; Juju 0.2 presses on a test server; a Yellow River film named Duppy Day.

## What worked and what failed
**Worked** (as reported; judged where stated)
- Kivu dark cut (kivu2/d). Ambi: "This video so far is the best... one mind so beautiful, lets keep on this path" (15:36, relayed).
- Juju cut its own map film for 9 cents in 90 seconds, down from 35 (worker, 16:26). Not judged for quality.
- Juju 0.2 presses: channel, style and title take 3 presses to a playing film. Verified by clicks on a test server (15:42).
- Moko and Duppy systems: 30 of 30 test sentences right after mending; 30 of 45 unseen right on first runs (Tehuti, 14:32, measured on tests).
- Juju Maps marks and river acts: under 2 ms a frame each; seeks identical. Judged by the builder from stills only.

**Failed or refused**
- Ambi on Moko r1: "slop... everything is random" (25 Nov, relayed 15:42). Refused.
- Ambi refused the parchment look (ADR 0022: "I hate parchment paper").
- Ambi on the Jenny cut: "I don't understand the ring" and "what's with all the lights" (15:42).
- Ambi's older refusals still hold: stand-in drawings ("garbage", ADR 0012), the "slop" script line, the dot strip ("worst looking thing"), and the 36-palette sheet ("2017").
- Ottoman take 1 was set aside (review, 11:40).
- Dam low-poly rough 1: worker reports dam and farm too far, muddy dusk, dead hold at 1:15 to 1:24 (14:20). Not judged by Ambi.
- Low-poly Egypt clip: not proven; clip fix not drawn (15:12).

## App engine and films
- Juju make: newest DONE is strip-japan (60 s, 08:34). strip-mughal reached DONE at 16 minutes with faults open (lead, 08:44). Juju Maps films are not in this count.
- Juju Maps takes: Ottoman 1:58 with the obsidian look only (12:14); Kivu, Jenny, and dam4 in the Moko Dusk look sent to Ambi. No verdict on dam4.
- Yellow River, "Duppy Day", 240p, 2:17. Worker reports the idea, title, 31 sources, script, voice, cut, sound and picture were made by Juju. Worker fixed engine rules only. Worker's visible faults: China's flag shows with no border (rule added); "50 years" touches the bank; near ground in daylight is soft; the last view needs one changed picture. Not judged by Ambi.
- Long films: a 20-minute slot sheet with 73 sets and 2,929 words (15:50). A picture timeline with 11 parts, 74 views, 26 stations, 20.7 minutes (estimated). Written only, not run through a writer, boarded or drawn. A 20-minute Yellow River is being written on paper, no voice (16:31).
- Ten river and ground acts (perch to saltcreep) and five marks: stills only, no moving clip, no blind viewer. No lead film uses them yet.
- Speed: 2.3 machine seconds per film second under load (10:12). Target 1.0 not met.
- Voice: Graham or Winston. No answer recorded.
- Moko run: stopped at 16:33 when the script was edited and crashed; the worker says it is running again.

## Web app and rooms
- Make-a-film room: 71 steps on web and phone, 0 bad, on the practice copy (11:07). It links to make. Not checked on a real film.
- Live app: answers after restart (11:40). Not reported since.
- Juju 0.2 prototype (15:04): 60 screens, 0 faults in the build check. Styles: Duppy Night, Moko Day, Moko Dusk; Spiritual is a shut door. Not built: Send private, lengths over 2 minutes, Raise cap. No YouTube upload code exists.
- Money can stop a film only in Story, Voice or Edit. Think's limit is fixed at 2.00 US in two scripts. The app showed $1.21 left at 15:55. A film costs about 0.27 US (estimate).
- Census (24 Nov): 573 controls; 112 real, 160 sample, 131 dead.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone. The phone job ran on an emulator only (24 Nov, 23:14): 19 checks pass, 3 fail. Paused; needs the Galaxy plugged in.
- Mac shell still bundles the old rooms (11:06). No release build. Not tested.
- The app's one tap still draws with the old engine; no code calls Juju Maps (14:20).
- ADR 0022: Juju is map films only; the drawing engine is forked as Juju Maps. Making a film with the Mac closed is unresolved.
- The Juju Maps folder has its own git repository. Its last commit is a merge from another project. The worker did not make it and warns that a reset or checkout could overwrite files (16:12).

## Agents running now
- The live agent page did not answer at 16:34. Transcripts written in the last 10 minutes: 0. The worker's 16:33 message says Moko is running, so the true count is unknown.
- Recently active by report: worker lanes from 16:11 to 16:33 (Juju Maps marks, river acts, the 20-minute timeline, Yellow River, the cheap cutter, Moko). Tehuti, last at 16:27.
- Mungura: last report 12:14. Lead: last report 08:37, a library test failing. No later lead report.

## Money spent on services
- Ledger: 6,639 calls, $16.1197. DeepSeek $2.4823; OpenRouter $9.5897; Google $2.4544; Inworld $1.2599; WaveSpeed $0.198; unsettled $0.1355.
- Answered: DeepSeek 3,284 (13 refused); OpenRouter 3,100 (45); Google 23 (7); Inworld 150 (1); WaveSpeed 6 (0).
- Cap: 20 US (16:02, reported). It was 15 US; spend passed 15 before the raise.

## Broken, blocked or open
- GitHub billing blocks merge of seven pull requests (lead, 08:16). No later report. Pull request 26 shows one failed check.
- Main has no new commit. Juju Maps work is uncommitted. The worker reports a Juju Maps file missing from git status and no cause found (16:12).
- Library test failed at 08:37, cause not reported. 61 tests passed at 07:58.
- Juju Maps: terra not rendered (12:14). The two lead faults on the ring and the lamps were raised at 16:27; the fixes are not confirmed.
- Rift take 3 broken by a full disk (14:10).
- Eight packs have a trigger with no row in the reach table (14:21). Subtitle conflict with ADR 0014 item 4 (14:21).
- Silent-film bed near -37 LUFS; a 1.28 s hush rule awaits a ruling. Music beds are about 14 dB under voice (11:10). No listener has heard them.
- Sound on main sets aside too little per call (lead, 08:06).
- Not proven: a voiced film over ten minutes; a 20-minute film; anything on a phone; the 95 of 100 taste bar.

## Waiting on Ambi
1. Fix GitHub billing so the seven pull requests can merge.
2. Choose the voice: Graham or Winston.
3. Rule on the silent-film bed level, the 1.28 s hush and the subtitle question.
4. Countersign the new music bars (11:11) and the pins for veve-gait, opon-sight and nyansapo-ladder (14:21).
5. Judge the Juju Maps films: Kivu, Jenny, dam4 and Yellow River. Pick the look. Judge the Ottoman voice and pictures.
6. Answer whether a film always finishes (10:50).
7. Plug in the Galaxy.
8. Decide the 0.2 questions: raise the cap from the app, length per channel, and where niches go.













# Sheet of 14:31 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 12:29 to 14:31 EAT, Wed 25 Nov 2026. Current time of this sheet: 14:31 EAT.
- Scope is map films only (ADR 0022, Mungura, 12:04). Ambi: "do this one niche really well", "I hate parchment paper", "having hard gates prevents a vid from rendering". Juju Maps is forked from an MIT project. Checks report; only the money cap, an unsourced sentence, picture rights and Ambi's publish clicks stop a render (lead's reading of ADR 0022).
- Ambi (about 13:51, relayed by Tehuti): dark take 2 "really good ... actually felt like I was learning"; spoken place must be in view. Ambi (about 13:55, relayed): upgrade skills and docs to the map stack. Ambi gave 7.5 of 10 on the Kivu cut (Tehuti, 14:10, reported).
- Money cap set to 15 US (Tehuti, about 13:55, reported in runs/meter/cap.json). Spend was 9.45 of 9.50 at 13:51 (reported).
- Paid calls: 6,384, $9.9000 (was 6,135, $8.8670). DeepSeek $2.3606, OpenRouter $5.0640, Inworld $1.0254.
- Mac load (1, 5, 15 min): 77, 71, 80 (was 4, 6, 9). Tehuti (13:51) reported load over 100 with nine agents. Disk and memory tight.
- Rust: 34,532 lines, unchanged. Skills: 56 (was 52). Rooms: 20. Decisions: 20. Logged attempts: 255 kept, 39 reverted, 47 inconclusive.
- Pull requests: 7 open, 19 merged, 1 closed (unchanged). Main has no new commit since 4dba4d9 (11:13).
- Finish check: still 2 of 23 clauses true.
- Whole-film runs on disk: 4 DONE, 4 FAILED, 24 HOLD (unchanged).
- Lead's last report: 08:37, a library test failing. Lead's 08:32 message: otto-chron-3 held at Outline (a cut before "of" made a false line). Not reported fixed.

## What worked and what failed
**Worked** (as reported; no one has judged all of it good)
- Juju Maps first take (Mungura, 12:14): 854×480, -15.1 LUFS, picture cards, no blank tiles in frames checked. Look test only.
- Kivu lake film: Ambi 7.5 of 10 (reported, 14:10). Tehuti: the Juju Motion timing is what would lift it further.
- Kivu agent cut (low-effort editor taught by veve-gait) reported as better than the cheap model's own cut (Tehuti, 14:10).
- Map-cut structure in code, one small form per view (board4, 14:10). Reported; Juju cut its own film for under a cent (reported, not judged).
- Moko and Duppy systems: 30 of 30 test sentences match the first answers (after mending); 30 of 45 unseen sentences right on first runs (Tehuti, 14:32). Measured on tests; no film boarded from it.
- Dark look: Ambi kept it (13:51, relayed).

**Failed**
- Ottoman take 1 (voiced, full music): flat delivery, treaty stretch, 1908 ending, thumbnail word, empty Paris map at 8:00 (review, 11:40). Set aside.
- proof12 (voiced, 12 min asked): first draft 1,483 words, cut to 800 by Juju's checks. Cost $0.46 (Mungura, 09:28).
- 25 of 29 ended runs were stopped by Juju's own checks (Mungura, 10:50). ADR 0022 changes these stop rules.
- Picture search gave people for bare country names, black-and-white copies, upside-down tiles (11:36 to 12:08). Fixes reported; not rechecked.
- Ambi refused the parchment look (ADR 0022).
- Lead's 08:32 film otto-chron-3: a line cut before "of" read false; stopped by the lead.

## App engine and films
- Whole runs: 4 DONE, 4 FAILED, 24 HOLD. Newest DONE: strip-japan (60 s, 08:34). strip-mughal DONE at 16 min with faults open (lead, 08:44).
- otto-chron-2: silent 60 s, Juju's own dated lines, -14.9 LUFS, DONE (lead, 07:39). Lead's own faults: counter wrong for about 1.5 s on each long flight; "every line is small".
- Juju Maps: Ottoman 1:58 take, obsidian only; terra not rendered (12:14). No verdict on voice, look or pictures.
- Kivu take (Juju's script, 240p plan): Juju Maps film. Seven open items: names ("Rusizi" not "Ruzizi"), a year and place out of view, boats, sensors, two lakes by size, 1,700 counter still counting at 90 s, Nyiragongo label on Karisimbi (worker, 11:26-era handoff; logged 13:51).
- Dam low-poly film: rough 1 (110 s, voice and sound in, dusk look). Worker reports the dam and farm too far away, muddy dusk, pictures name things instead of showing them, a dead hold at 1:15 to 1:24 (14:20). Not judged by Ambi.
- Dark look: kivu-machine and agent cuts drawing (14:10, 14:20). Status not reported after.
- Lowpoly recipes: 17 recipes, check passes (3 of 3 planted faults caught, Measured, 14:24). Eight scenes not watched moving.
- Engine notes: Moko default 0.10 of span where 0.19 is the floor; board never writes cutact (worker, 14:32).
- Voice: TTS-2 in use. Two samples await Ambi's choice; no answer recorded.
- Speed: 2.3 machine seconds per film second under load (10:12). Target 1.0 not met.
- Harvest: 11 of 12 films have notes (older report).

## Web app and rooms
- Make-a-film room finished (Tehuti, 11:07). Walks 71 steps each, web and phone, 0 bad, on the practice copy. Altar, Cauldron and Pact run through it.
- Live app on 4701 restarted; film room answers (11:40). Port 4700 needed a restart (11:07).
- Film room tested on a silent film only. Lengths 30 and 50 and voice checked only by a test list.
- Pinned programs are from 08:24. Not reported new.
- Not pressed since 24 Nov: five cards are placeholders; Mirror Bend and Feed Sight show broken pictures.
- Census (24 Nov 20:00): 573 controls; 112 real, 160 sample, 131 dead.
- Make-a-film button: Tehuti (08:53) said it still makes practice clips. Tehuti (11:07) says it now links to make. Newer report: links to make, unverified on a real film.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone.
- Phone job: emulator run (lead, 24 Nov 23:14): 19 checks pass, 3 fail. Paused. Needs the Galaxy plugged in.
- Phone walks are a browser at phone size, not an installed app.
- Mac shell still bundles the old rooms (11:06). No release build reported. Not tested.
- The app's one tap still draws with juju-stage; no code in crates or apps calls juju-maps (worker, 14:20).

## Agents running now
- Live agent page did not answer. Running agents: unknown.
- Recently active (reports): Tehuti (Claude, 14:10 to 14:32, map films, docs and systems); Mungura (read only, 12:14); worker lanes on lowpoly recipes, dam film, Moko and Duppy pick systems (14:20 to 14:32); kivu-machine and agent cuts drawing (14:10 to 14:20).
- Lead: last report 08:37, a library test failing. No later lead report.

## Money spent on services
- Ledger: 6,384 calls, $9.9000. DeepSeek $2.3606, OpenRouter $5.0640, Google $1.1165, Inworld $1.0254, WaveSpeed $0.198, unsettled $0.1355.
- Answered: DeepSeek 3,159 (13 refused); OpenRouter 3,001 (45); Google 15 (7); Inworld 127 (1); WaveSpeed 6 (0).
- Cap: 15 US (Ambi, about 13:55, reported). Was 9.50 US; 9.45 spent at 13:51 (Tehuti, reported).
- Cost of Juju Maps take: not reported. Juju cut for under a cent (Tehuti, 14:10, reported).

## Broken, blocked or open
- GitHub billing blocks merge of seven pull requests (21 to 27 open). Lead, 08:16; no later report. Ambi must fix billing.
- Commits: 11:13 on main is not reported pushed. Tehuti pushed the context repo by hand (08:53); the Juju code push is not reported.
- Juju Maps: terra not rendered. Files untracked; no commit, no push remote (12:14). Not tested: a 30-minute film. Mac-closed film production unresolved (ADR 0022).
- Rift take 3 broken by a full disk; redraw when Mac is quiet (14:10).
- Eight packs have a `when` with no row in reach.rs (14:21). Not run.
- Subtitle conflict: the engine draws one; ADR 0014 item 4 says none (14:21).
- Silent-film bed near -37 LUFS; 1.28 s hush rule awaits a ruling. Music bed about 18 dB under voice outside night look (worker, computed from mix.py, Estimated; grammar says 30).
- Tests: 61 passing (lead, 07:58); final full run unconfirmed (08:44). Library test failed 08:37, cause not reported.
- Sound on main sets aside too little money per call (lead, 08:06). No later report.
- Not proven: a voiced film over ten minutes; anything on a phone; the 95 of 100 taste bar.

## Waiting on Ambi
1. Fix GitHub billing so the seven pull requests can merge.
2. Choose the voice: "Graham" or "Winston". No answer recorded.
3. Rule on the silent-film bed level, the 1.28 s hush, and the subtitle question (ADR 0014 item 4).
4. Countersign new music bars (11:11), LINE-RULE 7 to 20, and the veve-gait, opon-sight and nyansapo-ladder pins (worker, 14:21).
5. Juju Maps: judge the kivu take and the dam film, pick the look, judge the pictures and voice of the Ottoman take. No verdict yet on terra.
6. Answer whether a film always finishes (Mungura, 10:50; Tehuti, 10:51). No answer recorded.
7. Plug in the Galaxy for the phone job.














# Sheet of 12:29 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 10:27 to 12:29 EAT, Wed 25 Nov 2026.
- **Scope cut to maps (ADR 0022, recorded by Mungura, 12:04).** Ambi decided Juju makes map films only: empires, wars and borders. The record quotes him: "do this one niche really well", "I hate parchment paper", "having hard gates prevents a vid from rendering". The map engine is forked as Juju Maps from an MIT open project. Checks now report. Only the money cap, an unsourced sentence, picture rights and Ambi's publish clicks stop a render. This replaces the HOLD rule for these films.
- Ambi's single-builder order (09:47) still stands.
- Paid calls: 6,135, $8.8670 (was 6,029, $8.0822).
- Mac load (1, 5, 15 min): 4, 6, 9 (was 14, 14, 17). 0 agent transcripts in the 10 minutes before 12:29.
- Whole-film runs on disk: 4 DONE, 4 FAILED, 24 HOLD. New: ottoman12f HOLD 11:25, stopped at Pictures and form.
- Main has a new commit, 4dba4d9 (11:13): app from press to watched film, music bed, export settings, closing-line check.
- Juju Maps first take, 1 minute 58 seconds, 480p (12:14).
- Make-a-film room walked (11:05). Live app restarted (11:40 log).
- Rust: 34,532 lines (was 33,969). Decisions: 20 (was 19). Logged attempts: 246 kept, 35 reverted, 47 inconclusive.
- Finish check: still 2 of 23 clauses true.

## What worked and what failed
**Worked** (as reported; no one has judged any of it good)
- Make-a-film room: subject or pasted link, look, silent or voice, length, one action. Web and phone walks, 71 steps each, 0 bad. A kept silent film plays to the end (worker, 11:05).
- Music beds: the proof75a and Pluto copies pass with the bed heard. 46 of 46 sound tests pass (worker, 11:11). No person has listened.
- Script quotes: 148 sentences each matched to an exact quote (builder, 09:46).
- Export: a 12-minute film projects to about 390 MB, down from 1.9 GB (builder, 10:35, estimate).
- Juju Maps take 1 (12:14): 854×480, -15.1 LUFS, picture cards with no blank tiles in the frames checked. Its maker calls it a look test.

**Failed**
- proof12 (voiced, 12 minutes asked): first draft 1,483 words, cut to 800 by Juju's own checks. Cost $0.46 and 353 s (Mungura, 09:28).
- Mungura's comparison: VerseBatch wrote 10 scripts averaging 6,905 words in 55 minutes. Juju wrote no usable script. This is Mungura's reading.
- Of 29 ended runs, 25 were stopped by Juju's own checks (Mungura, 10:50). This is why ADR 0022 changes the stop rules.
- ottoman12f take 1, full voice and music. A video model reviewed it (11:40): flat delivery, a treaty stretch, a 1908 ending, a thumbnail word, an empty Paris map at 8:00. Take 1 was set aside.
- Picture search: bare country names gave people (Venice gave a doge, Russia gave Nicholas II), black-and-white copies, every tile upside down (11:36 to 12:08). Fixes reported; not rechecked.
- Ambi's refusal, as recorded in ADR 0022: the parchment look is refused.

## App engine and films
- Whole runs: 4 DONE, 4 FAILED, 24 HOLD. Take 2 of Ottoman was drawing at 11:40. No result reported.
- DONE, as reported: otto-chron-2 (silent, 60 s, Juju's own dated lines, -14.9 LUFS; lead, 08:32). strip-japan (60 s, facts only; no look judged; 08:34). strip-mughal (16 min, faults open; lead, 08:44 log).
- Voice: TTS-2 in use. Two samples await Ambi's choice. Without an answer the builder uses Graham (10:03).
- Stops: a 0.30 US voice limit is in code (10:35). The price test was set to 0.30 (worker, 11:06, asks for confirmation).
- Script: Ottoman draft about 1,750 words (builder, 10:35). Make still does not link to the 52 skills (10:02). No fix is reported applied.
- Speed: 2.3 machine seconds per film second under load (builder, 10:12). Target 1.0 not met.
- Pictures: the engine draws 12 of the 40 picture moves in the 60 studied films (study, 03:39). The worker reports 19 search pictures (11:46), not reviewed.
- Juju Maps: only the obsidian look is rendered. Terra is not (12:14). No verdict from Ambi.
- Harvest: 11 of 12 films have notes (older report).

## Web app and rooms
- Make-a-film room finished. Altar, Cauldron and Pact run through it instead of dead-ending (11:05). Lengths 30 and 50 and voice were walked with a test list only.
- Film room: plays with sound to the end, chapters, thumbnail, download identical to the master (worker, Measured).
- Live app restarted; its film room answers (11:40 log).
- Pinned programs are from 08:24, before the voiced build. A new pin is due when a film passes (11:06).
- Not pressed since 24 Nov: five cards are placeholders; Mirror Bend and Feed Sight show broken pictures.
- Census (24 Nov 20:00): 573 controls; 112 real, 160 sample, 131 dead.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone.
- Phone job: emulator run (lead, 24 Nov 23:14) had 19 checks pass and 3 fail. Paused. Needs the Galaxy plugged in.
- Phone walks are a browser at phone size, not an installed app.
- Mac shell still bundles the old rooms (worker, 11:06). No release build reported. Not tested.

## Agents running now
- The live agent page did not answer. Running agents: unknown.
- Last reported: a worker (12:22 to 12:25) changed course to two short rough films and is writing Juju Motion, the on-map graphics, and scripts on real sources.
- Mungura made the Juju Maps take (12:14).
- Film room, sound and picture workers each reported finished, the picture fix at 12:08.
- Lead: last report 08:37, a library test failing. No later lead report.

## Money spent on services
- Ledger: 6,135 calls, $8.8670. DeepSeek $2.2314, OpenRouter $4.4468, Google $1.1165, Inworld $0.7389, WaveSpeed $0.198, unsettled $0.1355.
- Answered: DeepSeek 2,958 (13 refused); OpenRouter 2,981 (45); Google 15 (7); Inworld 99 (1); WaveSpeed 6 (0).
- Builder (11:40): 8.69 of 9.50 US cap spent. Film lane 0.482 of 0.50 (lead, 08:32). About $2.57 of test cap left (worker, 09:31). The ledger is the record.
- Cost of the Juju Maps take: not reported.

## Broken, blocked or open
- GitHub billing blocks the merge of seven pull requests (21 to 27 open). Lead, 08:16; no later report.
- The 11:13 commit on main is not reported pushed to GitHub.
- Sound: the watcher now reserves what the price gate charges (worker, 11:11). PR 26 not rechecked. Ambi said not to push to it (08:44).
- Silent-film music bed sits near -37 to -40 LUFS. The 1.28 s hush rule awaits a ruling.
- Missing prices: two models have none in main; PRs 24 and 25 refuse their calls (07:49). Not rechecked.
- Tests: 61 passing (lead, 07:58); final full run unconfirmed (08:44). One test did not run at head (11:07). Two older tests fail (10:01). A library test failed at 08:37.
- Juju Maps: terra not rendered. Files are untracked; no commit and no push remote (12:14). Not tested: a 30-minute film. How a film gets made with the Mac closed is unresolved (ADR 0022).
- Music: no person has listened. The player of Op. 18 No. 6 is inferred. A Naxos Bach cello and a Mussorgsky piece are refused on rights (worker, 11:11).
- Vault: LINE-RULE 7 to 20 await countersign (08:12).
- Not proven: a voiced film over ten minutes; Crossroads Chain on any film; anything on a phone.

## Waiting on Ambi
1. Fix GitHub billing so the seven pull requests can merge.
2. Choose the voice: "Graham" or "Winston". No answer is recorded.
3. Rule on the silent-film bed level and the 1.28 s hush.
4. Countersign the new music bars (11:11) and LINE-RULE 7 to 20.
5. Juju Maps: pick the look, and judge the two-minute take's pictures and voice. No verdict yet.
6. Watch Ottoman take 2 when it lands. Name the worst thing in it.
7. Who writes the scripts, and which pictures are allowed: no recorded answer. ADR 0022 covers scope and stop rules.
8. Plug in the Galaxy for the phone job.
9. A worker's check-in of 09:31 has no recorded reply.















# Sheet of 10:27 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 08:23 to 10:27 EAT, Wed 25 Nov 2026.
- Paid calls: 6,029 calls, $8.0822 in the ledger (was 5,825, $6.0073).
- Mac load (1, 5, 15 min): 14, 14, 17 (was 89, 84, 75). 0 agent transcripts written in the last 10 minutes.
- Ambi ruled: Juju only; the old Loop and Milarepa threads are out (10:02 log). He ordered single-builder mode, no swarms (09:47 log).
- Lead stopped otto-chron-3 himself at 08:32. Line 2 was cut before "of the Roman empire", which made it false. It is back at Outline.
- Finished runs: strip-japan DONE 08:34 (60 s, 0.008751 US). Whole-film runs on disk: 4 DONE, 4 FAILED, 23 HOLD.
- Newest runs: proof12c FAILED 09:47 (stopped at Render and mix); proof12 HOLD 09:16; proof75b HOLD 09:06; proof75a HOLD 08:59 (Publish kit); strip-planets HOLD 08:41; strip-pluto HOLD 08:40.
- Juju commits on this Mac's main: newest 04788e9 (10:12), then cbbffcb (09:46). The builder reports the work is committed here but not on GitHub.
- Rooms drawn: 20 (was 19). Rust: 33,969 lines in 14 crates (was 32,716).
- Logged attempts: 241 kept, 35 reverted, 47 inconclusive.
- Finish check: still 2 of 23 clauses true.

## What worked and what failed
**Worked** (as reported; no one has judged any of it good)
- otto-chron-2: DONE, silent, Juju's own lines, -14.9 LUFS, 0.0019 US (lead, 08:32).
- strip-japan: DONE (facts, 08:34). No judgement of its look is reported.
- First voiced 75 s film, proof75a: voice bought, 0.015 US, 4.6 minutes machine time (builder, 09:00). It stopped at the thumbnail check (0.69 against a 0.68 limit).
- The builder's first 60 s of the new Ottoman strip, reviewed by a video model: verdict "fix". Worst fault: about 10 s with nothing new on Constantinople (builder, 10:12). Still stillness went from 6.2 s to 2.2 s (builder, 10:02).
- Script quote check: 148 sentences each matched to an exact quote in a source (builder, 09:46).
- Date and map position alone found the event for 23 of 26 beats (builder, 10:06).

**Failed**
- proof12 (voiced, 12 min requested): first draft 1,483 words, cut to 800 by Juju's own checks. Spent 0.46 US and 353 s on one attempt (read-only audit by Mungura, 09:28, from the job files).
- Mungura's comparison: VerseBatch wrote 10 scripts averaging 6,905 words in 55 minutes (10 Oct). Juju wrote 0 usable scripts. This is Mungura's reading, not judged by Ambi.
- proof75b: the renderer's laws refused it (builder, 09:06). proof12c FAILED at Render and mix (facts, 09:47).
- Ambi on a sound run, 08:44: interrupted before any fix landed. Three sound asks remain open.

## App engine and films
- **Ottoman Empire, 9.5 min, 26 events, voiced:** the builder says the full film was drawn and rendered. No run for it appears in FACTS. The builder has not watched it whole. The builder reports it ends in 1908. A longer script with an ending is being written (10:12).
- **Voice:** the builder moved from the cheap "flash" voice to the real TTS-2. Two samples await Ambi's choice. Delivery was called flat by the video model.
- **Limits:** the builder removed the 0.30 US voice gate. No ruling by Ambi is recorded. The builder also says a test clip no longer blocks a real film's thumbnail.
- **Story skills:** 52 skills exist. `juju make` does not link to them. The 10:02 diagnosis says no fix was applied. Crossroads Chain is not tested on a real film.
- **Render speed:** about 2.3 machine seconds per film second while the Mac was busy (builder, 10:12). Target 1.0 not met.
- **Picture:** the engine draws 12 of the 40 picture moves in the 60 reference films (study, 03:39). The builder is adding painting cutaways (10:12). Not in the film yet.
- **Harvest:** 11 of 12 films have notes. The rest is not reported.
- **Day log, undated:** a draw check found 3 wrong of 100 in two subjects. Rules fixed. Fresh draws 0 wrong (judged).

## Web app and rooms
- Pressed 24 Nov 01:22: 61 screens. Gate, Altar, Crossroads, Cauldron, Pact, Conjuring, Spell Strip and Publish Kit work on the main path. The five cards are placeholders. Mirror Bend and Feed Sight show broken or empty pictures.
- "Make a film" still makes practice clips (log, 08:44). A builder is wiring the film path into the 10, 20, 30 and 50 minute choices (09:43). Not reported done.
- An earlier worker's rooms in the film path never landed (10:01).
- Census (24 Nov 20:00): 573 controls; 112 real, 160 sample, 131 dead.

## Mac app and APK
- APK files built: 0. Nothing has run on a phone.
- Phone job: an emulator run had 19 checks pass and 3 fail (lead, 24 Nov 23:14). Paused. Needs the Galaxy plugged in.
- Mac app: no release build reported. Not tested.

## Agents running now
- Live agent page did not answer. Running agents: unknown.
- Last reported, not confirmed live:
  - builder (10:12): three helpers, one per lane: app press-to-film path, a music bed, and painting cutaways. No film renders.
  - builder (10:15): auditioning space beds, then a `watch.py` fix.
  - a library test fails (lead, 08:37); no later report.
- Reviewers: all finished, last at 08:03.

## Money spent on services
- Ledger: $8.0822 over 6,029 calls. DeepSeek $2.1902, OpenRouter $4.3318, Google $0.834, Inworld $0.4198, WaveSpeed $0.171, unsettled $0.1355.
- Answered calls: DeepSeek 2,898 (13 refused); OpenRouter 2,949 (45); Google 14 (7); Inworld 87 (1); WaveSpeed 5 (0).
- Builder (10:12): 7.52 of 9.50 US spent. Lead: film lane 0.482 of 0.50 (08:32). Working limit 10.00 US (lead, earlier). The ledger is the record.

## Broken, blocked or open
- **GitHub billing blocks the merge** of seven pull requests (21 to 27 open). Nothing merged (lead, 08:16; no later report).
- **PR 26, sound:** the watcher reserves 0.000336 per call; main prices it at 0.001344; main refuses the call. Not reported fixed. Ambi said not to push to PR 26 (08:44).
- **PR 26** still holds two test frames pushed by mistake; they are Juju's own map film.
- **Two older tests fail** in files the builder has not touched (10:01).
- **Missing prices:** two models have no price in main; PRs 24 and 25 refuse their calls (07:49). Not rechecked.
- **Sound:** the 1.28 s hush rule on silent films awaits a ruling.
- **Vault:** LINE-RULE items 7 to 20 await countersign. No film made from a slot.
- **Pacing:** the Ottoman film is not watched whole. Its stillness and cutaway gaps are not yet measured after the cutaways.
- **Ending:** the Ottoman script stops at 1908; the longer ending is not written yet.
- **Not proven:** a voiced film over ten minutes; Crossroads Chain on any film; anything on a phone.

## Waiting on Ambi
1. **Fix GitHub billing** so the lead can merge the seven pull requests.
2. **Choose the voice:** say "Graham" or "Winston". Without an answer the builder uses Graham (10:03).
3. **Watch the first 100 seconds** of the Ottoman strip (10:01), then the full film when it is ready. Name the worst thing in it.
4. **Answer four questions** the builder put (scope, who writes, what may stop a film, pictures). Each has the builder's proposed "yes". No ruling by Ambi is recorded (Mungura, 09:28).
5. **Sound:** rule on the 1.28 s hush, and say whether the three sound fixes wait for the watcher fix.
6. **Plug in the Galaxy** for the phone job.
7. **Personal check-in:** a worker asked Ambi a personal question at 09:28 and 09:31. No reply is recorded.
















# Sheet of 08:23 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 08:18 to 08:23 EAT, Wed 25 Nov 2026.
- Paid calls: 5,825 calls, $6.0073 in the ledger (was 5,824, $6.0071). OpenRouter: 2,902 answered ok, last at 08:21.
- Mac load (1, 5, 15 min): 89, 84, 75 (was 87, 71, 69). Still rising.
- Agent transcripts written in the last 10 minutes: 7 (was 9).
- Worker, 08:21: the rebuilt Ottoman film is drawn. It is being checked against its rules, and looked at every 2 seconds. Not judged.
- Worker, 08:22: the main server pieces compile and the first unit tests pass. A playback stand-in has a fault, being found by hand.
- Still true from 08:16: GitHub is blocked, nothing is merged, seven pull requests are open. The Mughal film is finished.

## What worked and what failed
**Worked** (as reported; no one has judged any of it good)
- `juju make` produced three one-minute films with no test switch: otto-silent-2 (silent, 0.068 US), otto-chron-2 (words on the map, 0.001904 US), strip-mughal (from one typed sentence, 0.008507 US). The lead reports all three work and none is good.
- Mughal is the first subject Juju had never seen to reach a finished file.
- Vault review: 7 blocking faults, each red before the fix and green after. Simulation: 21,182 dealt, 238 refused, 0 faults on re-read (worker, 08:12). 54 tests.
- Title checks: 0 of 15 planted false titles pass, down from 15 of 15 (worker, 05:26).
- Film-harvest skill is in main (PR 20). Its self test scored 6 of 6, scored by its maker.
- Seven pull requests have CLEAN reviews: 23 from opus-ship-a (07:33), 21, 22 and 24 to 27 from opus-ship-c (08:03). These reviews check code and planted faults. They do not judge films.

**Failed**
- Ambi, 24 Nov 23:17, on the dot strip the lead had praised: "the worst looking thing ive ever seen." He asked for Juju's own house worlds.
- Ambi, 24 Nov 20:57, on the script line "the sun gave nothing": "What kind of slop is that?" The lead and two Claude listeners had praised it.
- Ambi, 24 Nov 13:51: stand-in drawings, "Both of them are garbage." Refused.
- Ambi, 24 Nov 13:54: the Jade Rabbit style. He said only Claude could make it, and the software runs on cheap models. Dropped.
- Ambi, 24 Nov 14:33, on a 36-palette sheet: "Just like some slideshows. 2017." Cut to 11.
- Of ten new subjects, nine have not reached a file: Japan, Pluto, Manchuria, Bulgaria, Austria, Jerusalem, Venice, Sweden, Space.
- Fast runner: about 1.2 times faster, not the 3 times target (lead, 04:15).
- Facts lane: 2 of 15 opened facts wrong, 6 pins misplaced (lead, 02:35). Later, two more bad pins: Sarai beside Baku, and Borodino in Siberia (lead, 04:30). Not reported fixed.
- Engine: draws 12 of 40 picture moves in the 60 reference films, and 0 of 20 skeleton and house pairs whole (study, 03:39).

## App engine and films
- **strip-mughal:** DONE, 60 s, finished 07:59. The lead watched one frame every 3 seconds (08:16). Mountains real, edges smooth, land lights as it changes hands. Still wrong: words too small for a phone; Mughal land first shows in 1539 though the film starts in 1525; it stops at 1659 though the idea said 1707; the line "But the Mughal Empire grew and took land" is weak.
- **otto-chron-2** (lead, 07:40): words tiny, coasts blocky, one colour on grey. "Belgrade was captured" shows at 1497. "Invaded Syria" sits on Istanbul.
- **otto-silent-2** (lead, 06:45): no words, stretches with no change, modern "now Turkey" labels, a doubtful area figure.
- **Rebuilt Ottoman film** (worker, 08:15): each line at its place after its year, readable, clean coasts, almost no inner borders. Being drawn at 08:21. Not judged by the lead.
- **Whole-film runs on disk:** 3 DONE, 3 FAILED, 19 HOLD. Newest: strip-bulgaria, strip-austria and strip-manchuria HOLD at 08:11 (stopped at Deal and package). strip-pluto HOLD at 08:08 (Render and mix). thru-mughal and otto-chron-3 HOLD at 08:06 (Pictures and form). strip-jerusalem FAILED at 07:36 (Script and heal). A worker reports both the Mughal and Ottoman forms legal at 08:10. The run list does not show that yet.
- **Sound:** silent film at -14.6 LUFS, 4 of 4 cues heard (worker). A 20-minute film took 912 s (worker, 05:43). Main sets aside too little money per call, so a film with no kept answer gets no sound. It fails closed (worker, 08:03).
- **Voice:** none in any real film. Nothing made at 10, 20, 30 or 50 minutes.
- **House strips:** Orion was refused by four judges (06:45). Egypt, Orion and lungs repaired at 08:05 (worker): check passes, 31 unit tests. Looks judged only by their maker. Render 7 to 19 seconds per film second at load 57 to 95; target 1.0 missed.
- **Harvest:** 11 of 12 films have notes (lead). Motion language: 64 of 64 truth rows expressible, held out on one film only. Our eye found 35 of 35 drawn events, rea-video 10 of 35, on the windows the eye was built on (03:41). The language measure gave 32 of 35 (05:18). No pack built, no blind rebuild.
- **Packaging:** 9 frames, 45 bends. Check passes, 145 of 145 planted faults refused. 9 bend sources unconfirmed. No blind judge.
- **Vault:** stage 0 built. Sameness across niches 2.2%, against 0.9% for published films. No film made from a slot yet.
- **Facts:** stage valid, 0 fallbacks on 8 tables. Second reader 0 of 100. No cold run.

## Web app and rooms
- Pressed 24 Nov 01:22 (lead): 61 screens, 32 desktop, 29 phone. Gate, Altar, Crossroads, Cauldron, Pact, Conjuring, Spell Strip and Publish Kit work on the main path. Not every button checked.
- "Make a film" still only makes the practice minute (lead, 07:40). A worker started at 08:06 to make it start the real film, on web and phone. Not reported done.
- Five cards are placeholders on the test copy. Mirror Bend and Feed Sight show broken or empty pictures. New Vessel and the Tank are drawings. The sound room sends you back to the Altar.
- Cauldron price overlaps the list on phone. Not confirmed fixed.
- Census: 573 controls; 112 real, 160 sample, 131 dead (measured, 24 Nov 20:00). Decisions: remove 378, keep 98, wire 79, build 18.
- Outside critics have not reviewed the rooms.

## Mac app and APK
- APK files built: 0. APK tested: no. Nothing has run on a phone.
- Phone job: an Android emulator run had 19 checks pass and 3 fail (lead, 24 Nov 23:14). Paused. Needs the Galaxy plugged in. Must export with no connection.
- Mac app: no release build reported. Not tested.
- Disk: 9.6 GB free after old build leftovers were cleared (lead, 08:06).

## Agents running now
- Unknown. The live agent page did not answer. Seven transcripts were written in the last 10 minutes.
- Last reported, not confirmed live:
  - film worker: rebuilt Ottoman film and Mughal through the whole chain (08:21);
  - app worker: "Make a film" server pieces (08:22);
  - sound, vault and facts repairs;
  - engine builder on the ten missing primitives.
- All reviewers reported finished, last at 08:03.

## Money spent on services
- Ledger: $6.0073 over 5,825 calls. OpenRouter $2.9972, DeepSeek $1.9606, Google $0.5074, Inworld $0.2357, WaveSpeed $0.171, unsettled $0.1355.
- Answered calls: DeepSeek 2,753 (13 refused or failed); OpenRouter 2,902 (45); Google 11 (7); Inworld 78 (1); WaveSpeed 5 (0).
- Working limit: 10.00 US (lead). Budget: 135 CAD agreed (ADR 0008). The ledger is the record.
- Provider balances: no current check. Google's prepaid balance is not in the facts.
- Inworld: stock voices answer. No speech in a film reported.

## Broken, blocked or open
- **GitHub billing blocks the merge** (lead, 08:16). All seven passed their combined test with 0 failures. The final step that records the pass could not run. Nothing is merged.
- **PR 26, sound:** the watcher reserves 0.000336 per call, but main prices the call at 0.001344, so main refuses every such call (worker, 08:03). Fails closed. The reservation also has no lock. Not reported fixed.
- **Missing prices:** main's price list has no price for two models, so the gate refuses their calls in PRs 24 and 25 (worker, 07:49). Not rechecked.
- **Two test frames** of our own were pushed on PR 26 by mistake. The branch stays (worker, 07:49).
- **Pending rulings:** the 1.28 s hush rule on silent films (sound worker). Vault LINE-RULE items 7 to 20 await countersign. ADR 0010 (20-minute plan) is a candidate, not accepted.
- Finish check: 2 of 23 clauses true. Not done.
- The full chain for a 10-minute or voiced film is not made.
- Cauldron, board frames and subtitles: not confirmed fixed. Art direction: not judged.
- Mac load is rising while the film chain and builds run.

## Waiting on Ambi
- **Fix GitHub billing:** open Settings, then Billing and plans. Fix the payment or raise the spending limit. The lead then restarts the last step and merges the seven (lead, 08:16).
- **Watch the Mughal film** (strip-mughal) and name the worst thing in it.
- **Decide on a one-minute voice take.** The lead asked at 06:50 and 07:40. Any voiced ten-minute take needs his yes (lead, 05:24).
- **Ear table:** holds one refused line; the script checker needs about five.
- **Packaging:** his eye and ear decide. Bend facts still unopened.
- **Phone:** plug in the Galaxy.

















# Sheet of 08:18 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Covers 08:16 to 08:18 EAT, Wed 25 Nov 2026, against the last sheet (08:16).
- **Mughal Empire film is DONE:** `strip-mughal`, 60 s, 0.008507 US, finished 07:59. The lead watched it one frame every 3 seconds. He has not judged it good. Lead says it is the first of ten new subjects to finish.
- **GitHub is blocked (lead, 08:16):** GitHub stopped running jobs. It says the account is at its limit or the spending limit must rise. All seven pull requests passed their combined test with 0 failures. The final step that records the pass could not run. Nothing is merged.
- **Pull requests:** 7 open (21 to 27), 19 merged, 1 closed (15). Unchanged. Each of the seven has two CLEAN reviews (worker, 08:03).
- **Paid calls:** 5,824 calls, $6.0071 (last sheet: 5,822, $6.0065). OpenRouter now 2,901 ok and last ok 08:18.
- **Whole-film runs on disk:** 3 DONE, 3 FAILED, 19 HOLD. The list shows strip-mughal DONE, so the count and the list agree now.
- **Logged attempts:** 236 kept, 33 reverted, 40 inconclusive (unchanged).
- **Mac load (1, 5, 15 min):** 87, 71, 69 (last sheet 69, 63, 66). Load is rising.
- **Running agents:** unknown. The live agent page did not answer. Nine transcripts were written in the last 10 minutes.
- **Worker at 08:15:** the Ottoman film with a second rebuild is being run through the whole chain with the same binary.

## What worked and what failed
**Worked**
- `juju make` produced one-minute films with no test switch: otto-silent-2 (06:45, silent, 0.068 US), otto-chron-2 (07:39, 0.001904 US, words on the map), strip-mughal (07:59, 0.008507 US, from one typed sentence). The lead reports all three work but are not good.
- Mughal is the first subject Juju had never seen to reach a finished file.
- Title checks: 0 of 15 planted false titles pass (before: 15 of 15). Worker, 05:26.
- Vault review: 7 blocking faults, each red before the fix and green after. Simulation: 21,182 dealt, 238 refused, 0 faults on re-read (worker, 08:12).
- Film-study tool: same answers as plain decoding; kill and resume give the same answers.
- Review of PRs 21 to 27: all six reviewed CLEAN by opus-ship-c (08:03). Planted tests named on GitHub. Reviews are mechanical and deeper; not a judgment of films.

**Failed**
- Ambi, 24 Nov 23:17, on the dot strip the lead had praised: "the worst looking thing ive ever seen." He asked for Juju's own house worlds.
- Ambi, 24 Nov 20:57, on the script line "the sun gave nothing": "What kind of slop is that?" The lead and two Claude listeners had praised it.
- Nine of ten new subjects did not reach a file (Japan, Pluto, Manchuria, Bulgaria, Austria, Jerusalem, Venice, Sweden, Space). Causes listed in the workers: title and thumbnail rules, too few dated events with a place, lines no fact supports, camera moves.
- Harvest fast runner: about 1.2 times faster, not the 3 times target. Lead, 04:15.
- Facts lane: 2 of 15 opened facts wrong, 6 pins misplaced (lead, 06:47). Later: two more bad pins found (Sarai beside Baku, Borodino in Siberia), lead, 04:30.

## App engine and films
- **Mughal film `strip-mughal` (lead, 08:16):** DONE, 60 s, 0.008507 US. Mountains real, edges smooth, land lights up as it changes hands. Still wrong: words too small for a phone; Mughal land first shows in 1539 though the film starts in 1525; it stops at 1659 though the idea said 1707; some lines weak ("But the Mughal Empire grew and took land").
- **Ottoman films (lead, 07:40):** words tiny, coasts blocky, one colour on grey; "Belgrade was captured" shows at 1497; "invaded Syria" sits on Istanbul. The silent one has no words.
- **Rebuilt Ottoman film (worker, 08:15):** every line sits at its place, after its year, readable, clean coasts, almost no inner borders. Running through the whole chain. Not yet judged by the lead.
- **Engine gap (60-film study, 03:39):** the engine draws 12 of 40 picture moves in the reference films, and 0 of 20 skeleton and house pairs whole. Ten missing primitives ranked. The builder is still coding; no new result reported.
- **House strips:** Egypt, Orion and lungs repaired at 08:05. Code check passes, 31 unit tests. Looks judged only by their maker. Need fresh eyes. No sound. Render 7 to 19 seconds per film second at load 57 to 95 (target 1.0 missed).
- **Sound:** silent film at -14.6 LUFS, 4 of 4 cues heard (worker). A 20-minute film took 912 s. The 1.28 s hush rule on silent films needs a ruling.
- **Voice:** no voice in any real film. Nothing made at 10, 20, 30 or 50 minutes.
- **Harvest:** 11 of 12 films have notes (lead). Motion language covers 64 of 64 hand-marked rows, held out on one film only. Our eye found 35 of 35 drawn events against rea-video's 10 of 35, on the windows it was built on. No pack is built.
- **Packaging:** 9 frames and 45 bends. Check passes; 145 of 145 planted faults refused. 9 bend sources unconfirmed. No blind judge yet.
- **Vault:** stage 0 built. Sameness across niches is 2.2%, against 0.9% for published films. No film is made from a slot yet.
- **Facts:** stage is valid with 0 fallbacks on 8 tables. Second reader 0 of 100. No cold run.

## Web app and rooms
- Pressed 24 Nov 01:22 (lead): 61 screens, 32 desktop and 29 phone. Gate, Altar, Crossroads, Cauldron, Pact, Conjuring, Spell Strip and Publish Kit work.
- "Make a film" is being wired to the real film by a worker started 08:06 (lead). Not reported done.
- Every path ended at the practice minute as of 01:22. The Roman roads idea queued the practice film, not a Roman roads film. Not re-tested since.
- The five cards are placeholders. Mirror Bend and Feed Sight show broken or empty pictures. New Vessel and the Tank are drawings. The sound room sends you back to the Altar.
- Census: 573 controls; 112 real, 160 sample, 131 dead (measured, 24 Nov 20:00).
- Cauldron price overlaps the list on phone. Not confirmed fixed. Outside critics have not reviewed the rooms.

## Mac app and APK
- APK files built: 0. APK tested: no. Nothing has run on a phone.
- Phone job: an Android emulator run had 19 checks pass and 3 fail (lead, 24 Nov 23:14). Paused since. Needs the Galaxy plugged in.
- Mac app: no release build reported. Not tested.
- Disk: 3.9 GB free at 08:05, then 9.6 GB after old build leftovers were cleared.

## Agents running now
- Unknown. The live agent page did not answer. Last reported, not confirmed live:
  - a film worker running the rebuilt Ottoman film and Mughal through the whole chain (08:15);
  - an app worker wiring "Make a film" (08:06);
  - sound, vault and facts repairs;
  - the engine builder on the ten missing primitives.
- All PR reviewers reported finished, last at 08:03.

## Money spent on services
- Ledger: $6.0071 over 5,824 calls. OpenRouter $2.997, DeepSeek $1.9606, Google $0.5074, Inworld $0.2357, WaveSpeed $0.171, unsettled $0.1355.
- Answered calls: DeepSeek 2,753 (13 refused or failed); OpenRouter 2,901 (45); Google 11 (7); Inworld 78 (1); WaveSpeed 5 (0).
- Balances last checked 12:37 Tue (lead), not rechecked: OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00.
- Budget: 135 CAD agreed (ADR 0008). Working limit 10.00 US (lead). Spent 5.97 US by the lead's count (07:40); the ledger is the record.
- Google: paid access works; prepaid balance not in the facts. Inworld: stock voices answer. No speech in a film reported.

## Broken, blocked or open
- **GitHub billing blocks the merge** (lead, 08:16). Nothing merges until fixed.
- **PR 26, sound:** the watcher reserves 0.000336 per call, but main prices it at 0.001344, so main refuses every such call. A film with no kept answer gets no sound. It fails closed. Fix needed; the reservation also has no lock (worker, 08:03).
- **Two frames of our own test film** were pushed to GitHub on PR 26 by mistake. The branch stays (worker, 07:49).
- **Prices missing:** main's price list has no price for two models, so the gate refuses their calls in PRs 24 and 25 (worker, 07:49).
- **PR 21 and 22 faults** were repaired and reviewed CLEAN (08:03).
- Lead (13:42 Tue): main's juju-stage tests do not compile. No later report.
- Finish check: 2 of 23 clauses true. Not done.
- The full chain for a 10-minute or voiced film is not made.
- Cauldron, board frames and subtitles: not confirmed fixed. Art direction: not judged.
- Mac load is rising (87 at 1 min) while the film chain and builds run.
- Nuance: 21 of 24 risky instruction lines misread by cheap models (13:43 Tue).

## Waiting on Ambi
- **Fix GitHub billing:** open Settings, then Billing and plans. Fix the payment or raise the spending limit. The lead then restarts the last step and merges the seven (lead, 08:16).
- **Watch the Mughal film** (`strip-mughal`) and name the worst thing in it.
- **Decide on a one-minute voice take** (lead asked 06:50 and 07:40). Any voiced ten-minute take needs his yes (lead, 05:24).
- **ADR 0010** (20-minute plan): candidate, not accepted.
- **Ear table:** holds one refused line; the script checker needs about five.
- **Packaging:** his eye and ear decide. Bend facts still unopened.
- **LINE-RULE items 7 to 20** (vault): awaiting countersign.
- **Phone job:** plug in the Galaxy.
- **Standing advice** (lead, 12:48 Tue): keep Inworld permissions read-only.


















# Sheet of 08:16 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- This sheet covers 13:45 Tue 24 Nov to 08:16 Wed 25 Nov.
- **A film from a new subject is DONE:** Mughal Empire, 60 s, 0.008507 US (FACTS NOW, 07:59). The lead reports it took 16 minutes and that it is the first of ten new subjects to finish. He watched it, one frame every 3 seconds. He has not judged it good.
- **GitHub is blocked (lead, 08:16):** GitHub stopped running jobs and says the account is at its limit or the spending limit must rise. All seven pull requests passed their combined test with 0 failures. The final step that records the pass could not run. Nothing is merged.
- **Pull requests:** 7 open (21 to 27), 19 merged, 1 closed (15). The count is unchanged. All seven now have two CLEAN reviews (worker, 08:03).
- **Paid calls:** 5,822 calls, $6.0065 (last sheet: 5,821, $6.0064).
- **Whole-film runs:** FACTS NOW counts 3 DONE, 3 FAILED, 19 HOLD. Its own list also shows strip-mughal DONE, so the count and the list disagree. Not resolved.
- **Newest film runs:** strip-bulgaria, strip-austria and strip-manchuria HOLD at Deal and package (08:11). strip-pluto HOLD at Render and mix (08:08). otto-chron-3 and thru-mughal HOLD at Pictures and form (08:06).
- **Logged attempts:** 236 kept, 33 reverted, 40 inconclusive (last: 234 kept).
- **Mac load (1, 5, 15 min):** 69, 63, 66.
- **Running agents:** the live agent page did not answer, so running agents are unknown. Nine agent transcripts were written in the last 10 minutes.

## What worked and what failed
**Worked**
- `juju make` produced one-minute films with no test switch. otto-silent-2 (06:45, 0.068 US, 17.2 minutes, silent). otto-chron-2 (07:39, 0.001904 US, with words on the map). strip-mughal (07:59, from one typed sentence). The lead reports all three are works but not good.
- Title checks: 0 of 15 planted false titles pass now (before: 15 of 15). Worker, 05:26.
- Vault review: 7 blocking faults, each red before the fix and green after. Simulation: 21,182 dealt, 238 refused, 0 faults on re-read (worker, 08:12).
- Harvest tool: same answers as plain decoding, and kill and resume give the same answers.

**Failed**
- Ambi, 24 Nov 23:17, on the dot strip the lead had praised: "the worst looking thing ive ever seen." He asked for Juju's own house worlds.
- Ambi, 24 Nov 20:57, on the script line "the sun gave nothing": "What kind of slop is that?" The lead and two Claude listeners had praised it.
- Ten new subjects tried. Mughal is the only one to reach a finished film. The others stopped at title and thumbnail rules, too few dated events with a place, lines no fact supports, or camera moves. Several are HOLD now (see Changed).
- Harvest fast runner: about 1.2 times faster, not the 3 times target. Lead, 04:15.
- Facts lane: 2 of 15 opened facts wrong, 6 pins misplaced (lead, 06:47).

## App engine and films
- **Ottoman films (lead, 07:40):** words are tiny, coasts are blocky, one colour on grey, some events wrong ("Belgrade was captured" shows at 1497; "invaded Syria" sits on Istanbul). The silent one has no words at all.
- **Mughal film (lead, 08:16):** mountains are real, edges smooth, land lights up as it changes hands. Still wrong: words too small for a phone; Mughal land first shows in 1539 though the film starts 1525; it stops at 1659 though the idea said 1707; some lines are weak.
- **Engine gap (60-film study, 03:39):** the engine draws 12 of 40 picture moves in the reference films, and 0 of 20 skeleton and house pairs whole. Ten missing primitives are ranked. The builder is still coding; no new result reported.
- **House strips:** Egypt, Orion and lungs repaired at 08:05. The code check passes, with 31 unit tests. Looks were judged only by their maker. They need fresh eyes. No sound. Render 7 to 19 seconds per film second at load 57 to 95 (target 1.0 missed).
- **Sound:** silent film at -14.6 LUFS, 4 of 4 cues heard (worker). A 20-minute film took 912 s. The 1.28 s hush rule on silent films needs a ruling.
- **Voice:** no voice in any real film. Nothing made at 10, 20, 30 or 50 minutes.
- **Harvest:** logs list at least five films read whole by 07:58. The motion language covers 64 of 64 hand-marked rows, tested held-out on one film only. Our eye found 35 of 35 drawn events against rea-video's 10 of 35, on the windows the eye was built on. The lead says 11 of 12 films have notes. No pack is built.
- **Packaging:** 9 frames and 45 bends. The check passes, and 145 of 145 planted faults are refused. Nine bend sources are unconfirmed. No blind judge yet.
- **Vault:** stage 0 built. Sameness across niches is 2.2%, against 0.9% for published films. No film is made from a slot yet.
- **Facts:** the stage is valid with 0 fallbacks on 8 tables. Second reader 0 of 100. No cold run.

## Web app and rooms
- Pressed 24 Nov 01:22 (lead): 61 screens, 32 desktop and 29 phone. Gate, Altar, Crossroads, Cauldron, Pact, Conjuring, Spell Strip and Publish Kit work.
- Every path ends at the practice minute. The Roman roads idea queued the practice film, not a Roman roads film.
- The five cards are placeholders. Mirror Bend and Feed Sight show broken or empty pictures. New Vessel and the Tank are drawings. The sound room sends you back to the Altar.
- "Make a film" is being wired to the real film by a worker started 08:06 (lead). Not reported done.
- Census: 573 controls; 112 real, 160 sample, 131 dead (measured, 24 Nov 20:00).
- Cauldron price overlaps the list on phone. Not confirmed fixed. Outside critics have not reviewed the rooms.

## Mac app and APK
- APK files built: 0. APK tested: no. Nothing has run on a phone.
- Phone job: an Android emulator run had 19 checks pass and 3 fail (lead, 24 Nov 23:14). Paused since. Needs the Galaxy plugged in.
- Mac app: no release build reported. Not tested.
- Disk: 3.9 GB free at 08:05, then 9.6 GB after old build leftovers were cleared.

## Agents running now
- Unknown, since the live page did not answer. Last reported, not confirmed live:
  - a film worker running two films through the whole chain (08:15);
  - an app worker wiring "Make a film" (08:06);
  - unseen-subject runs (Japan, Pluto, Manchuria, Bulgaria, Austria);
  - sound, vault and facts repairs.
- All PR reviewers reported finished, last at 08:03.
- Design-system teardowns: 0 of 5 finished (last report, 13:45 Tue).

## Money spent on services
- Ledger: $6.0065 over 5,822 calls. OpenRouter $2.9964, DeepSeek $1.9606, Google $0.5074, Inworld $0.2357, WaveSpeed $0.171, unsettled $0.1355.
- Answered calls: DeepSeek 2,753 (13 refused or failed); OpenRouter 2,899 (45); Google 11 (7); Inworld 78 (1); WaveSpeed 5 (0).
- Google: paid access works. Prepaid balance not in the facts. Inworld: stock voices answer. No speech in a film reported.
- Balances last checked 12:37 Tue (lead), not rechecked: OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00.
- Budget: 135 CAD agreed (ADR 0008). Working limit 10.00 US (lead).
- Lane limits: sound 0.50 US (0.478 at 08:03); gather 0.20 US (0.198 spent); sigil 0.25 US (0.077 spent). The lead's 5.97 US figure is older than the ledger.

## Broken, blocked or open
- **GitHub billing blocks the merge** (lead, 08:16). Nothing merges until fixed.
- **PR 26, sound:** the watcher reserves 0.000336 per call, but main prices it at 0.001344, so main refuses every such call. A film with no kept answer gets no sound. It fails closed. Fix needed; the reservation also has no lock (worker, 08:03).
- **Two frames of our own test film** were pushed to GitHub on PR 26 by mistake. The branch stays (worker, 07:49).
- **Prices missing:** main's price list has no price for two models, so the gate refuses their calls in PRs 24 and 25 (worker, 07:49).
- Lead (13:42 Tue): main's juju-stage tests do not compile. No later report.
- Finish check: 2 of 23 clauses true. Not done.
- The full chain for a 10-minute or voiced film is not made.
- Cauldron, board frames and subtitles: not confirmed fixed. Art direction: not judged.
- Nuance: 21 of 24 risky instruction lines misread by cheap models (13:43 Tue).

## Waiting on Ambi
- **Fix GitHub:** open Settings, then Billing and plans. Fix the payment or raise the spending limit. The lead then restarts the last step and merges the seven (lead, 08:16).
- **Watch the Mughal film** and name the worst thing in it. He was also asked to do this for the silent Ottoman film (lead, 07:40).
- **Decide on a one-minute voice take** (lead asked 06:50 and 07:40). Any voiced ten-minute take needs his yes (lead, 05:24).
- **ADR 0010** (20-minute plan): candidate, not accepted.
- **Ear table:** it holds one refused line; the script checker needs about five.
- **Packaging:** his eye and ear decide. Bend facts still unopened.
- **LINE-RULE items 7 to 20** (vault): awaiting countersign.
- **Phone job:** plug in the Galaxy.
- **Standing advice** (lead, 12:48 Tue): keep Inworld permissions read-only.



















# Sheet of 08:13 EAT, Wed 25 Nov 2026

## Changed since the last sheet
- Sheet covers 13:45 Tue 24 Nov to 08:13 Wed 25 Nov.
- Paid calls in the test ledger: 5,821 calls, $6.0064 (last sheet: 1,188 calls, $0.8778). The lead's 07:40 figure was $5.97 of a 10.00 US working limit. The ledger is the newer measured figure.
- Rust: 32,121 lines in 14 crates (last sheet: 12,772 in 7). Skills: 52 (last: 46). Decisions: 19 (last: 9).
- Design-system items on disk: 13 (last sheet: none). They are camera_motion.json, palettes.json, and folders for fonts, house, kits, looks, proof, proto and work pieces.
- Pull requests: 7 open (21 to 27), 19 merged, 1 closed (15). Last sheet: 8 open, 0 merged.
- Whole-film runs of `juju make`: 3 DONE, 3 FAILED, 19 HOLD.
- Logged attempts: 234 kept, 33 reverted, 40 inconclusive.
- Two one-minute films are DONE: otto-silent-2 (06:45) and otto-chron-2 (07:39).
- Mac load (1, 5, 15 min): 62, 60, 66 (last sheet: 67, 60, 64).
- Newest commit on main: 08:12, juju-db.
- The live agent page did not answer, so running agents are unknown.

## What worked and what failed
**Worked**
- `juju make` produced a one-minute silent film with no test switch (otto-silent-2, DONE, 0.068 US, 17.2 machine minutes). A second one with map words (otto-chron-2) reached DONE at 07:39. The run reports DONE. The lead has not judged either film good.
- Title checks (juju-next 0.5.0): 0 of 15 planted false titles pass now. Before, 15 of 15 passed. Zero cards stand.
- Vault review (worker): 7 blocking faults found, each red before the fix and green after. Simulation: 21,182 dealt, 238 refused, 0 faults on re-read.
- Pull requests 21, 22, 24 and 25 had blocking faults in second review. Each was repaired and rechecked CLEAN by the worker.
- Harvest tool gives the same answers as plain decoding. Kill and resume give the same answers.

**Failed**
- Ambi refused the dot strip the lead had praised (24 Nov 23:17): "the worst looking thing ive ever seen." He asked for Juju's own house worlds instead.
- Unseen subjects: nine tried (Japan, Pluto, space, Mughal, Venice, Sweden, Jerusalem, Manchuria, and one more). None reached a finished film. They stopped at title and thumbnail rules, at too few dated placed events, or at unsupported lines.
- Harvest fast runner: about 1.2x, not the 3x target.
- Facts lane: 2 of 15 opened facts wrong (06:47).
- Ottoman film (lead, 07:40): "Belgrade was captured" shows at 1497. "Invaded Syria" sits on Istanbul.

## App engine and films
- Whole-film chain: one minute, silent, works end to end. Not good yet. Lead's view: words are tiny, coastlines are blocky, one colour on grey, some events wrong. Worker's ten worst seconds are in the 07:25 message. The worker says it still has a counter error for about 1.5 s of each flight; the fix is in code.
- Next film (otto-chron-3) and a second empire: worker was drawing border stills at 08:13. Not reported finished.
- House strips (engine): Egypt, Orion and lungs repaired at 08:05. Code check TRUE, 31 unit tests pass. Looks judged only by their maker. Needs fresh eyes. No sound. Render is 7 to 19 seconds per film second at load 57 to 95 (target 1.0 missed).
- Engine gap (60-film study): it draws 12 of 40 picture moves. It draws 0 of 20 skeleton and house pairs whole.
- Silent-film sound: -14.6 LUFS, 4 of 4 cues heard (worker). Sound lane: a 20-minute film took 912 s at load 35 to 49. A 1.28 s hush rule on silent films needs a ruling.
- Voice: no voice track in any real film. Nothing made at 10, 20, 30 or 50 minutes. Lead's 20-minute plan says it fits; voice cost not measured. Film form filling costs about 5 cents per film (13:42 Tue).
- Harvest: lead says most of the twelve chosen films are read whole (07:40). rea-video scored 10 of 35 drawn events. Our own eye scored 35 of 35 on the same windows, with no held-out proof. Film-harvest skill merged (PR 20). Motion language written; held-out test on one film only.
- Packaging: 9 frames, 45 bends, check TRUE, 145 planted faults refused. Bend facts unopened. No blind judge.
- Vault: stage 0 built. Sameness across niches is 2.2%, against 0.9% for published films. No film made from a slot yet.
- Facts (gather): stage valid, 0 fallback on 8 tables. Second reader 0 of 100. No cold run.

## Web app and rooms
- Last reported 13:45 Tue. No newer report.
- All 19 rooms have a first build. 4 of 8 room builders had finished; four were still running.
- Cauldron: price overlaps the list on phone. Not confirmed fixed.
- Board: 329 room states at two sizes. Desktop frames were empty at 12:48. A later log lists them rendered. No judge check.
- ADR 0009 (quiet screens) accepted. PR 3 (quiet-screen rules) is merged (19:48 Tue), not open as the last sheet said.
- "Make a film" in the app still starts only the practice minute (07:40). A worker started wiring the real film at 08:06. Not reported done.
- Outside critics have not reviewed the rooms.

## Mac app and APK
- APK files built: 0. APK not tested.
- Mac app: nothing reported. Not tested.
- Earshot runs in full, phone included (Ambi, 24 Nov 08:16). Phone spike measured 08:48. No later result.
- Disk fell to 3.9 GB at 08:05, then reached 9.6 GB after old build leftovers were cleared.
- Load was 54 on 8 cores at 07:32 during builds and film render.

## Agents running now
- Live agent page did not answer. Running agents are unknown.
- Last reported at 08:06 to 08:13: film worker drawing border stills; app worker wiring "Make a film"; unseen-subject runs (Japan, Mughal); sound and gather repairs; a worker on PR checks and merges.
- GitHub combined check on PRs 21 to 27 was reported about 30 minutes long from 08:06.
- Design-system teardowns: last reported 0 of 5 finished (13:45 Tue). No later report.

## Money spent on services
- Ledger: $6.0064 over 5,821 calls. By service: OpenRouter $2.9963, DeepSeek $1.9606, Google $0.5074, Inworld $0.2357, WaveSpeed $0.171, unsettled $0.1355.
- Answered calls: DeepSeek 2,753 (13 refused or failed). OpenRouter 2,898 (45). Google 11 (7). Inworld 78 (1). WaveSpeed 5 (0).
- Google: paid access works. Prepaid balance not in the facts.
- Inworld: stock voices answered. No speech in a film reported.
- Balances last checked 12:37 Tue (lead): OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00. Not rechecked.
- Budget: 135 CAD agreed (ADR 0008). The 10:52 Tue split was Inworld 55, OpenRouter 23, DeepSeek 22, Google 21, WaveSpeed 14.
- Lane limits: sound 0.50 US (lane at 0.478 at 08:03). Sigil 0.25 US (0.077 spent, 00:57 Tue). Gather 0.20 US, nearly used.

## Broken, blocked or open
- PR 26 (sound): reserves 0.000336 per Watcher call, but main prices it at 0.001344. Main refuses those calls, so a film with no saved answer gets no sound. Fails closed. Fix needed.
- Two frames of our test film went to GitHub by mistake on PR 26. The branch stays.
- 7 PRs open, none merged. Mechanical and second reviews are CLEAN on all seven. Combined checks still pending.
- Otto film faults (worker, 07:25): 4 of 10 lines pinned to the signing of a paper, not the event. Stops at 1908 with no end.
- Lead (13:42 Tue, no later report): main's juju-stage tests do not compile.
- Finish check: 2 of 23 clauses true, so not done.
- Full chain for a 10-minute or voiced film: not made.
- Cauldron, board frames, subtitles: not confirmed fixed.
- Art direction: not judged (5 to 6 of 10 earlier).
- Packaging: 4 of 6 packages are below the winners' median contrast. The skill-ordered ranking got 48% right; random got 50%. The 90/70/50 rule could not be tested.
- Nuance (13:43 Tue): 21 of 24 risky instruction lines misread by cheap models.
- Gemini cache: 0 of 3 repeats saved.
- Design-system teardowns: 0 of 5 finished at last report.

## Waiting on Ambi
- Watch the one-minute silent film (otto-chron-2) and name the worst thing in it. Lead asked this at 07:40.
- Decide on a one-minute voice take. Lead asked at 06:50 and 07:40.
- Ambi's yes is still needed for any voiced ten-minute take (lead, 05:24).
- ADR 0010 (20-minute plan): candidate. Acceptance not reported.
- Replacement 90/70/50 wording for packaging (worker, 13:46 Tue).
- Packaging: Ambi's eye and ear decide. Bend facts still unopened.
- LINE-RULE items 7 to 20 (vault): awaiting countersign.
- Standing advice (lead, 12:48 Tue): keep Inworld permissions at read only.




















# Sheet of 13:45 EAT, Tue 24 Nov 2026

## Changed since the last sheet
- Paid calls in the test ledger: 1,188, $0.8778 (last sheet: 1,055, $0.7310). DeepSeek $0.4004, OpenRouter $0.2951, Google $0.1822.
- Direct Google key: the lead reports it works (13:42). This corrects the 13:21 report that only the OpenRouter route worked. The ledger shows 4 refused Google calls, last success 13:13.
- One spend meter now covers all paid tests, cap $2.25 for today (lead, 13:42). The ledger is at about 39% of it. The earlier $0.60 cap in one script is replaced.
- Mac load (1, 5, 15 min): 67, 60, 64 (last sheet: 45, 42, 61).
- Rust: 12,772 lines in 7 crates (last sheet: 12,109). Skills: 46 (last sheet: 44).
- Engine: 3 of 4 agents finished (last sheet: 2).
- Model measurements (lead, 13:42): DeepSeek on low thinking filled the film form validly 2 of 2 times. Thinking off was invalid. GLM low returned nothing for $0.06. Gemini cache: 0 of 3 repeats saved.
- Nuance test done (13:43): 21 of 24 risky instruction lines were misread by cheap models. 8 are fully cured on fresh material.
- Packaging test (13:46): 6 title and thumbnail packages drawn. The skill-ordered ranking got 48% of pairs right; random got 50%.
- ADR 0009 (quiet screens) accepted (13:00). ADR 0010 (20-minute plan) is a candidate.
- Ancient Logos teardown: silent since 13:14. The lead's 13:42 workflow includes a restart. Not reported running.
- Commits on main: none reported since e0115bd (10:33).

## App engine and films
- Engine: 3 of 4 finished. build:worlds running.
- Round 5 picture sheet (12:48): not scored by judges. Lead says it looks better than round 1. Earlier scores were 4 to 6 of 10.
- Subtitles and small labels are too wordy (12:48). Not confirmed fixed.
- Test render, 187 seconds (12:10): 1080p, 0 fallback scenes, safe-box check passed, no voice track, one act. A picture test, not a full film.
- Film reader: 0 of 1 finished. build:absorb running (tests, build, first clip).
- Design systems: 0 of 5 finished. Five teardowns running. No design-system library on disk.
- Milky Stellar teardown (lead, 13:17): 16 devices with times. Its job waits up to nine minutes for shared-lock jobs.
- Film cost (lead, 13:17): about $0.55 per 50-minute film on DeepSeek and $2.14 on GLM, at high or max thinking. Not shown to fit the budget.
- 20-minute plan (lead, 13:42): the lead's estimate says it fits. Voice is the tight part. Voice cost is not measured. Filling the film form is measured at about 5 cents per film.
- Freshness answer to the YouTube demonetisation wave (lead, 13:42): locked stance, voice and type; slow changes; new argument, opening, worlds and title per film; length 16 to 24 minutes. A sameness meter is planned, not built. The lead rejects random shuffling to fool a detector.

## Web app and rooms
- All 19 rooms have a first build. 4 of 8 room builders finished.
- Still running: crossroads, cauldron, conjuring, new-vessel.
- Cauldron: price overlaps the list on the phone screen (lead, 12:48). Round 6 renders running. No fix confirmed.
- Board (13:00): 329 room states at two sizes on one canvas. Desktop frames were empty at 12:48. A 13:00 log lists them as rendered. No judge check reported.
- Page map: board-fix was 12 of 13 finished, waiting for the final build and push. It is not in the 13:45 job list, so its end is not reported.
- ADR 0009: 30 interface words at desktop, 24 at phone, no text of 5 words or more, one 1 to 2 word status per object. Quiet-screen rules are in PR 3, open.
- Outside critics have not reviewed the rooms.

## Mac app and APK
- APK files built: 0. APK not tested.
- Mac app: nothing reported. Not tested.
- Earshot runs in full, phone included (Ambi, 08:16). Phone spike measured 08:48. No later result. build:voice is finding the Earshot model cache and running a check.
- Video work runs one job at a time (lead, 12:37). Load is still high.

## Agents running now
- Engine: build:worlds (3 of 4 finished)
- Conductor: fix:r2 (10 of 11 finished)
- Rooms: crossroads, cauldron, conjuring, new-vessel (4 of 8 finished)
- Film reader: build:absorb (0 of 1 finished)
- Design systems: five teardown jobs (0 of 5 finished)
- Guard, voice, 3D, PR loop: six jobs (0 of 6 finished): wave facts, PR review loop, one teardown, freshness build, money build, voice build
- Page map: board-fix, not in the 13:45 list

## Money spent on services
- Ledger: $0.8778 over 1,188 calls. Successful answers: DeepSeek 824 (1 refused or failed), OpenRouter 351 (1), Google 7 (4).
- Balances at 12:37 (lead): OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00. Not rechecked since.
- Google: billing linked; direct key works (lead, 13:42). Prepaid balance not in the facts.
- Inworld: key works, 403 stock voices (lead, 13:42; earlier 407). No charge seen. Making speech not tested.
- Budget: 135 CAD agreed (ADR 0008). The 10:52 split was Inworld 55, OpenRouter 23, DeepSeek 22, Google 21, WaveSpeed 14. Film costs above are not shown to fit.
- Gemini cache: 0 of 3 repeats saved (lead, 13:17; earlier figure of 5 corrected).
- Spend guard: one meter, cap $2.25 for today (13:42). The earlier worst case of $1.25 is superseded.

## Broken, blocked or open
- Engine drawing tests do not compile on main. PR 5 fixed the picture finder (26 of 26 pass). Lead says the main tests for juju-stage do not compile (13:42).
- PR 1 loosened the checks, so green status is partial. The 8 PRs were tested alone, not together. None merged.
- Conductor room list: a worker says two entries must be added, or the conductor refuses to start on its next build (13:41). Not reported done.
- Cauldron price overlap, board desktop frames, subtitles: not confirmed fixed.
- Art direction: not judged (earlier 5 to 6 of 10).
- Voice: no voice track. Inworld speech not tested.
- Film costs and the 20-minute plan: not measured end to end. Not shown to fit.
- Nuance: 6 new rules are written but no code enforces them. 3 repairs are better, not cured. 4 cannot be fixed by wording.
- Packaging: 4 of 6 packages are below the winners' median contrast, on hold. Foil is rated weak. The skill-ordered ranking did no better than random. The 90/70/50 rule could not be tested.
- Thinking level: the packaging flow runs with thinking off, which departs from ADR 0006. The lead found thinking off invalid for the film form.
- Full run from script to finished film on your keys: not tested.
- Repo: uncommitted changes (205 files at 12:10). ADRs 0008 and 0009 are untracked (13:00).
- Ancient Logos teardown: status unknown since 13:14.

## Waiting on Ambi
- No item is marked as waiting on Ambi at 13:42 or 13:45.
- ADR 0010 (20-minute plan) is a candidate. Acceptance not reported.
- Replacement 90/70/50 wording is a candidate for Ambi (packaging worker, 13:46).
- Standing advice (lead, 12:48): keep Inworld permissions on Read only.





















# Sheet of 13:32 EAT, Tue 24 Nov 2026

## Changed since the last sheet
- Paid calls in the test ledger: 1,055, $0.7310 in all (last sheet: 940, $0.6548). Split: DeepSeek $0.317, OpenRouter $0.2317, Google $0.1822.
- Rooms: 4 of 8 builders finished now (last sheet: 3). The altar room finished.
- Mac load (1, 5, 15 min): 45, 42, 61 (last sheet: 36, 43, 75).
- Rust code: 12,109 lines in 7 crates (last sheet: 11,670).
- The lead reports a model test on one film form (13:21): GLM 5.3 high $0.0428, Neon low $0.0286, DeepSeek high $0.0080.
- Conflict, not resolved: the lead's 13:17 message says Gemini works. The 13:21 day log says direct Neon calls still get 429 and only the OpenRouter route works.
- ADR 0009 (quiet screens) is accepted (lead, 13:00).
- Ancient Logos teardown: silent since 13:14 (lead). The lead plans to check at 13:33.
- Commits on main: no new ones. Latest is e0115bd (10:33).

## App engine and films
- Engine: 2 of 4 agents finished. Running: build:worlds and build:speed.
- The lead reports 9 world kinds drawn and 112 licensed pictures gathered (12:48).
- Round 5 picture sheet (12:48): not scored by judges. The lead says it looks better than round 1. Earlier scores were about 4 to 6 out of 10.
- The lead reports subtitles and small labels are too wordy (12:48). Not confirmed fixed.
- Test render, 187 seconds (12:10): 1080p, 0 fallback scenes, safe-box check passed, no voice track, one act only. It is a picture test, not a full film.
- Film reader: 0 of 1 finished. build:absorb is running. The lead reports it is still building (12:48).
- Design systems: 0 of 5 finished. Five teardown jobs are running. No design-system library exists on disk.
- The lead shared a Milky Stellar teardown with 16 devices and times (13:17). Its job waits up to nine minutes for shared-lock jobs (facts, 13:32).
- Film cost estimates (lead, 13:17): about $0.55 per 50-minute film on DeepSeek and $2.14 on GLM, at high or max thinking. The lead says 92 to 98% of output is hidden thinking. These are not shown to fit the budget. The next test uses lower thinking and longer stretches per call.

## Web app and rooms
- All 19 rooms have a first build. 4 of 8 room builders are finished.
- Still running: crossroads, cauldron, conjuring, new-vessel.
- Cauldron: the lead reports a price overlapping the list on the phone screen (12:48). The round 6 renders are running. No fix is confirmed.
- Board (13:00): 329 room states at two sizes on one canvas.
- Page map: 12 of 13 finished. board-fix is still running and waiting for the final build and push.
- Desktop frames on the board were empty (lead, 12:48). Not confirmed fixed.
- ADR 0009: 30 interface words at desktop, 24 at phone, no text of 5 words or more, one 1 to 2 word status per object.
- Quiet-screen rules are in PR 3, which is open, not merged.
- Outside critics have not reviewed the rooms (lead, 12:48).

## Mac app and APK
- APK files built: 0. APK not tested.
- Mac app: nothing reported in the facts. Not tested.
- Earshot runs in full, including on the phone (Ambi's decision, 08:16). The phone spike was measured at 08:48. No later result is reported.
- Video work runs one job at a time to protect the Mac (lead, 12:37).

## Agents running now
- Engine: build:worlds, build:speed (2 of 4 finished)
- Conductor: fix:r2 (10 of 11 finished)
- Rooms: crossroads, cauldron, conjuring, new-vessel (4 of 8 finished)
- Film reader: build:absorb (0 of 1 finished)
- Design systems: five teardown jobs (0 of 5 finished)
- Page map: board-fix (12 of 13 finished)
- Keys and PRs: none running (3 of 3 finished)
- The lead reports nuance, storyboard and packaging test jobs. Nuance and packaging have ledger calls (13:21). Storyboard has not been reported since. None are in the job list.

## Money spent on services
- Ledger: $0.7310 across 1,055 paid calls (split above).
- Balances at 12:37 (lead): OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00. Ambi's note said $10 for WaveSpeed. Not rechecked since.
- Google: billing linked and the first paid call worked at 13:10 (lead). The prepaid balance is not in the facts.
- Inworld: key works, 407 voices listed, no charge. Making speech is not tested.
- Budget: 135 CAD agreed (ADR 0008). The film costs above are not shown to fit it.
- Gemini cache: 3 repeat calls saved nothing (lead corrected its earlier figure of 5). The paid cache and batch route are not tested.
- Spend guard: each job has its own limit. A shared lock now exists (teardown jobs wait on it). The lead has not reported a total-limit test. Worst case if all jobs hit their limits: $1.25 (lead, 13:21).

## Broken, blocked or open
- Engine drawing tests do not compile on main. PR 5 fixed the picture finder (26 of 26 pass). The drawing part is still red.
- PR 1 loosened the checks, so green status is partial. The 8 PRs were tested alone, not together. None are merged.
- Cauldron price overlap: not confirmed fixed.
- Board desktop frames: not confirmed fixed.
- Art direction: not judged.
- Engine subtitles and labels: too wordy, not confirmed fixed.
- Voice: no voice track. Inworld speech is not tested.
- Film costs: not shown to fit the budget.
- Gemini: direct-route status conflicts (see above).
- Full run from script to finished film on your keys: not tested.
- Repo: uncommitted changes (lead's count at 12:10: 205 files). ADRs 0008 and 0009 are untracked.
- Ancient Logos teardown: status unknown since 13:14.

## Waiting on Ambi
- Nothing is reported as waiting on Ambi (lead, 13:21).
- The Google billing step asked for at 13:07 is done. The first paid call worked at 13:10.
- Standing advice (lead, 12:48): keep Inworld permissions on Read only.






















# Sheet of 13:27 EAT, Tue 24 Nov 2026

## Changed since the last sheet
- Paid calls rose from 940 to 991. Spend rose from $0.6548 to $0.6938.
- Mac load (1, 5, 15 min) went from [36, 43, 75] to [35, 41, 69].
- Several running tasks have new notes. Details are in the agent sections below.
- Newest commit on main: e0115bd, 24 Nov 10:33, "Decision: the software first, no channel drives the build."
- Pull requests, Rust size, skills, rooms drawn, decisions, APK count and design-system libraries: No change reported.

## App engine and films
- Job Engine: 2 of 4 agents finished. Running: build:worlds and build:speed, both Bash.
- Skills: 44. Decisions: 9.
- Commit 05d3a20 (24 Nov 09:20) reports stage engine test 1. Cheap-model films scored about 4 of 10. This is from the commit message, not a test shown in FACTS.
- Commit 3e91606 records the decision that LOT is 50-minute documentaries and old LOT is not a source.
- Film reader: 0 of 1 agents finished. Running: build:absorb. Its note now reads "Keep waiting and view the queue." Before, it read "Wait for tests and build, third window."
- Pull request #7, the sample film the rooms are drawn from, is open with checks SUCCESS.

## Web app and rooms
- No web app facts were reported.
- Rooms drawn: 19.
- Job Rooms: 3 of 8 agents finished. Five are running:
  - rooms:altar+2. Note changed to "Wait for truth on the final files."
  - rooms:crossroads+2. "Wait for full run a third time."
  - rooms:cauldron+2. "Patch look undo and wait for renders."
  - rooms:conjuring+2. "Collect faults from the sweep."
  - rooms:new-vessel+3. "Wait for interaction renders."

## Mac app and APK
- APK files built: 0.
- Mac load now [35, 41, 69]. It was [36, 43, 75].
- No Mac app facts were reported. Not tested.

## Agents running now
- Job Engine: build:worlds, build:speed (2 of 4 finished).
- Job Conductor: fix:r2 (10 of 11 finished).
- Job Rooms: five running, listed above (3 of 8 finished).
- Job Film reader: build:absorb (0 of 1 finished).
- Job Design systems: five teardown tasks running (0 of 5 finished). Notes:
  - teardown:ZgpMtombn9A: "Wait for bursts; show queue."
  - teardown:sJiaWNxYFUA: no note.
  - teardown:oRBu7wYuOSo: "Wait for frames."
  - teardown:G4w-a8NgnnQ: changed to "Wait up to nine minutes for lock jobs." Before, it was "Count distinct hedge footnotes and headers on code cards."
  - teardown:HmuQoak_IAg: "Wait for dates to finish."
- Job Page map: board-fix running (12 of 13 finished). Note changed to "Wait for the final build and push." Before, it was "Show where the placed ways out went, then start the final picture build and Doop push."
- Job Keys and PRs: 3 of 3 finished. None running.

## Money spent on services
- Paid calls in the test ledger: 991. Total $0.6938.
- deepseek $0.2899 (was $0.2627). openrouter $0.2217 (was $0.2098). google $0.1822 (no change).
- Wallet balances: not reported.

## Broken, blocked or open
- Design-system libraries: none on disk yet.
- Film reader and Design systems jobs are still running with no finished agents.
- Cheap-model film score about 4 of 10 (from commit 05d3a20). Newer tests not shown.
- Rooms still waiting on final truth files, a look patch, fault collection and interaction renders.
- Pull requests: 8 open, 0 merged, 0 closed. All checks SUCCESS.
- Lead has sent no messages and no day log entries.

## Waiting on Ambi
- No request to Ambi is stated in the messages or facts.























# Sheet of 13:25 EAT, Tue 24 Nov 2026

## Changed since the last sheet
The last sheet had no facts, so everything here is new.
- The test ledger shows 940 paid calls and $0.6548 spent.
- The lead's earlier spend figures ($0.44 at 13:17, $0.51 at 13:21) are superseded by the ledger.
- Google's direct key answers now. The lead reports billing was linked and the first paid call worked at 13:10. Earlier 429 refusals (12:51) are superseded.
- Eight pull requests are open, none merged. The lead corrected its "all checks green" claim at 13:21.
- All 19 rooms have a first build (ledger count). The lead's ADR 0009 on quiet screens is accepted.
- Mac load is now 36 (1 min), 43 (5 min), 75 (15 min). The lead reported 233 earlier.

## App engine and films
- Engine: 2 of 4 agents finished. Running: build:worlds and build:speed.
- The lead reports 9 world kinds drawn and 112 licensed pictures gathered (12:48).
- The lead's round 5 picture sheet is not yet scored by judges. Earlier scores were about 4 to 6 out of 10.
- A 187-second test render (12:10) had no fallback scenes and passed the safe-box check. It has no voice track and is one act only.
- Design systems: 0 of 5 agents finished. The five-film teardowns are still running. No design-system library exists yet.
- Film reader: 0 of 1 finished. build:absorb is running. The lead reports it is still building.

## Web app and rooms
- Rooms: 3 of 8 agents finished. Still running: altar, crossroads, cauldron, conjuring, new-vessel.
- The lead reports a price overlapping the list on the Cauldron phone screen (12:48). No fix is confirmed.
- The board (13:00) maps 329 room states at two sizes. The page map job is 12 of 13 finished, with board-fix still running. The desktop frames were empty earlier. A fix is not confirmed.
- ADR 0009 limits screens to 30 interface words on desktop and 24 on phone, with no text of 5 words or more.
- Outside critics have not reviewed the rooms yet (lead, 12:48).

## Mac app and APK
- APK files built: 0. APK not tested.
- Mac app: No change reported.
- The lead reports video work now runs one job at a time to protect the Mac (12:37).

## Agents running now
- Engine: build:worlds, build:speed (2 of 4 finished)
- Conductor: fix:r2 (10 of 11 finished)
- Rooms: five running, 3 of 8 finished
- Film reader: build:absorb (0 of 1 finished)
- Design systems: five teardown agents running, 0 of 5 finished
- Page map: board-fix (12 of 13 finished)
- Keys and PRs: none running (3 of 3 finished)
- The lead reports three test jobs (nuance, storyboard, packaging). They are not in the job list.
- The lead reports the Ancient Logos teardown has been silent since 13:14. Its status is unknown; the lead plans to check at 13:33.

## Money spent on services
- Ledger total: $0.6548 across 940 paid calls. DeepSeek $0.2627, OpenRouter $0.2098, Google $0.1822.
- Balances at 12:37 (lead): OpenRouter $18.82, DeepSeek $16.96, WaveSpeed $12.00. Not rechecked since.
- Inworld: key works, 407 voices listed, no charge. Making speech is not tested.
- Film cost estimates from 13:17: about $0.55 per 50-minute film on DeepSeek, $2.14 on GLM, at high or max thinking. The lead says 92 to 98% of output is hidden thinking. The lead says these are not yet shown to fit the agreed budget (13:21).
- Gemini cache: three repeat calls saved nothing. The lead corrected its earlier figure of five. The paid cache and batch route are not tested.
- Spend guard: each job has its own limit. No shared total limit exists yet. Worst case if all jobs hit their limits: $1.25 (lead, 13:21).

## Broken, blocked or open
- Engine drawing tests do not compile on main. PR 5 fixed the picture finder (26 of 26 pass). The drawing part is still red.
- PR 1 loosened checks, so green status is partial. PRs were tested alone, not together. Not merged.
- No shared spend limit yet.
- Ancient Logos teardown: status unknown since 13:14.
- Cauldron price overlap: not confirmed fixed.
- Board desktop frames: not confirmed fixed.
- Art direction: not judged.
- Voice: no voice track. Inworld speech is not tested.
- Film costs: not shown to fit the budget.
- Full run, script to finished film, on your keys: not tested.
- Repo: uncommitted changes exist (lead's count at 12:10: 205 files). ADRs 0008 and 0009 are untracked.

## Waiting on Ambi
Nothing is waiting on you (lead, 13:21).
