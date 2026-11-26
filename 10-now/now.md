# Juju now

As of 20:08 EAT, Thu 26 Nov 2026. Written every two hours by claude-haiku-5-5 (medium) from facts collected by code and the lead agent's own messages. Reports are not proof.

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

## Counted by code

- Pull requests: 8 open, 19 merged, 1 closed
- Paid calls in the test ledger: 10626, $36.0973 in all {deepseek: 11.0955, openrouter: 12.269, google: 8.3851, inworld: 3.9231, unsettled: 0.1365, lead-test: 0.0, wavespeed: 0.288}
- Paid services answering: deepseek 6531 ok, 23 refused or failed, last ok 26 Nov 17:52 EAT; openrouter 3411 ok, 47 refused or failed, last ok 26 Nov 16:38 EAT; google 119 ok, 16 refused or failed, last ok 26 Nov 13:59 EAT; inworld 458 ok, 1 refused or failed, last ok 26 Nov 10:54 EAT; unsettled 0 ok, 9 refused or failed, last ok None; lead-test 0 ok, 3 refused or failed, last ok None; wavespeed 6 ok, 2 refused or failed, last ok 25 Nov 11:24 EAT
- Rust: 37,404 lines in 15 crates. Skills: 59. Rooms drawn: 22. Decisions: 27. APK files built: 1
- Design-system libraries on disk: camera_motion.json, fonts, house, kits, looks, palettes.json, proof, proto, work-camera_motion, work-palettes, work-quotes, work-surfaces_light, work-typography
- Finish check: 1 of 23 clauses true, so not done
- Whole-film runs of `juju make` on disk: 4 DONE, 4 FAILED, 24 HOLD
- Newest film runs: ottoman12f HOLD 25 Nov 11:25 (stopped at Pictures and form); proof12c FAILED 25 Nov 09:47 (stopped at Render and mix); proof12 HOLD 25 Nov 09:16 (stopped at Script and heal); proof75b HOLD 25 Nov 09:06 (stopped at Render and mix); proof75a HOLD 25 Nov 08:59 (stopped at Publish kit); strip-planets HOLD 25 Nov 08:41 (stopped at Deal and package); strip-pluto HOLD 25 Nov 08:40 (stopped at Render and mix); 20261125-083722-131d HOLD 25 Nov 08:37 (stopped at Deal and package); strip-japan DONE 25 Nov 08:34 (60 s, 0.008751 US); strip-bulgaria HOLD 25 Nov 08:11 (stopped at Deal and package); strip-austria HOLD 25 Nov 08:11 (stopped at Deal and package); strip-manchuria HOLD 25 Nov 08:11 (stopped at Deal and package)
- Agent transcripts written to in the last 10 minutes (all Claude work on this Mac, mostly Juju): 0
- Logged attempts: 433 kept, 63 reverted, 52 inconclusive
- Mac load (1, 5, 15 min): [12, 13, 14]
- The live agent page did not answer, so running agents are unknown
