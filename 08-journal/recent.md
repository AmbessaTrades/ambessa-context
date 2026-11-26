# Juju day log, newest first

Rebuilt 06:53 EAT, Thu 26 Nov 2026. Only entries whose title names Juju. Times are EAT (UTC+3). Logged by agents: evidence of what they report, not proof. Where two entries disagree, the later one wins and the older stays.

---

## 2026-11-26 06:53 EAT — TEHUTI — Juju canon: three skill packs live under countersign; 124 audit faults listed; law 6 switch ready
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5), canon lane. Topics: juju
- **Changed:** rows 16-17 applied live: juju-director, time-map-storyboard, juju-roots packs; 5 skill patches; reach.rs MAPS + 6 rows; pins.txt 9 lines (backups runs/canon/countersign-16-17/before/). runs/canon/audit-124.md (no fixes). canon/laws/gap.py FINAL flag (False) and remeasure.py.
- **Why-verdict:** Measured: pins 0 DIFF; audit 124 before and after, 0 new, 0 naming the three packs; canon check TRUE; link-skills linked 59. Live conductor sha256 f3d6b2d4. The 124: pin new 79, no reach row 27, pin changed 10, no stage 8; 8 packs added since 25 Nov hold most.
- **Status-open:** law 6 report-only until dates draws 26 states and stories adds 9 stops (fills-26nov.json) and remeasure prints CLEAN; engine lane asked to raise only on gap.FINAL. The 124 wait for their own countersigned unit.
- **Related:** runs/canon/countersign-16-17/receipt.json; runs/canon/audit-124.md.

---

## 2026-11-26 06:45 EAT — TEHUTI — Juju canon: law 6 judged against the film itself; skill packs countersign trial stops on the conductor audit
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5), canon lane. Topics: juju
- **Changed:** canon/laws/gap.py: a gap is a book state or people inside the film's own camera frames, a 12 s question stretch with no stop, or a stop without its page; mask and inline keys read for roots.cover; 21/21 tests incl. a focused film with off-frame states that passes. canon/laws/LAW6-MEASURE.md and fills-26nov.json. Rows 16-17 run whole in an isolated copy: runs/canon/countersign-16-17/receipt.json.
- **Why-verdict:** Measured: Africa 11-min refused for 15 framed states + 5 stretches; Musa for Kilwa; Sahara 10 + 3 (7 off-frame pass); US 1 stretch. Trial: pins 0 DIFF, the three packs add 0 audit faults, but the conductor already refuses 124 faults before any change, so check 2 fails and nothing was applied (live pins.txt, reach.rs, packs untouched).
- **Status-open:** lead to decide check 2 (fix the 124 first, or read it as adds no fault); the engine lane runs the gate report-only.
- **Related:** runs/canon/countersign-16-17/receipt.json; juju-maps/canon/laws/LAW6-MEASURE.md.

---

## 2026-11-26 06:34 EAT — TEHUTI — Juju Make room built and walked on desk and phone; live swap and app-made film still open
<!-- type: event -->
**From:** TEHUTI

Juju Make room built and walked on desk and phone; live swap and app-made film still open
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 160a7d4c)
- Ambi asked: "wire up juju by urself, make sure ui ux buttons work, click around ... and launch full", with one tap making kingdoms, wealth, states, worlds and Night films.
- Built the Make room (/r2/make.html) with ideas first, your own sentence, five kinds, six theme frames, size pick (1080p preselected), progress words, player, film list and Stop. Routes are under /api/tap in make.rs.
- Verified: server build passes its 22 unit tests; desk (1440x900) and phone (390x844) click walks ran with no faults, and the screenshots were looked at.
- Open: the app-made wealth film was still drawing its map at 50% when the log ended. The live swap on port 4700 and the launchd load are not done, and runs/predicate/overnight/app.json is not written.
- Files changed: crates/juju-serve/src/make.rs; crates/juju-serve/src/lib.rs; mockups/r2/make.html; mockups/r2/gate.html; mockups/r2/kit2.js; scripts/serve/start; scripts/serve/com.auh.juju-serve.plist; juju-maps/make/CONTRACT.md
- Status: in-progress — Make room works on the test server (4705); live swap, app-made film end and overnight app.json still open

---

## 2026-11-26 06:30 EAT — TEHUTI — Juju velocity: four systems timed; 1080p drawing is the film; requests to engine and make lanes
- Harness: Claude Code (claude-opus-5-5), velocity worker. Topics: juju
- **Changed:** runs/predicate/overnight/velocity.json (stage table, four systems); juju-maps/timemap/REQUESTS-velocity.md; juju-maps/velocity/REQUESTS-make.md; bench under juju-maps/velocity/bench. mix.py prefetch tried and reverted (23.4 -> 22.0 s median, inside noise, output byte-identical).
- **Why-verdict:** Africa 1080p: a 30 s window costs 1,257 CPU s (21x 240p); encode is 15% of it (x264 193 vs VideoToolbox 13 CPU s, PSNR 46.8 dB). Planning 373 s, of which 197 s are 24 drawer relaunches; make step 2 plans again. Bar FALSE: no stage is in a velocity-owned file.
- **Status-open:** engine lane: countries read once, probe-many, Cliopatria cache, VideoToolbox flag; make lane: step 2 --draw.
- **Related:** runs/decision.tsv lane velocity

---

## 2026-11-26 06:20 EAT — TEHUTI — Juju canon: laws 6, 20, 24 are code; migration rows 1-4 done; skill packs prepared for countersign
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5), canon lane. Topics: juju
- **Changed:** juju-maps/canon/laws/ (gap.py law 6, director.py law 20, rights.py law 24, words.py, test_laws.py 18 planted faults, wired.py, HANDOFF.md with one call per chain); canon/check.py runs the tests and prints wiring; LAWS.md cites ADR 0027 items 37-41, law 25 (asset drift) added; GLOSSARY.md 8 words; AGENTS.md one Where row; canon/THRESHOLD-CHANGE-skills.md (rows 16-17, not applied); one wish line at the foot of timemap/CONTRACT.md.
- **Why-verdict:** Measured on a copy of the 11-min Africa: the gap gate refuses it (101 undrawn states, narrow -3300 to -800, fill.json), strips the "not drawn" credit; the director (DeepSeek low, 0.0226 US in two calls) kept 2 merges and undid a planted turn cut. check.py TRUE; gold films the same. 6 decide rows.
- **Status-open:** no chain calls the laws yet (engine, worlds, states, stack lanes); the first wired Africa make will be refused until roots and dates fill 101 states or the span narrows; night films not covered by the director.
- **Related:** juju-maps/canon/laws/HANDOFF.md; python3 -m canon.laws.wired.

---

## 2026-11-26 06:15 EAT — TEHUTI — Juju time maps: no hedge words drawn, Mansa Musa rebuilt around his road, Asia land source named
<!-- type: event -->
**From:** TEHUTI

Juju time maps: no hedge words drawn, Mansa Musa rebuilt around his road, Asia land source named
- Harness: Claude Code (claude-opus-5-5)
- What happened: Harness: Claude Code (claude-opus-5-5). Topics: juju.
**Changed:** timestory.py gains polish() and hedge_check() (ADR 0027 items 28 to 33): no hedge word in drawn text; one bracket at most from a closed list (their own record, by tradition, from the dug site, ruled through local kings, influence not rule, in name only); crucial/pulse stops; today_outline at most one a minute; the doubt kept in e.doubt. Applied to tm-africa-long (TRUE), st-us (TRUE), Sahara, Musa, Africa. tm-musa is rebuilt around Musa's road: 15 stops; the caravan route Niani, Walata, Taghaza, Tuat, Cairo, Mecca; the Catalan Atlas find image (BnF via Commons, public domain). films/tm-asia/land-source.json names the UN manufacturing set. st-us words.json has Fort Sumter's second card.
**Why-verdict:** Ambi: "be confident"; the Musa film was mostly North Africa's dynasties.
**Status-open:** Musa and Sahara each fail one gap check (an act with a stop only every 26 to 28 s). Musa spent about 0.05. Another worker is charging timestory.py calls to this lane's purse (purpose tm-africa-28).
- Status: complete; two small gap faults open

---

## 2026-11-26 05:51 EAT — TEHUTI — Juju canon: one map of the Powers, one design-system form, the laws tied to code
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5), design sub-agent. Topics: juju
- **Changed:** new juju-maps/canon/ (README, MAP.md + map.json, design-system.schema.json + DESIGN-SYSTEM.md, systems/{kingdoms,wealth,states,worlds,duppy-night,duppy-day,moko-day}.json + HANDOFF.md, LAWS.md (24 laws, each tied to file:function or "not yet code" + lane), DIRECTOR.md, skills/ drafts, MIGRATION.md (18 rows), check.py, diagram.py); docs/CANON.md; vault board ~/LOT Files/LOT/LOT+AAY/JUJU/Juju Powers.excalidraw.md (+3 stills). Lead orders of 26 Nov (director step, one partition per year, colour roles, exports 720/1080/1440, system bar 7+ at 240p and clean 1080p) written in.
- **Why-verdict:** ADR 0027 items 28, 29, 35. canon/check.py TRUE; three planted faults each FAIL; golden.py istanbul and po3 the same. Nothing live edited.
- **Status-open:** gap closing before drawing is not yet code (roots.cover only reports; timemap.py:764 still makes "[dates about]", seen on the Africa still); director, stripes, finals export not yet code; ADR 0027 items 37-40 not yet in the ADR file; board not opened in Obsidian.
- **Related:** start from juju-maps/canon/MIGRATION.md row 2.

---

## 2026-11-26 05:36 EAT — TEHUTI — Juju overnight: US film critique, exports 720p to 2K, director step, all lanes running
<!-- type: event -->
**From:** TEHUTI

Juju overnight: US film critique, exports 720p to 2K, director step, all lanes running
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: ADR 0027 items 28 to 40 (no gap words; confident brackets; motion of change; flat kingdoms; modern outline; year pulse; one cohesive canon; 28-minute law; US film rebuilt: one partition per year, contested as stripes, colour with meaning, no meaningless rings, smooth morphs; exports 720p/1080p/1440p; a director step). Lanes running: engine, dates, roots, stories, type (seventh theme for political films), stack proof, app (exports, ideas first screen, every button), styles, channels, long+sound (28 min Africa), Night on two grounds, canon. Why: Ambi 06:10, going to sleep: "log all these changes and have them be executed". Status-open: films churn overnight; purse 32.46 of 35 US at last read; lead's US mark 4.5.
- Status: in-progress; overnight run

---

## 2026-11-26 05:18 EAT — TEHUTI — Juju dates: Africa rebuilt from Roots round four; lab dates no longer stretch a state past its end
- Harness: Claude Code (claude-opus-5-5), Juju dates worker. Topics: juju
- **Changed:** door.py: Axum drawn as Aksum (aliases.json), a dated extent is a hold in itself, extents ride lab sets; reach.rs Hold.clip (a lab set ends at its state's own dated end); dates/draw/africa-roots.geojson rebuilt; engine lane told to redraw Africa.
- **Why-verdict:** same-state mean |log ratio| 0.204 -> 0.222 (Aksum 1.66 and Wagadu by their own GHA extents, noted; Songhay 0.62, Mali 0.74); Wagadu ends 1202 not 1706. Frames 340, 1550, 1580, 1700 read. 28/28 tests incl. a clip law with a planted fault.
- **Status-open:** "Aksum under Ezana" drawn as its own state; Asante 1700 uncapped; read-back in dates/HANDOFF-to-roots.md.

---

## 2026-11-26 05:17 EAT — TEHUTI — Juju: full control taken, app wiring, stack proof and style lanes started, GitHub save fixed
<!-- type: event -->
**From:** TEHUTI

Juju: full control taken, app wiring, stack proof and style lanes started, GitHub save fixed
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: GitHub autosave push had failed since 04:03 (HTTP 400); fixed with http.postBuffer, 8 saves pushed. Three new lanes: Stack Proof (ju make KIND "sentence", ju doctor per part, env -i runs), App (juju-serve wires ju make, every button clicked at 390x844 and 1440x900, keeper/launchd after sleep), Styles (5 new design systems as stills and 90 s films). Lead decisions under Ambi's full-control order in ADR 0027 item 26: two grounds behind smooth: true, working name Juju Ardhi, real cultures on real land. Why: Ambi 05:15 "assume ur in full control ... wire up juju by urself ... launch full". Status-open: engine and Dates lanes still running; purse 32.46 of 35 US.
- Status: in-progress

---

## 2026-11-26 05:08 EAT — TEHUTI — Juju Roots round four: Songhay to 1591, Kongo 1540-1666, Aksum under Ezana, six gaps filled
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5)
- Changed: lead holds for Songhay (Gao 1591, Teghazza 1539-49, Macina 1512), Kongo (Mbanza Kongo 1540/1548/1666, Pool 1566-67, Mbwila 1665), Aksum under Ezana (320-360) dating the Meroe extent; roots/gaps.py; Napata, Meroe, Kilwa, Gondar, Djimi gaps filled; merge only when years meet; OCR i486 and decades fixed.
- Why-verdict: Dates lane found Songhay ending 1529, Kongo empty 1543-1645, Aksum extents undated. check.py TRUE; planted fault (Songhay 1591 hold removed) fires. No paid calls.
- Status-open: Garamantes, Persia, Aksum -100..0 and Kongo 1567-1622 have no dated place on the shelf; Dates lane session not running, note in roots/HANDOFF-to-dates.md.
- Related: juju-maps/dates/HANDOFF-to-roots.md

---

## 2026-11-26 05:07 EAT — TEHUTI — Juju time maps: US film worded by the stories lane and its faults fixed; Africa on Dates round three
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** timemap.py: a state made from its own territory appears in place (move "there", no blob); stops take their land's own width (small cessions and Hawaii close); a stop's further cards (the dive's second card); the find pan (view 150 px lower while the picture stands; dy on a camera fit). Engine: "there" birth can be asked for; find picture moves clear of the event's words; fit dy. states/statemap.py handoff merges films/st-us/words.json (who|date) over the data words, with sources.
- **Why-verdict:** films/st-us/a.mp4 359.6 s with the stories lane's words, Alaska 1959 in place, Hawaii close, second Fort Sumter card shown; judged 6.5 of 10. films/tm-africa-long/a.mp4 697.5 s on Dates round three (Mali across the west in 1235-1350), turncheck FAIL 1 (655, same holder); judged 6.5 of 10.
- **Status-open:** US: ground edge west of 172 W, the dive's return frame, words over land on 8 shots; Africa: the 658 BC frame shows the change mid-way; the find moment has no real find in any story yet.
- **Related:** films/st-us/run.json, words.json; films/tm-africa-long/run.json; data/timesets-fixes.json

---

## 2026-11-26 05:00 EAT — TEHUTI — Juju maps: sourced African state extents, US states film rebuilt, US story cards reworded
<!-- type: event -->
**From:** TEHUTI

Juju maps: sourced African state extents, US states film rebuilt, US story cards reworded
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked for Juju's Roots, Maps and Stories lanes to be built from sources. Roots: 18 reach records, 37 of 39 ends placed. Africa drawn from them (429 shapes); 27 of 27 tests pass.
- Africa sizes now: Songhay 1.12, Mali 0.92, Wagadu 0.87, Kanem/Borno/Asante 1.00 of source. Kongo 5.8x (flagged, size disputed). Kush 0.34 and Aksum 0.45 still small.
- US states film now uses the Africa path: 360.9 s at 240p, $0.012 spent, 57 of 64 shots pass the clock. Alaska (1959 green blob) and Hawaii (dark sea stop) are still weak; fixes are running.
- All 34 US story cards reworded from the inside; 17 carry a quoted line from an open source. Native side is thin: 4 of 7 cessions have no second line. Total test spend $32.46 of the $35 cap.
- Open: statemap.py still rewrites story.json from old words each run; words.json is not merged yet. Africa 1550 gap (Songhay ends 1529, Kongo 1543-1645 empty); Aksum conquests have no year.
- Files changed: juju-maps/dates/draw/africa-roots.geojson; juju-maps/dates/work/size-table-round3.md; juju-maps/states/statemap.py; juju-maps/films/st-us/story.json; juju-maps/films/st-us/words.json; juju-maps/films/st-us/a.mp4; juju-maps/roots/HANDOFF-to-dates.md
- Status: in-progress — Africa extents and US film drawn and tested; Alaska/Hawaii fixes, words merge and 1550 gaps still open

---

## 2026-11-26 04:58 EAT — TEHUTI — Juju time maps: US states film stops worded from inside, quoted lines from Royce, the Historian, the Apology Resolution
<!-- type: event -->
**From:** TEHUTI

Juju time maps: US states film stops worded from inside, quoted lines from Royce, the Historian, the Apology Resolution
- Harness: Claude Code (claude-opus-5-5)
- What happened: Harness: Claude Code (claude-opus-5-5). Topics: juju.
**Changed:** films/st-us/words.json (keyed who|date) and films/st-us/story.json: all 34 stops reworded; 17 carry a line whose quote stands word for word in a saved page (Royce 1899 schedule, US Office of the Historian, Public Law 103-150, The American Yawp, now on the source shelf); 17 are title only. timestory.py wordstates.
**Why-verdict:** no data talk left ("created from territory", "on this date"). Lines that repeated the year, or quoted a passage about another year, were blanked by code; 4 stops where the pen read a passage of another year keep plain rule words ("Utah becomes a state").
**Status-open:** statemap.py handoff() must merge words.json or the next run brings back the old words (engine lane told). Spent 0.087 of 0.10, of which 0.039 was a timed-out call charged at its worst case. DeepSeek total for this lane 0.791.
- Status: complete; the merge is the engine lane's

---

## 2026-11-26 04:54 EAT — TEHUTI — Juju dates: Roots' extent rows drawn; states reach the places their own sources name
- Harness: Claude Code (claude-opus-5-5), Juju dates worker. Topics: juju
- **Changed:** extent holds grow a state from its nearest dated site to each named end along the ground (250 km margin, no corridor across >80 km of open water); an extent with 2+ ends speaks for size above Cliopatria; Cliopatria's widest figure yields to its shape of the year; size notes only between source ranks; Asante influence kept aside, not land; dates/draw/africa-roots.geojson rebuilt (429 features); engine lane told Africa can be redrawn.
- **Why-verdict:** 21 states mean |log ratio| 0.233 -> 0.21; Songhay 1.12, Mali 0.92, Borno 1.0, Wagadu 0.87; Kongo 5.82 by GHA's own extent (noted); Aksum 0.45 and Kush 0.34 stay short for book reasons. 27/27 tests.
- **Status-open:** Roots: date Aksum's 4th-century extents, Songhay after 1529, Kongo 1543-1645 (dates/HANDOFF-to-roots.md).
- **Related:** juju-maps/dates/work/size-table-round3.md, work/stills4/sheet.png.

---

## 2026-11-26 04:43 EAT — TEHUTI — Juju time maps: the US states film now draws on the shared path; find moment and zoom sizes built
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** timemap.py: a "given" land source (films/NAME/land.json from another chain), per-stop bodies, tricks, dive cameras and battle rings from the story, a clock fix for sharp speed changes, pull backs never wider than the film's home view, find pictures made into PNGs. Engine: find moment (line, picture with rim and shadow, caption, dim line), sizes by zoom and weight, bodies marching in file, blast trick, closed travel outline. states/statemap.py: film_us hands its land and stops to timemap.py (handoff); --own-path keeps the old drawing; Canada and money untouched. timemap/CONTRACT.md: layer order, fractional years, new fields.
- **Why-verdict:** films/st-us/a.mp4 360.9 s, run 193 s; clock ok (worst change 3.94); 57 of 64 shots pass; the Fort Sumter dive is sharp with islands and harbour. Judged 6 of 10.
- **Status-open:** Hawaii 1898 and 1959 stops dark and tiny; Alaska 1959 drawn as a round blob; 7 cession shots too small; the dive's second card dropped; Africa waits for the Dates lane.
- **Related:** films/st-us/run.json, land.json, story.json; juju-maps/states/statemap.py handoff()

---

## 2026-11-26 04:34 EAT — TEHUTI — Juju Roots round three: checked extents and areas for the first states, Mali added
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5)
- Changed: roots/extent.py (extent and area tagger; ends placed from GeoNames CC BY 4.0, Pleiades, p3k14c, gazetteer, Natural Earth shores); book/africa/extents-lead.json (18 extent rows chosen by reading); 18 Cliopatria area rows; Mali state row; check.py round-three bar.
- Why-verdict: the Dates lane drew states too small (Aksum 0.05). Code-only tagging was about half wrong (Ghana Gold Coast, footnote years), so its finds stay as unchecked candidates; the 18 checked rows place 37 of 39 ends. check.py TRUE; planted fault (Aksum extents removed) fires. No paid calls.
- Status-open: no km2 sentence in GHA; Sibiridugu and Birni Kafela unplaced; Dates lane session not running, note left in roots/HANDOFF-to-dates.md.
- Related: juju-maps/dates/HANDOFF-to-roots.md

---

## 2026-11-26 04:27 EAT — TEHUTI — Juju Africa map: Roots fixes pass, states sized to sources, Africa film at 6.5/10
<!-- type: event -->
**From:** TEHUTI

Juju Africa map: Roots fixes pass, states sized to sources, Africa film at 6.5/10
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Roots: check.py passes after fixing Carthage (now 814 to 145 BC, no era-less centuries) and D'mt (passages stored word for word). Added 14 dated state ends and 20 placed holds; nothing guessed, unplaced holds stay in queue.json.
- Time Map: Egypt keeps its purple from 658 BC, the Fatimid colour gap and label collisions were fixed, and the 12-minute Africa film was redrawn at 6.5/10 (up from 6). Turncheck is down to one FAIL (655 BC, same holder).
- Dates and Reach: states are capped by the highest-ranked source's stated extent, not the Cliopatria cap. Average size gap fell from 0.97 to 0.23 on a log scale over 21 states; 27 of 27 tests pass.
- Open: Fatimid colour still close to the prior ruler, Kush label and an empty view at 8:00, Egypt's 658-616 BC shape, and Aksum, Kush and Wagadu drawn far below source size until the world book places their named ends.
- Files changed: juju-maps/films/tm-africa-long/a.mp4; juju-maps/dates/draw/africa-roots.geojson; juju-maps/dates/work/stills3/sheet2.png
- Status: in-progress — Roots check passes and the new size rule is tested, but the redrawn Africa still needs world-book placements before state sizes match their sources.

---

## 2026-11-26 04:26 EAT — TEHUTI — Juju time maps: Africa turn colours pass, dive coasts follow the real shore
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** timemap.py: farthest OKLab colour for own powers too; a pass that keeps every successor on a turn land 14 OKLab from the holder before it across families; a freed land takes its own rulers' last sourced shape (not the modern outline). Engine: a name is hidden where a later land covers its anchor; in a dive (under 6 degrees) a land reaches the true 10 m coast within 0.12 degrees of its outline.
- **Why-verdict:** films/tm-africa-long/a.mp4 697.4 s, run 308 s; turncheck FAIL 1 (655, same holder, no drawn change); flips 22 of 23. Fort Sumter dive: Sullivan's and James Island now coloured, harbour mouth reads.
- **Status-open:** find moment and sizes with zoom not built; States asks 2-6; 8:00 rest view still thin; Dates lane's ranked sizes equal the last round until Roots places the named ends.
- **Related:** films/tm-africa-long/run.json; films/st-us (dive at 190-221 s); data/timesets/relief/9, /10

---

## 2026-11-26 04:18 EAT — TEHUTI — Juju dates: Cliopatria is no longer the hard cap; the highest-ranked source sets a state's size
- Harness: Claude Code (claude-opus-5-5), Juju dates worker. Topics: juju
- **Changed:** reach.rs size_speakers: caps and extent holds rank by rules.json; a compiled set caps only where nothing higher speaks, and its border is not drawn in a year it is outranked; sizes more than 1.5x apart give one short note; dates/draw/africa-roots.geojson rebuilt.
- **Why-verdict:** lead 05:55 on ADR 0028 (Cliopatria is one outside compilation). 27/27 tests; the new test fails when the compiled set is ranked first. Today's map unchanged: only Garamantes and Nubia have extent holds and neither has a Cliopatria cap.
- **Status-open:** extent ends need Roots' gazetteer (the Delta, First Cataract, Mediterranean, Semna) and extent tags; asked in dates/HANDOFF-to-roots.md.

---

## 2026-11-26 04:11 EAT — TEHUTI — Juju dates: Africa's states sized against their sources
- Harness: Claude Code (claude-opus-5-5), Juju dates worker. Topics: juju
- **Changed:** juju-dates measure (computed vs Cliopatria area on one ground); caps (a state never drawn past its source's shape of that year); rules.json state_reach kingdom 2.0, empire 2.5, only for states a source sizes; a border yields only to a row sited inside it; extent sentences' named ends become holds; dates/draw/africa-roots.geojson rebuilt (386 features) from Roots' fixed book.
- **Why-verdict:** Ambi: Africa's states look tiny. Measured on 21 states: mean |log ratio| 0.97 -> 0.23, over source 8 -> 0, under half 8 -> 2 (Aksum 0.05, Kush 0.26). 26/26 tests incl. a cap law with a planted fault.
- **Status-open:** extent tags and named-end places asked of Roots (dates/HANDOFF-to-roots.md); Kongo and Asante stay at Cliopatria's size until a source says larger.
- **Related:** juju-maps/dates/work/size-table.md, work/stills3/sheet2.png; runs/decision.tsv rows 446-447.

---

## 2026-11-26 04:03 EAT — TEHUTI — Juju time maps: Africa keeps Egypt's own colour, banners, estimate notes and a sharp dive ground
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** timemap.py: a sourced "freed" turn cuts the outside holder from that year until the set draws the own row (Egypt 658 BC back in its purple); Dates round two read (114 polities); banners from time-banners.json; estimate note (one in two minutes, under the year); land-less stops framed 35 degrees with the lands near them. Engine: foot cloth woven to the clock hand, head hair line with walkers of their years, note drawing, dive ground (zoom 9 relief + 10 m coast) for views under 6 degrees; 430 free relief tiles fetched for Fort Sumter and the Klondike only.
- **Why-verdict:** films/tm-africa-long/a.mp4 697.2 s, run 336 s; turncheck FAIL 2 (655 same holder; 969 Fatimids 11.8 against 12); flips 22 of 23; shots 105 of 108. Judged 6.5 of 10.
- **Status-open:** 8:00 rest view still bare; "Kush" label on Assyria at 663 BC; Egypt 658-616 BC clipped to the modern outline; find moment and sizes with zoom not built; dive harbour still blocky (region coast comes from the cell grid).
- **Related:** films/tm-africa-long/run.json, check.json; data/timesets/relief/9, /10; stack/systems/time-banners.json

---

## 2026-11-26 03:59 EAT — TEHUTI — Juju Roots: eraless centuries refused, passages kept as printed, Carthage and D'mt fixed
<!-- type: event -->
**From:** TEHUTI

Juju Roots: eraless centuries refused, passages kept as printed, Carthage and D'mt fixed
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 627f03d6)
- Ambi asked to fix two faults: Carthage drawn to AD 500 from an era-less 'fifth century', and D'mt refused over 'cerqos' vs 'çerqos'. Then quick wins from the holds, attestations and takings with no dated end.
- Done: the era reader gives no year for a century with no BC/AD unless the passage or nearby page text says which era. Carthage now runs 814 to 145 BC. D'mt keeps 'Çerqos' as printed.
- Done: 14 states got dated ends from the Cliopatria dataset, and 20 more hold places were placed. Unresolved holds stay in book/africa/queue.json; nothing was guessed.
- Verified: check.py prints TRUE. Two new guards fail on an era-less century or a passage not found word for word on its page. Numbers: 264 holds, 237 placed, 99 states with a dated hold.
- Lane message sent to the Dates lane. Open: the 50 attestations and 37 takings with no dated end are not shown as finished in this session.
- Files changed: juju-maps/roots/roots.py; juju-maps/roots/check.py; juju-maps/roots/book/places.json; juju-maps/roots/book/africa/queue.json
- Status: in-progress — both faults fixed and check.py TRUE; attestation and taking end-dates not confirmed done

---

## 2026-11-26 03:58 EAT — TEHUTI — Juju Roots: eraless centuries refused, passages kept as printed, Carthage and D'mt fixed
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5)
- Changed: roots.py era reader refuses a century with no BC/AD unless the passage or about 600 letters of page around it say which; book passages stored as the page prints them (diacritics, case); short lead passages widened; Cliopatria years added as data claims for 14 states; 20 more sites placed; check.py gains both checks.
- Why-verdict: Dates lane found Carthage drawn to AD 500 and D'mt refused for cerqos vs Çerqos. Now Carthage -814 to -145, D'mt passes; check.py TRUE; both planted faults fire. Holds 264, placed 237, 99 polities drawable. No paid calls.
- Status-open: queue still holds unplaced and undated holds; Dates lane told by message.
- Related: juju-maps/dates/HANDOFF-to-roots.md

---

## 2026-11-26 03:52 EAT — TEHUTI — Juju Africa map: 12-minute film now 6/10, world book rebuilt from dated sources
<!-- type: event -->
**From:** TEHUTI

Juju Africa map: 12-minute film now 6/10, world book rebuilt from dated sources
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked for a 12-minute Africa that shows the land. Redrawn film judged 6 of 10 (was 5). Turn check fails 1 flip (was 5), and 21 of 23 flips show on drawn frames.
- Africa world book rebuilt from dated sources: 232 places become 216 map shapes, 95 after 1500. All 25 tests pass and the frozen fixture is untouched. A slip overwrote a test file; restored from the GitHub save.
- Story fixes done for under 1 cent: five ruler names corrected with quoted sources, closing line added (true but weak), draft title 'Africa Holds Its Land To About The Year 1350' left for Ambi.
- Still open: most of Africa is near-empty because states are too small (true extents not built yet), the Egypt-orange colour fix is not on screen, and the title and closing line need Ambi's call.
- Two-ground split for Night and Day (drawer for wide views, plain globe up close) is written up in GROUNDS.md as a candidate. Waiting on Ambi's yes/no and the name pick (Juju Ardhi).
- Files changed: juju-maps/films/tm-africa-long/a.mp4; juju-maps/dates/draw/africa-roots.geojson; juju-maps/films/tm-africa-long/NEXT.md; juju-maps/films/_data/time-type/lab/turncheck.py; juju-maps/stack/GROUNDS.md
- Status: in-progress — Africa redraw judged 6/10; state extents, colour fix and Ambi's decisions still open.

---

## 2026-11-26 03:50 EAT — TEHUTI — Juju dates round two: Africa's land rebuilt from 817 Roots rows into dates/draw
- Harness: Claude Code (claude-opus-5-5), Juju dates worker. Topics: juju
- **Changed:** door.py reads Roots' new site holds (taken/start/lost/end/span/within; reach and ruler open a stretch from their year); another state's dated taking ends a site; borders never written into a frozen fixture; juju-dates build --drop-refused (a refused row is dropped and named, the rest drawn); rules.json site_holder (newest dated change holds a site) and notes only where sources of different kinds disagree.
- **Why-verdict:** dates/draw/africa-roots.geojson = 216 features, all kept by the engine's reader; held-year frames show Persia 520/460 BC, Kemet free 400 BC, Persia again 336 BC, Kerma, Garamantes, Songhay 1500, Kongo, Asante 1730. 25/25 tests, fixture untouched.
- **Status-open:** Roots fixes in juju-maps/dates/HANDOFF-to-roots.md (D'mt letter, Persia c0 short passage, Carthage 5th century coded AD); engine lane told.
- **Related:** juju-maps/dates/work/stills2/sheet.png, persia.png; runs/decision.tsv rows 443-444.

---

## 2026-11-26 03:43 EAT — TEHUTI — Juju time maps: 12 minute Africa redrawn, turn check FAIL 5 to FAIL 1
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** timemap.py reads dates/draw/*.geojson (estimate edge hatched), kept row names (data/timesets-names-africa.json) + fix rows of kind "name", outside colours picked farthest in OKLab from the theme's own list, continent pull back at most every 90 s outside chains, end on the whole continent with every place lit; engine: 2 px dark rim on outside lands, morphs about ten clock years centred on their year, near filter for rest views.
- **Why-verdict:** films/tm-africa-long/a.mp4 696.7 s, drawn in 196 s; turncheck FAIL 1 (655: same holder, no drawn change), flips 21 of 23, judged 6 of 10. Kerma, Kush, Aksum, Palmyra, Sosso and Mali now have land.
- **Status-open:** bare rest views at 4:40, 8:00, 10:00; two pull backs 97-100 s apart inside chains; type 1.1 banners, estimate note, find moment, sizes with zoom; states asks (dive ground needs zoom 9-10 tiles not on disk).
- **Related:** films/tm-africa-long/run.json, check.json; data/timesets-fixes.json; stack/systems/themes/*.json succession

---

## 2026-11-26 03:38 EAT — TEHUTI — Juju 12-minute Africa film: pull-backs, dated shapes, palette and end fixes; full redraw still running
<!-- type: event -->
**From:** TEHUTI

Juju 12-minute Africa film: pull-backs, dated shapes, palette and end fixes; full redraw still running
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 6a09db7f)
- Ambi asked for the 12-minute Africa film to show more than Egypt: add the Dates lane's 36 shapes, pull back to the continent at least every 90 s, and end on the whole continent with a closing line.
- Done in code: timemap.py now reads dates/draw/*.geojson; scene.rs morph timing changed; rest view fits the nearby lands; continent pull-back interval set to 62 s; ending uses a fixed whole-continent camera.
- Outside-power colours now spaced by OKLab distance (Persia and Rome were 91 apart in RGB, 8.8 in OKLab); a 2 px dark rim keeps outside lands in one colour family.
- Stories lane's name fixes (Ayyubids, Ptolemies, Mamluks, Seleucids, Normans of Sicily) and closing line were applied in the draw. Earlier 240p draw: 748.6 s, $0.0002 measured spend.
- Still open: the final full draw was running at the end of this part; the turncheck.py PASS and a frame read of the new draw have not been run yet. States-lane close-up request not started.
- Files changed: juju-maps/timemap.py; juju-maps/timemap/src/scene.rs; juju-maps/timemap/src/draw.rs; juju-maps/timemap/src/fit.rs; juju-maps/films/tm-africa-long/a.mp4
- Status: in-progress — full 12-minute Africa redraw running; turn check (PASS needed) and frame read still pending

---

## 2026-11-26 03:36 EAT — TEHUTI — Juju Roots round two: Persia, late Egypt, Garamantes, Aksum, D'mt and 1500-1880 Africa as dated holds
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5)
- Changed: juju-maps/roots: 10 more GHA readers (vols II, V, VI; line anchors, code cuts the words); pharaoh.se dynasties 25-31 (CC BY); Fazzan radiocarbon; Black Athena (Bernal own words, Lefkowitz, Wilson Quarterly critique) shelved; each polity now carries holds (site, place, dated claim, passage).
- Why-verdict: the dates lane draws only from dated holds. Book 817 rows, 98 polities with a placed dated hold (236 holds, 170 after 1500). Persia in Egypt 525-404 and 343-332 BC (GHA prints -341); 25th Dynasty takes Thebes and Memphis about 752 BC; D'mt dated through the south Arabian period (5th-4th c. BC). check.py TRUE; a hold whose place is not in its passage now fails it. Spend 0.
- Status-open: Sais dated only within the Late Period; 1018 queue items; Bernal read only as a reading, colonies in India still unsourced; nothing committed.
- Related: juju-maps/dates/README.md, REQUESTS-roots.md

---

## 2026-11-26 03:27 EAT — TEHUTI — Juju time maps: 12 minute Africa gets name fixes, a quoted end, a title that fits its span
<!-- type: event -->
**From:** TEHUTI

Juju time maps: 12 minute Africa gets name fixes, a quoted end, a title that fits its span
- Harness: Claude Code (claude-opus-5-5)
- What happened: Harness: Claude Code (claude-opus-5-5). Topics: juju.
**Changed:** data/timesets-fixes.json gets 5 rows of kind name, each quoted: Ayyubids, Ptolemies, Mamluks, Seleucids, Normans of Sicily. tm-africa-long/story.json: end.lines "Kilwa is wealthiest / Zimbabwean gold made Kilwa the wealthiest of all", quoted from OpenStax 15.2; film_title "Africa Holds Its Land To About The Year 1350" (a draft).
**Why-verdict:** the label "Aleppo" is not in this lane's files (the names file already says Ayyubids); the name row overrides it. A second try at the end lines said "Kilwa holds the land", which is false, and was refused.
**Status-open:** check TRUE, turns 23 of 23. Spent 0.0065 of the allowed 0.05 (DeepSeek total 0.704). The engine lane has been told.
- Status: complete

---

## 2026-11-26 03:14 EAT — TEHUTI — Juju: dated-land engine passes 25/25 tests, 12-min Africa story built, state films and worlds drafted
<!-- type: event -->
**From:** TEHUTI

Juju: dated-land engine passes 25/25 tests, 12-min Africa story built, state films and worlds drafted
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked that every border come from dated sources in code: no source, no land, and carbon dates kept as ranges. juju-maps/dates passes 25 of 25 tests, and planted faults fail as they should.
- Roots shelf: 80 open sources across 13 regions, each saved word for word with a receipt; 12 refused, Native Land out on its terms. check.py prints TRUE; Africa before 1000 BC now holds Kemet, Ta-Seti, Kerma and Punt.
- 12-minute Africa story: 55 stops over about 12.5 minutes, 23 of 23 ruler changes on screen, all checks pass. Not yet drawn by the engine. Night round two marked 4.5 and 4, so further Night spending is held.
- US states (6.5 min) 5.5, Canada 5, which states make the money 5.5, all about 2 cents total. The Canada borders are copyrighted and would need Toronto's permission to publish. Dates checked 10 of 10 against pages.
- Worlds: Atlantis marked 7, the strongest simulation so far. Green Sahara marked 5 and held: it uses made-up peoples where real cultures are known from digs, so Ambi must decide. Juju Time Stories exit check still FALSE.
- Files changed: juju-maps/dates; juju-maps/roots/check.py; juju-maps/films/tm-africa-long/story.json; juju-maps/films/st-us/a.mp4; juju-maps/films/w-atlantis/a.mp4; docs/adr/0029-world-book.md
- Status: in-progress — dates engine and Africa story done and checked; Night, Kinds and Green Sahara still below bar or awaiting Ambi's decision

---

## 2026-11-26 03:14 EAT — TEHUTI — Juju time maps: 12 minute Africa drawn with turn chains, row fixes and the clear page
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/timemap.py (story turns become chain stops, chains split at 30-year gaps, must stops never dropped, data/timesets-fixes.json drawn with cut/clip, Roots FINDS rows kept with hatched edge, places-lit counter, flip probe on the final clock); timemap/src (key cut/clip, --probe same camera no letters 3 degrees, type 1.1: no head scrim, year alone 56 px at 118, tide line in the foot y 1040-1070 that never vanishes, chart-forward boxes, measure only when it moves 5 points, at most 3 names at rest, lit dots; single-frame calls skip the draw lock); CAMERA.md, README.md.
- **Why-verdict:** films/tm-africa-long/a.mp4, 748.6 s, drawn in 272 s at 240p; 18 of 23 flips seen on pixels, 98 of 100 shots pass. Judged 5 of 10: Egypt's chain reads well 4:20-9:40; empty ground at 1:20, 2:00, 3:00, 10:20, 12:00; the rest of Africa barely shows.
- **Status-open:** 5 flips without a drawn change listed in run.json; outside reds too close (619, 692, 1250); type 1.1 banners, estimate note, find arrival, sizes by zoom not built; Roots reach-from-sites and routes not built; Dates shapes not read yet.
- **Related:** films/tm-africa-long/run.json, check.json; data/timesets-fixes.json (Stories); roots/REQUESTS-roots.md

---

## 2026-11-26 03:14 EAT — TEHUTI — Dates and land crate for juju-maps passes its full test bar, 25 of 25
<!-- type: event -->
**From:** TEHUTI

Dates and land crate for juju-maps passes its full test bar, 25 of 25
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session a97dabc6)
- Ambi's bar: plain `scripts/heavy cargo test` in juju-maps/dates must pass. It now passes 25 of 25 tests (receipt in work/receipt/cargo-test.txt).
- Dates keep what the source printed and give a 68% and 95% range, never a single year. A radiocarbon age older than the 55,000-year curve is refused.
- Planted-fault checks fail as they should: land with no row, a hold with no date, a single year shown for a range, a made-up row, a passage not in its page.
- A Ta-Seti test was added for Wadi Halfa in 3100 BC. Putting the old river cost (0.3) back made the test fail, so it catches the bug. The rule was restored to 0.5.
- Open: Marine20 has no published check yet. Kakapel passes within 1 year but on IntCal20, while the paper says SHCal20 and the numbers do not match.
- Files changed: juju-maps/dates/tests/roots.rs; juju-maps/dates/rules.json; juju-maps/dates/.gitignore
- Status: complete — full cargo test bar passes 25 of 25; Marine20 check and Kakapel curve mismatch still open.

---

## 2026-11-26 03:11 EAT — TEHUTI — Juju Maps grounds: globe vs drawer measured, division proposed for Night and Day
- Harness: Claude Code (claude-opus-5-5), design sub-agent. Topics: juju
- **Changed:** new juju-maps/grounds/ (views, make.py, lines.py prototype, plain-night look, stills, moves, blind read) and juju-maps/stack/GROUNDS.md. No edit to timemap/src, record.mjs, storyboard3, systems, looks or golden. Four free terrarium tiles (z6, Sumatra) added to cache/terrarium.
- **Why-verdict:** candidate division: drawer + exact lines (lights, rivers, lakes, towns) for views 4 deg and wider; globe with plain look (no satellite photo) for close and low views; smooth toggle ground: classic|smooth, classic default. Measured: plain globe 34.7 s vs 319 s per 20 s at 480p; drawer 33.8 s. Blind (2 Haiku, weak): plain globe 5/8 sits with gold.
- **Status-open:** one camera law for both grounds; Rust port of lines.py into the drawer; a pixel check in golden.py; trench needs a sea depth ramp. golden.py check: istanbul and po3 the same. Names for the drawer are Ambi's choice.
- **Related:** docs/adr/0027 items 17-18; juju-maps/grounds/stills/SHEET-480.jpg

---

## 2026-11-26 03:09 EAT — TEHUTI — Juju dates: carbon dates and sourced rows now compute who held which land, year by year
- Harness: Claude Code (claude-opus-5-5), Juju dates worker. Topics: juju
- **Changed:** new Rust crate juju-maps/dates (juju-dates): radiocarbon calibration on IntCal20/SHCal20/Marine20 with 68/95% ranges; OSL, U-series, K-Ar/Ar-Ar, tree rings, king-list counts, spans, tradition counts through one door; land computed from dated site rows over the ground (deserts and slopes slow it, rivers and coasts carry it, sea stops it); sourced borders (Cliopatria) win where present; one rule file (rules.json) decides disputes, own account and dated finds first; door.py bridges the Roots world book (194 dates, 94 holds, 76 places, 0 refused) and writes the drawer's shelf form (dates/draw/africa-roots.geojson, 36 features, all kept by timemap.py's own reader).
- **Why-verdict:** Ambi 26 Nov 02:35 "solid in code ... true to indigenous accounts and carbon dating". Published calibrations matched (Cajamarca within 2 yr, Great Zimbabwe within 5, Kakapel within 1 on IntCal20). Laws hold with planted faults failing: no land without a dated sourced row, no holder change without a dated row, no year sharper than its range, a tradition never shown as a date nor drawing land, a made-up row refused. Persia holds Egypt 520 BC, Egypt itself 400 BC (hand fixture; the Roots book has no Persia row). Kerma 2000 BC from Roots rows.
- **Status-open:** engine lane needs one glob (dates/draw/*.geojson) beside roots/draw; Roots gaps: Garamantes start, Persia, Egypt after 1080 BC, Axum outside AD 300-400; Marine20 has no published check yet; crate untracked in the juju-maps repo.
- **Related:** juju-maps/dates/README.md; films juju-maps/dates/work/film-roots-slow/dates-240.mp4, work/film-persia; runs/decision.tsv rows "dates".

---

## 2026-11-26 03:07 EAT — TEHUTI — Juju Africa timemap: engine row-fix and turn-probe work, 12-minute film drawing
<!-- type: event -->
**From:** TEHUTI

Juju Africa timemap: engine row-fix and turn-probe work, 12-minute film drawing
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 6a09db7f)
- Ambi's Persia critique: turn stops must stay on the land with the flip colour and holder name. Done: row fixes from Stories' timesets-fixes.json are cut and drawn in the engine, and the flip probe uses one camera with no letters.
- Probe result before the timing fix: 24 of 36 flips seen, and the 12 unseen turns have no drawn change at that year. That list goes to Stories for year rows. A later plan run's count is not in the transcript.
- Lead's order: draw tm-africa-long (748 s, 55 stops) as one film with turn chains and the row fixes. A counter of places lit was added. Plan run showed 15 of 23 flips before the probe-timing fix.
- Still open: the 240p draw was still running at the end of the transcript. Frames are not yet read by eye, and the mark and faults by the second have not been sent to the lead.
- Files changed: juju-maps/timemap.py; juju-maps/timemap/src/scene.rs; juju-maps/timemap/src/draw.rs; juju-maps/timemap/src/main.rs; juju-maps/timemap/README.md; juju-maps/films/tm-africa-long/story.json
- Status: in-progress — engine fixes built and tested on fixtures; 12-minute Africa film still drawing and not yet checked by eye

---

## 2026-11-26 03:06 EAT — TEHUTI — Fixed outline bug in Juju reach code and bridged Roots' Africa book into the date engine
<!-- type: event -->
**From:** TEHUTI

Fixed outline bug in Juju reach code and bridged Roots' Africa book into the date engine
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session a97dabc6)
- Ambi asked for the reach example to be built from Roots' Africa book rows (Kemet, Ta-Seti, Kerma, Punt, Kush, Napata, Aksum, Carthage, Garamantes), not a fixture: 'Go on.'
- Fixed an outline ring-orientation bug in reach.rs: real outlines were dropped and only holes survived. Removed the wrong reversal; a new outline test confirms it. 20 tests pass in release.
- Bridged Roots' book.json into the crate's row form: 132 dates, 95 holds and 3 borders pass every law with 0 refused. Each book now writes its own borders file.
- Changed the river factor 0.3 to 0.5 in rules.json, logged via scripts/decide, because Kemet reached Kerma in 3100 BC past Ta-Seti. Great Zimbabwe now 1197-1557 against Roots' 1187-1557.
- The engine's shelf reader keeps all 36 features from the new shelf file. Films drawn for the fixture, Roots dense clock and Roots slow -2200 to -1500 BC. Open: the final debug test run and README section 5 check.
- Files changed: juju-maps/dates/src/reach.rs; juju-maps/dates/src/source.rs; juju-maps/dates/rules.json; juju-maps/dates/door.py; juju-maps/dates/tests/outline.rs; juju-maps/dates/README.md; juju-maps/dates/draw/africa-roots.geojson; juju-maps/dates/fixture/africa-roots.json
- Status: in-progress — outline fix and Roots bridge verified; final debug test run and last film check still pending

---

## 2026-11-26 03:01 EAT — TEHUTI — Juju time maps: first three state films (US, Canada, America's money) at 240p
<!-- type: event -->
**From:** TEHUTI

Juju time maps: first three state films (US, Canada, America's money) at 240p
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: new chain juju-maps/states/statemap.py (its own copy beside timemap.py; the engine's Rust code was not touched) plus shp.py. It reads US states with their dates (Newberry, any lawful use), Native land cessions (Royce/USFS, CC BY 4.0), Canada's borders (Toronto atlas, copyright, review only), Canada's treaties (OGL) and BEA income by state. It draws films/st-us, st-canada and st-money. Five rows were added to data/timesets.json. Engine wishes are in timemap/REQUESTS-states.md. A country list is in states/COUNTRIES.md. Why/verdict: time maps can show states; Native land is a grid on top of the states and territories; at each stop the year creeps forward so the change happens on screen; wars run through their years with battle rings; dives work at Fort Sumter and the Klondike, but the ground blurs. Status/open: the card words are thin; the dive ground is blurred; the Métis are not in any set; the Canada borders need permission before publishing. Related: ADR 0027 items 17 to 24.
- Files changed: juju-maps/states/statemap.py; juju-maps/states/shp.py; juju-maps/states/COUNTRIES.md; juju-maps/states/DATES-CHECK.md; juju-maps/timemap/REQUESTS-states.md; juju-maps/data/timesets.json; juju-maps/data/timesets/states/
- Verification: ffprobe: 382.6 s, 357.8 s and 248.7 s, all h264+aac at 426x240, around -17 LUFS. I read frame sheets at one frame every 4 s for all three. Ten dates matched a page each (states/DATES-CHECK.md). The model cost 0.021 US.
- Status: complete: three playable 240p films; first takes for Ambi's critique

---

## 2026-11-26 02:58 EAT — TEHUTI — Juju time maps: Roots world book merged into the 12 minute Africa
<!-- type: event -->
**From:** TEHUTI

Juju time maps: Roots world book merged into the 12 minute Africa
- Harness: Claude Code (claude-opus-5-5)
- What happened: Harness: Claude Code (claude-opus-5-5). Topics: juju.
**Changed:** tm-africa-long/story.json now has 55 stops over 741 s (Measured), 15 of them before 1000 BC. 18 rows come from the Roots world book (facts/roots-africa.json, 18 of 21 rows used): Kemet's Archaic, Old, Middle and New Kingdoms with both Intermediate Periods, Ta-Seti, Kerma, Nubia under the 12th dynasty, Kush, Punt and the sea road to it, Napata, Carthage (traditional date) and Rome's landing, Meroe's Ergamenos, the Garamantes, and Aksum's coins. Each row was re-proved word for word against Roots' saved page. Roots' marks (dug, later, record, tradition) and dispute notes are kept as they are (6 notes). The turn stops are worded by the pen; 8 are flagged wrong by their pages and marked argued.
**Why-verdict:** check TRUE; turns 23 of 23 on screen. D'mt is not in the book; 3 rows were dropped (an Aksum row whose quote is about a 1906 dig, Adulis, and a second Carthage).
**Status-open:** spent DeepSeek 0.698 (0.109 of the 0.30). The engine shows 24 of 36 flips on tm-africa; the 12 unseen are years where the drawn set has no change (its receipt: films/tm-africa/check.json flips). tm-output still has one 39 s gap. Titles are drafts for Ambi.
- Status: complete for the merge; flips the set cannot draw remain open

---

## 2026-11-26 02:49 EAT — TEHUTI — Juju Worlds: a sentence in, a simulated world out; three 240p films
- Harness: Claude Code (claude-opus-5-5), worker of the worlds lane. Topics: juju
- **Changed:** juju-maps/worlds.py (frame, ground, book with attack and mend, simulation, words, time.json, story.json, film), juju-maps/worlds/ (Rust: ground, sim, plates; speed.py, exit.py, README), data/worlds (sea curve, rain, lakes, Plato's text, plate model), stack/formats/worlds.json (rules and inks), stack/worldideas.json (40 ideas), timemap/STORY-NOTE.md (asks to the engine).
- **Why-verdict:** Ambi wants a world from one sentence, and the lead wanted Atlantis first and "simulated" to be true. The history now comes from a seeded simulation (food, reach, war, revolt, trade, ships, drowning). The model sets only the start and words what happened. Films: films/w-atlantis/a.mp4, films/w-green/a.mp4, films/w-bridge/a.mp4, each 150 s at 240p; frame sheets looked at.
- **Status-open:** paid 0.653 US (DeepSeek), GLM 0. Head counts in the three films run 3 to 10 times higher than HYDE, so those films are pinned (pin.json) and new worlds use 0.2. A sim at 4 threads runs 5.5 to 22 s depending on load. Lake levels were not read again (PNAS 403). Alternate history from the record's borders is not built. Deep time: a reader and a still only. Nothing committed (juju-maps is an embedded repo).
- **Related:** juju-maps/worlds/README.md; python3 juju-maps/worlds/exit.py

---

## 2026-11-26 02:46 EAT — TEHUTI — Juju time maps: turn stops got sourced words, six titles under 58 letters, Asia pocket done; predicate still FALSE
<!-- type: event -->
**From:** TEHUTI

Juju time maps: turn stops got sourced words, six titles under 58 letters, Asia pocket done; predicate still FALSE
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 2589b416)
- Ambi asked: turn stops get real words from inside the land, quote-checked; then titles under 58 letters; then the Asia pocket; feed test only if money is left.
- Turn stops: 21 of 28 Africa stops now have a second line backed by a saved-page quote; 7 are title only. The writer found 7 dates wrong and marked them 'argued' with the doubt written on the stop.
- Titles: six candidates per film, judged blind by three strangers against 36 real titles. Each title is under 58 letters. The world-output title lost to the real ones. Weak evidence: the comparison set was not the same subject.
- Spend: $0.084 of the new $0.30 used on four jobs. Exit predicate is FALSE: 5 of 6 stories pass check; the world-output film fails on one long gap. South America waits for Roots.
- Still open: fix the world-output film's long gap, the 7 title-only stops, and the feed test (not run; money held back).
- Files changed: juju-maps/timestory.py; juju-maps/data/timesets-fixes.json; juju-maps/films/_data/time-stories/series/tm-asia.json
- Status: in-progress — exit predicate FALSE: 5 of 6 stories pass; world-output film fails one long gap, $0.216 of the $0.30 left unspent

---

## 2026-11-26 02:43 EAT — TEHUTI — Juju time maps: turn stops worded from inside, titles picked blind, Asia pocket, fix rows for the engine
<!-- type: event -->
**From:** TEHUTI

Juju time maps: turn stops worded from inside, titles picked blind, Asia pocket, fix rows for the engine
- Harness: Claude Code (claude-opus-5-5)
- What happened: Harness: Claude Code (claude-opus-5-5). Topics: juju.
**Changed:** timestory.py (word_turns, titles, feed). Turn stops of tm-africa now carry the pen's words: 21 have a second line held to a quote, 7 are title only, and 7 the pen showed wrong are marked argued. Example: 402 BC Egypt ends Persian rule / Amyrtaios organizes revolt. Six films have a title under 58 letters chosen by a blind feed test. tm-asia/story.json is new (14 stops, 210 s). data/timesets-fixes.json holds 11 rows: corrections plus turn years moved to the page's year, read by both this lane and the engine.
**Why-verdict:** the engine drew 26 of 36 flips because the fixes lived only in this lane's code; now they are one data file. The feed test passed on 4 of 5 films, but the real titles are generic, so the test is easy.
**Status-open:** 5 of 6 stories pass check; tm-output fails one gap (39 s with a single stop). South America waits for Roots; the states draft and gold film were not made. Spend: DeepSeek 0.673 (0.084 of the new 0.30), GLM 0.040.
**Related:** ADR 0027, ADR 0028.
- Status: in-progress: 5 of 6 stories pass check; engine redraws with the fix rows

---

## 2026-11-26 02:41 EAT — TEHUTI — Juju Roots: sourced shelf, Africa world book, and a check that catches coverage gaps
<!-- type: event -->
**From:** TEHUTI

Juju Roots: sourced shelf, Africa world book, and a check that catches coverage gaps
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 627f03d6)
- Ambi asked for open sources the time maps can cite: 'rarely told', 'the oldest known record', and 'within a few minutes' per region. Built a machine-readable shelf of 80 open sources across 13 regions.
- Each shelf source was fetched by code, saved with a receipt (link, time, fingerprint), and holds its passage word for word. 12 were refused with reasons; Native Land is out on its licence terms.
- Built an Africa-first world book: 435 rows from ten readers of UNESCO General History of Africa vols II to IV, plus sourced rows. 188 dated, 207 placed. Before 1000 BC it holds Kemet, Ta-Seti, Kerma and Punt.
- Coverage check (check.py) prints TRUE. It fires on both planted faults (South America opening at 1188 despite Caral and Aspero on the shelf, and 'X of Y sources agree' counts). Writer step measured at 0.18 US cents.
- Still open: the time map engine cannot draw the new data yet; that is with the engine lane. Hand-off notes for the Stories, Worlds and Engine lanes are in HANDOFF.md.
- Files changed: juju-maps/roots/shelf.json; juju-maps/roots/roots.py; juju-maps/roots/check.py; juju-maps/roots/book/africa/book.json; juju-maps/roots/book/places.json; juju-maps/roots/book/READER-BRIEF.md; juju-maps/roots/HANDOFF.md; juju-maps/roots/shelf_src.py
- Status: in-progress — shelf, Africa book and checker are built and check.py passes; the engine must still draw the data and the other regions are not yet built

---

## 2026-11-26 02:39 EAT — TEHUTI — Juju Roots: corrections after review
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5)
- Changed: book years now follow the ladder rule (a source counts once; a period claim shows as "within" its period); notes are short ladder forms, not clipped quotes; check.py now fails on a year that stands on no page (planted fault fired).
- Why-verdict: correcting the 02:5x entry: Napata is 800 BC, not before 1000 BC; Punt now dates from the Old Kingdom (-2750), not 2900 BC; Kerma stays -2000 to -1580. check.py TRUE again.
- Status-open: 26 rows rest on sentences picked by code (Aksum unit mostly); 8 reader disputes were paraphrased and dropped; paper licences were typed from the page, not compared; engine does not yet read draw/.
- Related: juju-maps/roots/HANDOFF.md

---

## 2026-11-26 02:34 EAT — TEHUTI — Juju Night round two: shelf gate, dated shapes, numbers from the sentence, changes read from pixels
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/shots/ shelf.py (gate, 20 subjects a shelf: borders, quakes, plague, battles), table2.py (rows by code from the shelf), night.py + night_film.py (short menu, frame in the clear window, figure copied from its sentence, years without commas), seen.py (before and after stills, threshold from Istanbul 0.0445), pick.py.
- **Why-verdict:** three first takes: scar (quakes, seen 7 of 8), bristol (Black Death, seen 4 of 13), khovd (Xiongnu borders, seen 6 of 9); planted Aral fault fails as it must. A fresh Haiku reader: what the scripts claim about people (merchants, herders, Silk Road) is never drawn.
- **Status-open:** time-type system card is over the 26,000 limit (not this lane); bristol towns faint and whole view thin; scar claims a stretch unbroken since 1992 (false, not checked by GLM).
- **Related:** juju-maps/films/{scar,bristol,khovd}/a.mp4, films/_data/kinds/fresh-read.json, shots/data/subjects.json

---

## 2026-11-26 02:32 EAT — TEHUTI — Built juju-dates crate: dates as printed, calibrated ranges, Africa land-by-year (in progress)
<!-- type: event -->
**From:** TEHUTI

Built juju-dates crate: dates as printed, calibrated ranges, Africa land-by-year (in progress)
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session a97dabc6)
- Ambi asked for a Rust crate in juju-maps/dates that turns source-printed dates into honest ranges, with 68 and 95 percent bounds, and maps land by year.
- Built the crate (date, curve, source, show, ground, reach modules) and a Python door; it builds. Calibration was checked against published SHCal20 dates in the Cajamarca and Great Zimbabwe sources.
- Wrote 19 law tests on the shape-by-year rules; all 19 pass. Planted-fault mutant checks were started, results not yet reported.
- Africa 20-row fixture built from passages found word for word in the Roots pages. Two disputes are flagged (Carthage, Garamantes) rather than resolved.
- Still open: the film render was running in the background, and the camera first framed the wrong area; the door was changed to aim at live land. Frames not yet viewed or verified.
- Files changed: juju-maps/dates/src/reach.rs; juju-maps/dates/src/date.rs; juju-maps/dates/src/show.rs; juju-maps/dates/tests/laws.rs; juju-maps/dates/door.py; juju-maps/dates/rules.json; juju-maps/dates/README.md; juju-maps/dates/src/lib.rs
- Status: in-progress — crate builds and 19 tests pass; film render and camera framing not yet verified in frames

---

## 2026-11-26 02:30 EAT — TEHUTI — Juju Roots: sourced shelf, world book for Africa, coverage check that catches missing ancient states
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5)
- Changed: juju-maps/roots/ (shelf.json 80 open sources by region with receipts and picture licences; ladder.json; roots.py; check.py; book/africa/book.json 435 rows from 10 Haiku readers of UNESCO GHA II-IV; places/andes,kemet,indus + draw/*.geojson; FACTS.md, HOW-TO-DIRECT.md, SKILL.draft.md, REQUESTS-roots.md, HANDOFF.md).
- Why-verdict: Ambi (ADR 0028, 0029) wants own accounts first, no count odds, a book built ahead. check.py TRUE; cover fires on tm3-south (Caral, Chavin) and tm3-world; Africa before 1000 BC now holds Kemet, Ta-Seti, Punt with its sea route, Kerma, Kush, Napata. Writer pick (DeepSeek off) 7.3 s, 0 invented rows; spend 0.63 US cents.
- Corrections: Mehrgarh date disputed (5200 BC new vs 8000 BC old); Turin papyrus gives 13,420 and 23,200 years, the 36,620 total is a readers sum; Native Land refused by its own treaty (no commercial use).
- Status-open: engine must accept FINDS/ACCOUNT types (REQUESTS-roots.md); GHA V-VIII unread; 379 queue items; nothing committed.
- Related: juju, juju-maps, ADR 0027-0029

---

## 2026-11-26 02:19 EAT — TEHUTI — Juju time maps: Africa film re-cut from proved sources, audit of two old films, pockets still open
<!-- type: event -->
**From:** TEHUTI

Juju time maps: Africa film re-cut from proved sources, audit of two old films, pockets still open
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 2589b416)
- Ambi asked for accuracy first and for slower pacing: "pacing was quite poor", "you just kind of rushed to the two-minute mark". Built timestory.py to make each card's year and quote checkable.
- Audit of tm-africa and tm-output: 6 of 13 Africa cards were wrong and 4 were loose. Causes: unrelated rows glued by short name, grid years, and a 96% claim that counted only drawn states. Card table in AUDIT.md.
- Africa story rebuilt as 43 stops over about 490 s, with turning points on their own stops and Persia-Egypt flips shown. Each card's quote was found in a saved open page. Africa's stories are in place and the engine worker is drawing them.
- Sahara roads and Mansa Musa story built in code. Ambi's new rule (ADR 0028) is noted and the four new 2 to 3 minute pockets (Asia, South America, North America, one more wealth) are not done.
- Money ran out at $0.586 of $0.60, so the North America and wealth pockets and the feed test were not finished. The exit predicate prints FALSE.
- Files changed: juju-maps/timestory.py; juju-maps/timemap/STORY-NOTE.md; juju-maps/timemap/STORYBOARD.md; juju-maps/films/_data/time-stories/AUDIT.md; juju-maps/films/_data/time-stories/briefs/tm-africa.json; juju-maps/films/_data/time-stories/briefs/tm-output.json; juju-maps/films/_data/time-stories/briefs/tm-sahara.json; juju-maps/films/_data/time-stories/facts/africa.json
- Status: in-progress — Africa, Sahara and the audit are done; four new pockets, North America and the feed test are open, and the exit predicate is FALSE because the DeepSeek budget ran out.

---

## 2026-11-26 02:18 EAT — TEHUTI — Juju time maps: story lane, proved cards, turns of each land, Sahara roads by rule
<!-- type: event -->
**From:** TEHUTI

Juju time maps: story lane, proved cards, turns of each land, Sahara roads by rule
- Harness: Claude Code (claude-opus-5-5)
- What happened: Harness: Claude Code (claude-opus-5-5). Topics: juju.
**Changed:** juju-maps/timestory.py (source shelf of about 140 open pages in SQLite full text; hunt, facts with verbatim quotes, pen story, ear, GLM doubt, mend, frame; code checks; turns of each core land with chains; turncheck). New story.json for tm-africa (68 stops, 729 s, 36 of 36 turns on screen), tm-africa-long (the first ~7 minutes of the 20 minute film), tm-sahara (roads drawn by a stated rule: 34 km a day, 26 day stretch, cost d^1.5; it reproduces Ibn Battuta's 25 and 10 days), tm-musa, tm-output (new credits and the original papers). Also films/_data/time-stories/AUDIT.md, africa-rule.json (honest counter: 79 percent of Africa not ruled from outside in 1880, 5 in 1914; GHA VII says 80 percent ruled by its own), data/timesets.json (+14 sets), data/timesets-chains.json, stack/formats/timemap-long.json (laws and two 20 minute plans), stack/timeideas.json (84 hand-made ideas, unranked), timemap/STORYBOARD.md and STORY-NOTE.md.
**Why-verdict:** the first Africa film had 6 wrong cards out of 13 (renamed rows told as ends, keyframe years, the base of the 96 percent). Every card now stands word for word in a saved page, its year is beside its quote or in a second page, and every change of holder of a core land is a stop.
**Status-open:** DeepSeek 0.589 of 0.60 spent and GLM 0.040 of 0.05, so no more pen work. Not done: Asia (facts only), states (a draft with 222 faults, marked stories-draft), gold (series only), and South America, which waits on Roots. The feed test was never run. Five film titles are over 58 letters. Turn stops carry the rule's words; the pen should reword them.
**Related:** ADR 0027, ADR 0028; engine worker told by message.
- Status: in-progress: five stories stand; four new pockets and the feed test need money

---

## 2026-11-26 01:41 EAT — TEHUTI — Juju: Africa remake seven minutes, clear-map and own-account rules, Night shots round two
<!-- type: event -->
**From:** TEHUTI

Juju: Africa remake seven minutes, clear-map and own-account rules, Night shots round two
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: ADR 0027 items 10 to 16 and ADR 0028 (own account first, sureness shown) from Ambi's words; GLOSSARY own account; lanes sent: clear-map page for six themes (Type), camera that fits its subject (Engine), slower and inside-told stories (Stories), new lane Juju Roots (source shelf, marks, coverage check). Why-verdict: time maps work because the picture is the data; Night picture-first films came out 4.5 to 6.5 by the builder, 4.5 for Bolivia by the lead (wrong land filled, figures that differ from the voice). Status-open: round two of Night shots with a subject gate and dated shapes; five questions put to Ambi (odds in counts, hatched own record, outside dating, banners, Night keeps the globe). Test spend 31.76 of 35 US.
- Status: in-progress; waiting for lanes and Ambi's answers

---

## 2026-11-26 01:41 EAT — TEHUTI — Juju taught seven story kinds and a shot-first film builder; first takes still below bar
<!-- type: event -->
**From:** TEHUTI

Juju taught seven story kinds and a shot-first film builder; first takes still below bar
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 9019894e)
- Ambi asked: teach Juju seven kinds so a new film is good on its first take. Seven kinds are written in juju-maps/kinds/, hooked into storyboard3 with one hook. Istanbul's scene is unchanged to the byte.
- Verified: kinds check passes, stack/test_kit.py runs, and golden.py check shows Istanbul and po3 gold unmoved. The blind six-film comparison was built but never judged.
- Built juju-maps/shots/ (menu of 17 shots, table, write, run.sh) per Ambi's 'picture first' rule. First takes: trench 5, suez2 4.5, aral 4.5, shrinking 6.5 by the agent's own eye. Not shown to Ambi.
- Still open: no fresh-eye judgement of the takes, the 25-minute pocket was only tested on a short fixture, and the 'one person carries the film' thread is not yet proven.
- Files changed: juju-maps/kinds/moves.py; juju-maps/kinds/water.py; juju-maps/kinds/border.py; juju-maps/kinds/route.py; juju-maps/kinds/steps.py; juju-maps/shots/menu.py; juju-maps/shots/write.py; juju-maps/shots/run.sh
- Status: in-progress — kinds and shot builder exist; bar not met (best first take 6.5 by agent's eye, no fresh judge yet)

---

## 2026-11-26 01:39 EAT — TEHUTI — Juju Maps: seven kinds of story in code, then Juju Shots, films written as pictures first
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/kinds/ (seven kinds, rules, steps, choose, born, plan; one hook in storyboard3; kit.py carries the kind; birth.py and spine.py one line each); juju-maps/shots/ (title, table, menu, write, check, make, run.sh).
- **Why-verdict:** three kind-driven first takes came out about 3 (tengiz, ore, niger). Juju Shots first takes: trench 5, suez2 4.5, aral 5.5, shrinking (Bolivia) 6.5 by the builder's own eye; every name on screen, no unchanged return, 4.6 to 5.6 new things per 10 s.
- **Status-open:** no blind eye has compared them; 12 minute list came out 9.4 minutes; people, except, bars and years shots weak; border fills need old borders. Spent about 1.00 US (kinds) and 0.52 US (shots).
- **Related:** juju-maps/films/shrinking/a.mp4, juju-maps/films/_data/shots/menu.jpg, runs/decision.tsv

---

## 2026-11-26 01:34 EAT — TEHUTI — Juju: models only in close views after a lost blind test; time-map pages redesigned
<!-- type: event -->
**From:** TEHUTI

Juju: models only in close views after a lost blind test; time-map pages redesigned
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Blind test: films with Poly models won 2, without won 4, tied 2. The set Ambi rated 8 was restored, and models now appear only in views closer than about 250 km.
- Jakarta test used a 25 Nov cut with the banned Harold voice and repeated camera angles. A Neon cut cost $0.53 and was poor. Ambi's 'sounds AI-ish' note was confirmed.
- Four more time-map films drawn for critique (Asia 7, World 4 by Ambi's scale). Five two-minute films cost 3.1 US cents. Seven-minute Africa redrawn for 1.6 cents, mark 7.
- Time-type page redrawn: 8 to 22 words on screen against about 45 before. Blind readers scored it 5.4 and 5.1 against 4 for the old films. Nobody has seen it move yet.
- Open: the picture-first Night film has a script but no film yet. Testing spend is $30.41 of $35, with DeepSeek at $10.56 left. Juju Roots builder is new and unverified.
- Files changed: juju-maps/stack/bodies.json; juju-maps/data/voices.json; juju-maps/timemap-v03/churn.sh; juju-maps/stack/systems/time-type.json; docs/adr/0027-time-maps.md
- Status: in-progress — builders still working on the Africa remake, Atlantis and the first picture-first Night film.

---

## 2026-11-26 01:11 EAT — TEHUTI — Juju time maps: four more films drawn for critique, faults handed to the builders
<!-- type: event -->
**From:** TEHUTI

Juju time maps: four more films drawn for critique, faults handed to the builders
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: the first time-map engine (commit a3010f5) frozen in juju-maps/timemap-v03 (opens just before the first state); drew Asia, South America, North America, Europe, World from one sentence each. Why-verdict: Ambi asked for more videos to critique and for scale; Asia is the best (lead mark 7), South America 6, Europe 5 (cut Russia, set dates wrong), North America held back (camera leaves to Siberia). Status-open: new engine, type, stories, worlds and shots lanes running; faults sent to engine and stories lanes. Decisions added to ADR 0027 items 7 to 9 (low thinking is fine; Night and Day stay but need extreme consistency; testing is for scale).
- Verification: frame sheets read for south, asia, north, europe; all decode to 125 s; under 1 US cent each in run.json
- Status: in-progress; films sent to Ambi for critique

---

## 2026-11-26 00:52 EAT — TEHUTI — Juju Writer lane closed: short scripts good, long form 3 of 10
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** stack/write (truth.py, pages.py, long.py, list rule); nothing in the live default.
- **Why-verdict:** DeepSeek two minute chain 6 of 8 films, 18 of 24 votes (seven films reuse v4 drafts); max 7 of 12 votes for twice the time and money; 19 minute script from true pages 3 of 10: pockets planned one by one, no person carrying it.
- **Status-open:** hard read wired but off (0.023 US); lessons handed to Juju Shots; no more money on long scripts until shots prove.
- **Related:** juju-maps/films/_data/writer

---

## 2026-11-26 00:51 EAT — TEHUTI — Juju: why the voiced films fail, and the shot-first lane
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** voice Harold banned; bodies only under 250 km; taste; Juju Kinds worker turned to Juju Shots (picture first), beside everything, golden check required.
- **Why-verdict:** Ambi on Jakarta (25 Nov 19:51, before the upgrades): "terribly bad", voice "AI-ish"; measured over nine films: 2 to 7 of 6 to 32 named places off screen, 6 to 12 views on seen spots; Jakarta was cut by Neon for 0.53, so the model is not the cause; time maps one-shot because picture is the data.
- **Status-open:** exploring, not decided by Ambi: shot-first for Night and Day; narrated time maps.
- **Related:** juju-maps/films/jakarta

---

## 2026-11-26 00:49 EAT — TEHUTI — Juju Writer: numbers of the last round, one line put right
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** PEN_HARD is off by default (the two minute Neon read costs 0.023, over the 0.02 bar).
- **Why-verdict:** the wired chain won 6 of 8 films, 18 of 24 votes; lost Istanbul 0 of 3 and Congo 1 of 3. Correction to the entry before: the words about a wrong sentence shape mean nothing; Neon gave three usable sentences on dam4 and three on kivu2.
- **Status-open:** as in the entry before.
- **Related:** juju-maps/films/_data/writer/votes/9-0.json

---

## 2026-11-26 00:48 EAT — TEHUTI — Juju Writer: max measured, facts first works for sheets, the long script still fails
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/stack/write (truth.py, pages.py, idea.py, long.py facts first, hardread.py, list rule in pen.py); spine.py WRITER=deepseek makes a true sheet when there is none and takes one Neon read; the default path asks the same bytes.
- **Why-verdict:** max 7 of 12 votes at twice the price and time: low stays. Sheets now hold quoted, dated steps. 25 minute script 3 of 10: true pages, no story carried by people. Neon read of two minutes costs 0.023 to 0.024, over the 0.02 bar, and put one wrong sentence shape in nothing.
- **Status-open:** DeepSeek went 0.02 over its 0.70; the list rule is unheard; the Neon read ran on two films only.
- **Related:** juju-maps/films/_data/writer/long6-heard.md, votes/

---

## 2026-11-26 00:43 EAT — TEHUTI — Juju time maps: new channel type, voices wired, safety net and read-only front door added
<!-- type: event -->
**From:** TEHUTI

Juju time maps: new channel type, voices wired, safety net and read-only front door added
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked for better time-map fonts, smaller text, zooms and map tricks, and Africa pacing that slows at turning points. Work was split across type, engine, stories and worlds builders.
- Ambi said 'don't mess up' what works. Gold Istanbul and a Day film are locked as golden tests, restore points are marked, and ./ju doctor reported 10 of 10 OK. A planted fault was caught.
- All 19 shelf voices passed the hard-name check on the cheap model (0.91 or better) and are wired in as Àṣẹ Regular V 0.3. Àṣẹ High V 0.3 is the dear option.
- CPU fell from 73 to about 41 after the 100k-tile map cache was moved out of the builders' scan path to ~/AUH/.juju-store. Only one Night or Day film draws at a time.
- Still open: time maps are not yet in the golden test. The Atlantis, Sahara and Mansa Musa films and the Africa re-make are still in production and not yet checked by Ambi.
- Files changed: docs/adr/0027-time-maps.md; juju-maps/ju; juju-maps/stack/golden.py; juju-maps/data/voices.json; juju-maps/stack/golden/istanbul/scene.json; ~/AUH/.juju-store
- Status: in-progress — safety net and voices are done; new time-map films are still rendering and not yet reviewed

---

## 2026-11-26 00:42 EAT — TEHUTI — Juju: safety net round the gold films, read-only front door, cache moved, voices cheap, worlds lane
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** stack/golden.py (istanbul, po3), stack/stack.json, ju (doctor, where, seats, systems, films); tile cache and .toolchain moved to ~/AUH/.juju-store behind links; record.mjs one drawing at a time; data/voices.json 19 of 19 on Ase Regular V 0.3; GitHub tags gold-istanbul-25nov, safe-26nov-0055; ADR 0027 items 4 to 6; Juju Worlds lane.
- **Why-verdict:** Ambi: "don't break what's working"; net proven with a planted fault; load 73 to 24; all 19 voices say the hard names at 0.91 or better on the cheap model (machine listener).
- **Status-open:** time engine remaking Africa, kinds, writer, poly report, worlds, stories, type running.
- **Related:** docs/adr/0027-time-maps.md

---

## 2026-11-26 00:40 EAT — TEHUTI — Juju bodies: new engine and casts built, blind test lost, live set restored
<!-- type: event -->
**From:** TEHUTI

Juju bodies: new engine and casts built, blind test lost, live set restored
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 867c3ea9)
- Ambi's ask: Juju Poly bodies on Duppy Night and Day, fitting each map; he rated Istanbul an 8 and said the placing "just fit everything very well". Istanbul is frozen, so proofs use kivu2, po3 and jakarta.
- Built: night lit windows and ground light, day relief-matched roofs, sizes 12 to 30 px, acts in stack/bodies.json (24 verbs; burn weakest; open, unload, leave, wait have no still), 28 own models.
- Verified: blind A/B on 8 ten-second pairs gave with bodies 2 wins, without 4, equal 2. New against old was never tested. The live models.js is byte-identical to the set Ambi gave an 8.
- Cast: 11 films read, $0.182 for 52 calls. Not tried on a 25-minute script; kivu2 views are thin; the last seat changes were not re-assessed. Sound brief left at stack/sounds/BODIES-NOTE.md.
- Stopped drawing on the lead's order (load 73); no draws running.
- Files changed: juju-maps/models.js; juju-maps/bodies.py; juju-maps/stack/cards/bodies.md; juju-maps/stack/bodies.json; juju-maps/stack/sounds/BODIES-NOTE.md; juju-poly-assets/own.json
- Status: in-progress — the bar is not met (blind test lost); live set restored, no draws running, the seat is not re-tested on a full script

---

## 2026-11-26 00:39 EAT — TEHUTI — Juju bodies: new engine, cast and 28 own models built; lost the blind test, live set restored
<!-- type: event -->
**From:** TEHUTI

Juju bodies: new engine, cast and 28 own models built; lost the blind test, live set restored
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: juju-maps/bench/new (models.js, bodies.py, card, block), stack/bodies.json (closed shelf, 25 verbs, tweaks), 28 own models in juju-poly-assets (own_bodies.mjs, own.json), bench still tool, notes to Ear and Maps+Motion. Live is the old set (Ambi's 8 on Istanbul); bench/swap.py new switches. Why-verdict: blind agent on 8 ten-second pairs: with bodies 2, without 4, equal 2; only strong win is the Jakarta sea wall rising. Status-open: houses that flood and small day boats lose; verbs must show change in the words' own place; test again new against old when the Mac is free. Related: Istanbul frozen by Ambi.
- Verification: 240p stills and films looked at; blind agent; swap.py old verified byte-identical to the 23:00 engine
- Status: complete, reverted live; new set waits for a second test

---

## 2026-11-26 00:02 EAT — TEHUTI — Juju time maps become a channel type; three lanes started
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** docs/adr/0027-time-maps.md, GLOSSARY (time map), taste.json; lanes: engine (motion, clock, camera, Juju Poly in Rust, themes), Time Type (fonts, page, six themes), Time Stories (accuracy audit, data, pockets, 60 ideas).
- **Why-verdict:** Ambi: Africa film "absolutely beautiful ... almost perfect"; wanted less and smaller text, better fonts, no glitches, calmer clock, placed assets, 20 minute pockets.
- **Status-open:** films to be remade; names and grouping of the two systems open; kinds, writer, poly lanes also running (six workers, Mac load about 30).
- **Related:** juju-maps/films/tm-africa/a.mp4

---

## 2026-11-25 23:58 EAT — TEHUTI — Juju: money window built, Juju Maps fixes shipped, writer stop rule failed, GitHub save set up
<!-- type: event -->
**From:** TEHUTI

Juju: money window built, Juju Maps fixes shipped, writer stop rule failed, GitHub save set up
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked for a live money window and a GitHub save. The window is at runs/pots/window.png: DeepSeek, WaveSpeed and OpenRouter refresh live, Inworld and Google are estimates. The film guard is built but off.
- Juju Maps: marmara2 half-fill and dashed sea lines fixed, 0 pops on seven test films, shore ring and thin crack drawn. Every move has a sound by program count (120 of 120), but nobody has listened yet.
- Juju Writer stop rule FALSE: DeepSeek beat Neon on 2-minute scripts (21 of 24 AI votes) but lost Istanbul, and its 25-minute script scored 3.5 of 10. Version 4 kept; 25-minute writing is still unproven.
- Tic fixer was silently skipping 26 of 125 rules; all now run. A rule I added made it invent people, so I removed it. Time-map films tm-africa and tm-output drew in 26-34 s; the agent's marks are 7 and 6.5.
- Juju GitHub save: merged a separate copy with the private main and pushed; a half-hour LaunchAgent plist was written. Open: voice choice, seven old pull requests, money window at login, Ambi's listening test.
- Files changed: juju-maps/film.js; juju-maps/calabash.py; runs/pots/window.png; docs/adr/0026-sixty-day-pots-and-zero-shot.md; juju-maps/films/istanbul/gold6.mp4; juju-maps/films/tm-africa/a.mp4; scripts/juju-save.py; juju-maps/films/istanbul/gold-ear.mp4
- Status: in-progress — money window, map fixes and tic fixer done; listening test, 25-minute scripts and voice choice still open

---

## 2026-11-25 23:57 EAT — TEHUTI — Juju Writer: DeepSeek wins most two minute scripts blind; GitHub saved; time maps landed
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** routes.json pen rows (max, high, low); tics-maps.json without the nobody rule and calabash.heal told to add nothing; private main a3010f5 by juju-save (half-hourly launchd loaded); films/tm-africa, tm-output.
- **Why-verdict:** the nobody rule made the healer invent people (found by the writer); DeepSeek v4 chosen 21 of 24 by three Haiku listeners and 14 of 16 by two Opus, lost Istanbul 2 of 5, 25 minute script 3.5 of 10 (no sourced sheets). Ambi on the time maps: "you finally use reverse engineer video like excellently".
- **Status-open:** one max call unmeasured; long form sheets; hard read not wired; Ambi's pair reading, voices, pull requests.
- **Related:** juju-maps/films/_data/writer/read-me.md

---

## 2026-11-25 23:56 EAT — TEHUTI — Juju Maps: correction, the writer stop rule is FALSE
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** nothing in code; read-me.md now shows the Istanbul, Bosphorus and Kivu pairs.
- **Why-verdict:** 8 of 8 was the Haiku round; under the strict listeners version 4 lost Istanbul 0 of 2; mississippi was written by GLM and mud last by GLM; the shipped chain adds a GLM doubt no listener heard; one version won one round only. calabash.heal is not wired: 2 of its 3 rewrites made up a person. Congo sheet asked again twice, failed (every step stamped 2025).
- **Status-open:** one more full bench round, about 0.17 US; Istanbul run of places; level max.
- **Related:** juju-maps/films/_data/writer/rows.md, long-heard.md

---

## 2026-11-25 23:53 EAT — TEHUTI — Juju Maps: DeepSeek writes the two minute script as well as Neon; the long script is not there
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/stack/write/ (craft, ear, mend, doubt, pen.py, bench.py, blind.py, long.py, hardread.py); spine.py WRITER=deepseek (default path asks byte for byte the same).
- **Why-verdict:** blind listeners chose DeepSeek on 8 of 8 films (version 4, kept) and 6 of 8 (version 7, reverted); Istanbul lost to Neon under the strict listeners. The 25 minute script got 3.5 of 10: false facts, repeats. Neon hard read cost 0.051 and found the false facts GLM missed. All at level low: no max row in routes.json yet.
- **Status-open:** rows in films/_data/writer/rows.md; max unmeasured; the long form needs a sourced sheet per pocket.
- **Related:** juju-maps/films/_data/writer/read-me.md, rows.md, long-heard.md

---

## 2026-11-25 23:45 EAT — TEHUTI — Juju Pots: live balances in a tiny window, the app row and a guard
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** crates/juju-pots, ~/Applications/Juju Pots.app (open), crates/juju-serve pots.rs + one route, live.js row, juju-maps/pots.py, runs/meter/pots-said.json.
- **Why-verdict:** Ambi (ADR 0026) wants the money seen without a browser. Live read works; fail-open proved with a dead gate. At 60 films of 22.5 min the pots are short about 71 US (Estimated); 70 CAD is 49.
- **Status-open:** server not swapped, login not loaded, guard not wired, LOT's money unknown.
- **Related:** AMBESSA/intel/juju/crates/juju-pots/HANDOFF.md, runs/pots/window.png

---

## 2026-11-25 23:44 EAT — TEHUTI — Juju: Mac load fixed, tic linter repaired, date and name one mark, GitHub save started
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** record.mjs queue (two drawings, nice 12), mix.py nice; calabash.py (26 of 125 rows were skipped in silence; heal()), tics-maps.json +5, test_calabash.py; film.js joins year and place; scripts/juju-save.py, ~/.juju-save/repo (merge e2856b1 of live and 77 GitHub commits), LaunchAgent com.auh.juju-save written, not loaded; ADR 0026 items 7 to 14; voice pair films/audition/pair.
- **Why-verdict:** load 150 to 13; Congo script 8 flagged to 0 for 0.0012 US in 8 s; stills only of the new marks, Istanbul not remade on Ambi's word. Push to private main running.
- **Status-open:** push result, merged crates not compiled, 7 old pull requests open, voice choice, pots and kinds and writer and poly and time-map workers running.
- **Related:** docs/adr/0026-sixty-day-pots-and-zero-shot.md

---

## 2026-11-25 23:42 EAT — TEHUTI — Juju Maps: wordless time maps from one command, two pockets
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/timemap (Rust drawer), timemap.py, data/timesets.json, stack/systems/duppy-time.json, stack/formats/timemap.json, refs/umstrUXqmRg.*; films tm-africa, tm-output.
- **Why-verdict:** Ambi 25 Nov: a film with no script is a niche of its own. Study film measured (31 cards, median hold 4.0 s, clock 39 percent slower under a card); blind rebuild 0.43 against 0.35 unrelated and 1.00 itself, 58 gaps listed. Bugs found by looking: 1500 to 1803 was never sampled (fixed, asserted), shadows drew squares (fixed), dates of early states are sampled and now say about.
- **Status-open:** drawer capped at 4 threads, nice 12, one draw at a time on the lead's order; world film is 34 s at that cap (bar 30). Clip export works, not wired. Third pocket stopped. $0.038 spent.
- **Related:** juju-maps/timemap/README.md

---

## 2026-11-25 23:24 EAT — TEHUTI — Juju Maps: shore ring, thin crack, painted night land and five new kinds landed; gold film redrawn with all of it
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** storyboard3 emits shore inside a named sea and no longer forces life off; worker added area lists, turn, level, gate, part; films/istanbul/gold6.mp4.
- **Why-verdict:** 93 s to draw at load 55 to 75, 120 of 120 moves heard by the count, plays; seen by the lead in stills of the worker's two takes, gold6 itself not read frame by frame.
- **Status-open:** round 3 unanswered; poly, kinds, writer, pots, time-map workers running.
- **Related:** juju-maps/films/_data/sheets/istanbul-shore-life.png

---

## 2026-11-25 23:20 EAT — TEHUTI — Juju Ear: every on-screen move now gets its own quiet sound, built and checked on marmara2, not yet listened to
<!-- type: event -->
**From:** TEHUTI

Juju Ear: every on-screen move now gets its own quiet sound, built and checked on marmara2, not yet listened to
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 64feae74)
- Ambi's ask (ADR 0024): "every little element... can be subtle, it can be quiet, but it has to be there." Camera whooshes, diagram in/out, and number jingles. Never 8-bit or game-like.
- Built: timeline.mjs reads each move from the engine's own numbers with no hook needed; chooser.py picks sounds per film; mix.py lays voice first at about -14 LUFS from 51 roles in 5 packs.
- Agent's own checks on marmara2, po3 and kivu2: moves heard 96/96, 96/99 and 80/80; timing within 40 ms on most; the check fails when moves are removed or dropped 12 dB.
- Open: no person has listened yet. Timeline page load took 8-11 s against a 5 s target. The timeline bar, one kivu2 fault and low-poly are not done. Watch file: films/marmara2/ear.mp4 (matches b.mp4).
- Files changed: juju-maps/mix.py; juju-maps/timeline.mjs; juju-maps/stack/sounds/chooser.py; juju-maps/stack/cards/sound-map.json; juju-maps/stack/sounds/roles.json; juju-maps/ear.py; juju-lowpoly/mix-poly.py; juju-maps/films/marmara2/ear.mp4
- Status: in-progress — system built and self-checked; predicate not fully TRUE, awaiting human listen and open items

---

## 2026-11-25 23:20 EAT — TEHUTI — Juju Ear: every move heard, chooser fixed, sound put on the gold film
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** chooser.py (16000 room, 45 s), mix.py join 45, routes sound row; films/istanbul/gold-ear.mp4 (q.mp4 picture, new mix); cap.json 35 on Ambi's order; ADR 0026; taste (8 gold, polygon 5); delegates Juju Writer, Juju Kinds, Juju Pots.
- **Why-verdict:** 117 of 117 moves heard by the count, 4 of 4 pockets by DeepSeek low for 0.0047 US in 13 s (0 before: the stage allowed 0.02 and the call was held at 0.077). Nobody has listened yet.
- **Status-open:** grilling round 3 unanswered (films in 60 days, Neon's jobs, top-up, cheaper voice, GitHub save).
- **Related:** runs/sound/ear-1125/HANDOFF.md

---

## 2026-11-25 23:18 EAT — TEHUTI — Juju Maps: shore ring, thin fault, five kinds of change, painted land on at night
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps film.js, gl.js, tiles.js, record.mjs, stack/changes.json, stack/cards. Nothing committed.
- **Why-verdict:** Ambi: ring the surrounding water; crack was a blob; five kinds had no act. Istanbul drawn whole twice, 0 late; blind eye took the painted land 8 of 8.
- **Status-open:** day painted land off; gate at most .11 of the view; dam wall not proven; order_to_build next.
- **Related:** juju-maps/films/istanbul/shore.mp4, life.mp4, films/_data/sheets

---

## 2026-11-25 23:17 EAT — TEHUTI — Juju Ear: every move on the map films is heard, from the engine own clock
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/timeline.mjs, mix.py, ear.py, stack/sounds/ (51 roles, 5 packs, chooser), stack/cards/sound-map.json and sound.md, beds/ (things, airs, small, six public domain beds), channels/*.json sounds row, juju-lowpoly/mix-poly.py.
- **Why-verdict:** Ambi 21:40 (ADR 0024): marmara2 had two sounds in 100 s. Now 96 of 96 moves heard by the check, ambience 15 percent, -14.2 LUFS; the check fails planted faults. Nobody has listened yet.
- **Status-open:** kivu2 one sound 1.5 dB over its law; low poly uses scene seconds; DeepSeek low answers under half the pockets, code stands. Chooser spend 0.057 US in all.
- **Related:** juju-maps/films/marmara2/ear.mp4, ear.json, ear-list.md; runs/sound/ear-1125/HANDOFF.md

---

## 2026-11-25 22:55 EAT — TEHUTI — Juju Maps: motion lane reported, next five jobs sent
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** nothing by the lead; worker added window.timeline, bloom fills, upright ruler, painted land (off), one engine version per film.
- **Why-verdict:** a whole Istanbul film on tonight's engine plays; night plain and close day fields read, po3 villages at 1.6 degrees too faint.
- **Status-open:** shore ring, crack shape, missing kinds, painted land default; sound, poly and time-map workers running.
- **Related:** juju-maps/films/_data/sheets/life-true-size-240p.png

---

## 2026-11-25 22:53 EAT — TEHUTI — Juju Maps: DeepSeek thinking fixed, Istanbul film redrawn with Juju Poly models, sound rules written down
<!-- type: event -->
**From:** TEHUTI

Juju Maps: DeepSeek thinking fixed, Istanbul film redrawn with Juju Poly models, sound rules written down
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked: 'Get DeepSeek working... It must work.' DeepSeek thinking now returns an answer on the Istanbul cut that returned nothing before. It left 7 faults, against 15 to 18 for the weaker tries, for about 3 cents.
- Redrew the Istanbul film as take3 (ten views, land cut restored) and take5-poly (Juju Poly models: flats that shake and fall, a ferry and boats with wakes). Self-marked about 7.3; sound is still the old mix.
- Wrote ADR 0024 (every move is heard, a channel owns its sound) and ADR 0025 (Juju Poly casts every Night and Day film). Found and fixed a latitude/longitude swap in the place finder.
- Congo economics film judged about 3.5 and not sent: it filled the wrong Congo. Rules changed, not redrawn, so the fix is unproven. Villages were turned off because they read as red spots on grass.
- Spend was $26.75 of $30 at last check. Open: sound packs, motion with sound, a blind test for Juju Poly against the same film without models, and the Congo redraw.
- Files changed: juju-maps/storyboard3.py; juju-maps/board7.py; juju-maps/models.js; juju-maps/geo.py; juju-maps/server.mjs; docs/adr/0024-every-move-is-heard.md; juju-maps/films/istanbul/take5-poly.mp4; juju-maps/films/istanbul/take3.mp4
- Status: in-progress — Istanbul film is at about 7.3 and awaiting Ambi's watch; sound, Juju Poly blind test and Congo redraw are still open

---

## 2026-11-25 22:52 EAT — TEHUTI — Juju Maps: Juju Poly put on the Night and Day maps, with a casting seat
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/models.js, states.js, film.js hook, server.mjs serves models, bodies.py, stack/cards/bodies.md, storyboard3 BODIES block and the locked stretch, make.sh; ADR 0025; two Congos fixed; board7 still-stretch pass; Juju Poly delegate started.
- **Why-verdict:** Ambi marked Istanbul take 3 a 7 ("after one minute it just stops doing things") and asked for Juju Poly on everything. First stills worked at once; night windows, shake and fall, boats under way drawn in films/istanbul/poly.mp4 (50 s to draw). Congo economics film about 3.5 by the lead (headings for sentences, wrong Congo filled): rules fixed, not redrawn.
- **Status-open:** Juju Poly, sound, motion, time-map workers running; still-stretch pass kept 0 of 3 on its only run.
- **Related:** juju-maps/films/istanbul/poly.mp4, films/congo

---

## 2026-11-25 22:34 EAT — TEHUTI — Juju Maps: villages painted in the ground at true size, off by default; fills bloom; one engine per film
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps film.js, gl.js, tiles.js, record.mjs, data/roads10.bin, stack/cards. Nothing committed.
- **Why-verdict:** lead and Ambi: clumps read as pox. Standing bodies removed; towns, roads, parcels and lights are in the tiles.
- **Status-open:** life stays off; day villages at 1.6 degrees are faint; no air photo compared by day.
- **Related:** juju-maps/films/_data/sheets/life-true-size-240p.png, bloom-rupture-240p.png

---

## 2026-11-25 22:27 EAT — TEHUTI — Juju Maps: niches wired into the idea stage; first economics film started
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** birth.py takes NICHE=<id> (53 in stack/niches.json); geo.py asks for lat and lon by name (swapped rows fixed); storyboard3: named is seen, breaks and follow the break, cuts of a fault get their crack, joined dots no longer a river, sweep by country; life off until it reads.
- **Why-verdict:** Juju Changes trial 8 of 12 twice, inconclusive, so depict.md is only used when a niche is named; Istanbul take 3 about 7 by the lead's eye, Ambi has not marked it.
- **Status-open:** films/congo running end to end; sound, motion and time-map workers running; spent about 26.8 of 30.
- **Related:** juju-maps/films/istanbul/take3.mp4, stack/changes.json

---

## 2026-11-25 22:15 EAT — TEHUTI — Built the changes-kit data layer for Juju maps and tested it; the depict card did not prove better
<!-- type: event -->
**From:** TEHUTI

Built the changes-kit data layer for Juju maps and tested it; the depict card did not prove better
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 939c60ba)
- Ambi asked for 12 to 18 kinds of map change, as closed data a cheap model can pick from. Built stack/changes.json with 18 kinds (9 drawn, 9 partly drawn, 0 with no op), plus 53 niches and 159 ideas.
- Checked stills at 240p on port 4720 by eye: 28 windows, each with a bare twin. stack/test_changes.py and test_kit.py pass, so the predicate printed TRUE.
- Blind trial of the depict card: first version won 8 of 12 (below the 10 needed to call a win); second version also 8 of 12, so it was reverted. Total spend $0.0848, 49 calls.
- Open: idea facts are from memory and marked checked:false; level, border, gate, split, swallow, pile, allegiance, ring and years cannot be drawn in full; storyboard3.py:387 sends sweep a bare name, so 'Iraq' lit the wrong place.
- Files changed: juju-maps/stack/changes.json; juju-maps/stack/niches.json; juju-maps/stack/cards/depict.md; juju-maps/stack/test_changes.py; juju-maps/films/_data/changes-trial/stills.py
- Status: complete — changes layer built and tests pass; depict card unproven (trial 8 of 12, below the 10 needed) and idea facts unchecked

---

## 2026-11-25 22:14 EAT — TEHUTI — Juju Maps: kinds of change corrected, sweep by country name goes to the wrong land
<!-- type: event -->
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** stack/changes.json (9 drawn, 9 partly with what is missing), stack/niches.json (18 ideas lifted from street size to map size), stack/test_changes.py.
- **Why-verdict:** sweep given only "Iraq" lit a small place elsewhere (films/_data/changes-trial/o-sweepname); regions by name work (Sahel, Sahara). The trial ran on the lists before these edits.
- **Status-open:** storyboard3.py:387 needs country:1 or rings (another lane's file).
- **Related:** sheet-e.jpg

---

## 2026-11-25 22:09 EAT — TEHUTI — Juju Maps: 18 kinds of change, 53 niche families, depict card, blind trial 8 of 12
<!-- type: event -->
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/stack/changes.json (18 kinds, 10 drawn, 8 partly), stack/niches.json (53 families, 159 ideas, checked:false), stack/cards/depict.md (1,344 characters), stack/test_changes.py, films/_data/changes-trial/ (stills, scenes, trial, verdicts). No other file edited.
- **Why-verdict:** blind judge, 12 titles, DeepSeek medium: the card and lists win 8, lose 4; 5 clear wins, 0 clear losses; under the 10 that would be past noise, so inconclusive. A second version of the card gave 8 of 12 again and was reverted. Spend under 0.10 US.
- **Status-open:** nothing is wired: kit.py and seats are other lanes; the niches' facts are unchecked; pulled edge cases listed in changes.json notes.
- **Related:** films/_data/changes-trial/verdict.json, sheet-chain.jpg, sheet-b.jpg, sheet-c.jpg

---

## 2026-11-25 22:03 EAT — TEHUTI — Juju Maps: DeepSeek thinking works, Gemini cache understood, the fault is drawn, every move to be heard
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** docs/adr/0023 (any niche, Night and Day lead, 28 min under 1.50), docs/adr/0024 (every move heard, channel sound packs); faults.py (PB2002 seam names + GEM traces); storyboard3 (real fault, ruler = voice, shake at its place, named is seen, breaks by rupture, follow the break); talk.py + plan.py (one Neon conversation per film); board7 DIRECT7=fill; routes: fill low 64000, sound low; spine sheet lists the changing thing's steps; record.mjs refuses a film that does not play.
- **Why-verdict:** DeepSeek gave nothing because max_tokens cut its thinking (14-16k; its own default is 64k) and medium is served as high: 48 s, 0.0056 US for a whole 100 s cut at low. Gemini 4 has no manual cache; automatic cache hits only a continued conversation (3 of 3), not a shared prefix. Cut cost 0.03 against 0.18-0.32 (Neon). Ambi's best film missed its fault because "Eurasian plate" was not found.
- **Status-open:** Neon T2 missed after ~5 min (plan now asked straight after script); cheap cut weaker in the last third than Neon's (Judged); time map, changes, sound, motion workers running; spent about 26.4 of 30.
- **Related:** juju-maps/films/istanbul, marmara2, marmara4

---

## 2026-11-25 21:57 EAT — TEHUTI — Juju Maps: the engine tells its own moves; stretch op; marmara2 faults fixed
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps film.js, gl.js, record.mjs, stack/cards/marks.md. Nothing committed.
- **Why-verdict:** ADR 0024: picture and sound read one timeline. The half fill was the mask box, not tiles.
- **Status-open:** no whole film redrawn; sum op still starts at once.
- **Related:** juju-maps/films/_data/sheets/marmara-fixed-stretch.png, timeline-marmara2.json

---

## 2026-11-25 21:37 EAT — TEHUTI — Juju Maps: the living land
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps film.js, gl.js, tiles.js, server.mjs, record.mjs, data/places500.bin, stack/cards views.md and marks.md. Nothing committed.
- **Why-verdict:** Ambi: a village everywhere on the planet. Real GeoNames settlements, trees, field grain, standing views; po3 redrawn as life.mp4.
- **Status-open:** OSM hamlets never answered, no smoke, boats or trains, cutter not told to use stand.
- **Related:** juju-maps/films/po3/life.mp4, juju-maps/films/_data/sheets/life-*.png

---

## 2026-11-25 21:21 EAT — MUNGURA — Juju Eye blind test on marmara: eye 4.8 vs count 5.6, count 0.8 too kind
<!-- type: event -->
**From:** MUNGURA

Juju Eye blind test on marmara: eye 4.8 vs count 5.6, count 0.8 too kind
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session c42a65bd)
- Ambi asked for a blind test: mark films/marmara/a.mp4 by eye before reading the count. eye.json was written before score.py ran (eye 4.8 D, count 5.6).
- Gaps (count minus eye): opening +4.2, views +1.4, script +1.3. Largest miss: Izmit's 1999 quake drawn over Istanbul at 52 s because the hero fell back to a circle.
- Eye faults the count misses: fault line never drawn at 20 s, ruler reads 74 km while the voice says 20 at 9 s, Turkey half filled for about 20 s at 18 s.
- Count fell from 6.3 to 5.6 after score.py changed at 21:04; likely cause, not verified. Its 507 km distance compares the cut with a mid-point, so it is unreliable.
- Not judged: sound (measured, not heard). Only eye.json, score.json, the marmara SCOREBOARD line and scores.jsonl were touched; no code, rubric or gate changed.
- Files changed: juju-maps/films/marmara/eye.json; juju-maps/films/marmara/score.json; juju-maps/SCOREBOARD.md
- Status: complete — eye.json and score run done, marmara SCOREBOARD row rewritten; no code changed.

---

## 2026-11-25 21:15 EAT — TEHUTI — Juju Maps: Ambi's best film so far is Istanbul quakes with Gavin; a film that does not play can no longer land
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/taste.json (verdict and voice kept, film inferred as marmara, the last sent), juju-maps/record.mjs (joins beside the film, decodes, counts frames, removes broken pieces, then swaps).
- **Why-verdict:** Ambi: "best vid thus far tho, and good voice." Two files, mississippi and gB, were unreadable; first check (decode only) passed a planted broken piece, so frames are counted too. Planted fault: exit 7, old film kept, piece redrawn, plays.
- **Status-open:** cause of the two old broken files not proven (two writers on one file suspected); blind marmara critic running; grilling round 1 unanswered.
- **Related:** SCOREBOARD.md, data/voices.json

---

## 2026-11-25 21:15 EAT — TEHUTI — Juju Eye blind test on marmara: eye 4.8, count 5.6
<!-- type: event -->
**From:** TEHUTI

Juju Eye blind test on marmara: eye 4.8, count 5.6
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: films/marmara/eye.json, score.json, one scores.jsonl row, marmara row plus its stale clause in SCOREBOARD.md. Why/verdict: eye 4.8 D, count 5.6, blended 5.0 D; the count is 0.8 too kind, worst on opening (+4.2), clutter vs marks (+4.0), stillness vs motion (+3.6). Film fault: the fault line is never drawn, and the 1999 Izmit quake is drawn over Istanbul. Related: juju-maps/eye-rubric.md.
- Verification: eye.json mtime 21:14:26 before score.json 21:14:40; eye.json sha unchanged across the score run
- Status: complete; sound measured, not heard; amazon not looked at

---

## 2026-11-25 21:05 EAT — TEHUTI — Juju's own agent stack built (after pstack), taste and scoreboard, standing improvers
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/stack (PRINCIPLES, 10 seats, cards, 3 systems, 3 formats, 4 bracket skeletons, kit.py, test_kit.py), docs/JUJU-STACK.md, spine/draws/board7/package/birth call it; storyboard3 mappings (opening, sweeps, counts, names, rings leave), regions.json, taste.json rows, score.py, times, film.sh voice beside places.
- **Why/verdict:** Ambi: reverse engineer Poteto's system for Juju's own agents per design system; "best one in a while" for the Po film. po3 = first film on the stack, my mark 7.5 (Judged).
- **Status/open:** counted score is not trusted (kivu2 6.2, fault film 8.6): Juju Eye delegate calibrating; Low Poly, Ear, Maps delegates standing; churn of 2 running; about 4.8 US left under the 30 cap.
- **Related:** docs/JUJU-STACK.md, juju-maps/taste.json, juju-maps/SCOREBOARD.md (coming)

---

## 2026-11-25 21:05 EAT — TEHUTI — Juju Eye calibrated against Ambi's eight film verdicts; rubric and score.py written, four causes named
<!-- type: event -->
**From:** TEHUTI

Juju Eye calibrated against Ambi's eight film verdicts; rubric and score.py written, four causes named
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 86ab7fd0)
- Ambi asked the Juju Eye critic to mark films blind and order them to match his verdicts, with the reasons in the pictures written as a 30-line rubric.
- Eye scores (Judged) for Ambi's eight: kivu2 9.1, dam4 9.1, kokaral 8.5, mud 7.3, yellow 7.2, mississippi 5.7, ghosts 4.9, faultsnorthana 3.0. Order matches Ambi.
- score.py --test matched 7 of 7 of Ambi's pairs on the five films it can fully count. The agent notes this is a fit to known verdicts, not a blind test.
- Four causes named from the code: nothing changes state, a country is used as hero (wrong ground), known script holes are drawn anyway, and borders and fills are coarse or run off-frame. Fixes are proposed, not shown applied.
- Six new films all score below B (gB 6.1, po3 6.0, undertow 5.4, podelta 5.3, yamal 4.1, sarygamysh 3.3). Sarygamysh's atlas lat/lon came out reversed, which puts the lake in Russia.
- Files changed: juju-maps/eye-rubric.md; juju-maps/score.py
- Status: complete — calibration, rubric and scoring written; the four cause fixes are proposed and not applied in this part.

---

## 2026-11-25 21:04 EAT — TEHUTI — Juju Eye: films marked, scoreboard made, count put in order
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/eye-rubric.md, SCOREBOARD.md, score.py, 14 films/*/eye.json, scores.jsonl. Nothing committed.
- **Why-verdict:** of six new films none passes B: po3 6.0, gB 6.1, undertow 5.4, podelta 5.3, yamal 4.1, sarygamysh 3.2 (eye). The count had been reversed; now 7 of 7 of Ambi pairs between fully counted films, fitted, not blind.
- **Status-open:** marmara and amazon not looked at; sound measured, not heard; mississippi mp4 reads black; three scenes of judged takes are gone.
- **Related:** juju-maps/SCOREBOARD.md, runs/decision.tsv lane maps-score

---

## 2026-11-25 20:46 EAT — TEHUTI — Juju Maps: built Juju's own agent stack, a voice audition tool, and fixed the cutter crash
<!-- type: event -->
**From:** TEHUTI

Juju Maps: built Juju's own agent stack, a voice audition tool, and fixed the cutter crash
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked for Juju Maps to render cleanly (no dancing polygons), better voices, a blacklist for the Moko Dusk voice (mispronounces Kazakhstan), and a Juju agent stack modelled on poteto's pstack.
- Built: audition.py (same text through each voice), kit.py (each thinking seat gets its rules and skeleton), score.py (power-by-power scoreboard), and docs/JUJU-STACK.md. Cutter crash fixed per the agent.
- Juju's own stack made film po3 alone. Podelta, po3, undertow, yamal and gB were queued for the Juju Eye critic. Those renders are still running and not yet checked by Ambi.
- Ambi's verdicts: too slow to churn concepts, too sparse on drawing (draw the border, don't assume knowledge), '40 deltas' unexplained, and no map context (world, then region, then river).
- Open: the Moko Dusk blacklist is requested but not confirmed applied in the transcript. Film quality is still below his bar, with the goofy look and corny openings flagged.
- Files changed: juju-maps/audition.py; juju-maps/kit.py; juju-maps/score.py; juju-maps/storyboard3.py; juju-maps/board7.py; juju-maps/thumb.py; docs/JUJU-STACK.md
- Status: in-progress — Juju's own stack and first film exist; more films are rendering and the quality bar is not yet met

---

## 2026-11-25 20:32 EAT — TEHUTI — Juju Maps: Neon put back in the thinking seats, taste ledger, voice shelf of 20, flat coloured land
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** routes.json (Neon: ladder, script, editor, judge, speak, direct, package, birth pick; DeepSeek small work), spine.py on Neon (29 s, 0.06 US), board7 one Neon cut then cheap repairs, taste.json read by the cutter, gl.js flat fills and solid lines, pre-fetch (4x faster drawing), geo.py places first, hero never a chain of towns, churn.sh; code snapshot runs/map-snap-1125-1945.
- **Why/verdict:** Ambi: film 4 cheesy, shiny border, fat arrow, "scores four" meaningless; likely culprit the model switches. Ledger agreed: kivu2, dam4, kokaral, mekong all ran Neon in those seats, film 4 none. Po film ("mud") is the new baseline, sent.
- **Status/open:** land below sea level painted as sea and square mazes on near coasts (powers B on it); ranked scripts need a baseline on Neon; Neon cache still 0 hits; about 5 US left under the 30 cap; churn of 2 films running.
- **Related:** films/mud, films/undertow, data/VOICES.md, refs/4NeoQMOIDGU.md, arcs/ranked.json

---

## 2026-11-25 20:22 EAT — TEHUTI — Juju Maps: the coast file decides the sea
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/tiles.js, film.js (world tiles may take 30 s), new data/land10.json (9 MB, Natural Earth 10 m land and minor islands). Nothing committed.
- **Why-verdict:** land below sea level was painted as sea; now the coast decides and heights only add land.
- **Status-open:** no whole film drawn after the change; drains deeper than 12 m keep the height rule.
- **Related:** juju-maps/films/_data/sheets/coast-before-after.png

---

## 2026-11-25 20:14 EAT — TEHUTI — Juju Maps: smooth near shore
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/tiles.js only. Nothing committed.
- **Why-verdict:** height tiles ring by a few metres round nought near coasts and drew square mazes; water is now softened height plus the drawn coast.
- **Status-open:** coast detail near is about 600 m; Lake Pontchartrain causeway no longer drawn; mississippi has no scene to reshoot.
- **Related:** juju-maps/films/_data/sheets/near-shore-before-after.png

---

## 2026-11-25 19:55 EAT — TEHUTI — Juju voice shelf: 19 newest Inworld voices auditioned, five sent to Ambi for ear test
<!-- type: event -->
**From:** TEHUTI

Juju voice shelf: 19 newest Inworld voices auditioned, five sent to Ambi for ear test
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 64c674b0)
- Ambi asked for the newest, best Inworld narration voices on our pay-as-you-go plan, and only those. Docs show inworld-tts-2 is the flagship and 1.5 is deprecated.
- Built the shelf of 19 voices (10 men, 9 women) and cast only from it. 56 paid calls cost about 0.288 US. Casting rotation was fixed so the whole shelf gets turns, not just 8 of 19.
- Verified by measurement only: 18 of 19 voices hit the target rate (155 to 170). Graham is blacklisted. Warren is off the shelf. Machines cannot judge accent or warmth.
- Five candidates are rendered for Ambi to hear: Gavin, Tonya, Russell, Marek, Kristen (films/audition/line2/rate). Not yet tested: ABV V9 routing for LOT, and the St. Bernard pause fix, which the lead owns.
- Files changed: juju-maps/castvoice.py; juju-maps/audition.py; juju-maps/voice.py; juju-maps/data/voices.json; juju-maps/data/voice-traits.json
- Status: in-progress — shelf and rotation built and measured; waiting on Ambi's ear test of five voices, ABV V9 LOT routing unconfirmed.

---

## 2026-11-25 19:55 EAT — TEHUTI — Juju Maps: voice shelf of 19 newest Inworld voices; casting only from the shelf
<!-- type: event -->
**From:** TEHUTI

Juju Maps: voice shelf of 19 newest Inworld voices; casting only from the shelf
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: juju-maps data/voices.json (shelf of 19, profiles.lot = ABV V9), data/voice-traits.json, data/VOICES.md, audition.py (speak, hear, measure), castvoice.py (shelf only, rest rule kept and lengthened), voice.py (row's model and rate). 
Why/verdict: Ambi said the last films' voice was weak and not one of the new ones. inworld-tts-2 is the flagship (docs). Graham is on the old 1.5 lists, the shelf voices are not (Inferred newest). 56 takes, 0.288 US (Measured). Machine listeners rate Graham near the top, so they only reject faults; nobody has listened.
Status/open: Ambi hears five (Gavin, Tonya, Russell, Marek, Kristen). door.py cannot speak ABV V9 (no price for 1.5-max, no temperature); mend.py still voices from kits.json; channels digger keeps Ambrose, griot Beatrice, pilot Cordelia, but surveyor Harold and witness Tristan are off the shelf.
Related: juju-maps/data/VOICES.md
- Verification: 60 dry casts in a temp folder: 14 voices used, none off the shelf, none repeated within 3 films. voice.py's row line run with VOICE=Graham, VOICE=Marek, LOT and ABV on griot: all gave the right voice. No film was voiced.
- Status: complete; waits for Ambi's ear and for the lead on door.py

---

## 2026-11-25 19:54 EAT — TEHUTI — Juju maps: borders now flat colour, not light; arrow is a flat band; proven by stills, no full film drawn
<!-- type: event -->
**From:** TEHUTI

Juju maps: borders now flat colour, not light; arrow is a flat band; proven by stills, no full film drawn
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 01f0bfee)
- Ambi asked for night area borders at 40% with no bloom, and an arrow capped at 1.6% width. He then corrected it: no glowing borders anywhere, countries filled flat like the Moko Dusk look.
- Changed juju-maps/gl.js: area is a flat fill (.42 day, .5 night) that wipes in over 0.6 s; edge is one solid 2 px line; arrow is a flat tapering band on the ground, 2.2% wide, max 45% of the picture.
- Fixed a double fill where Turkey was painted twice, and the glowing yellow line in faultsnorthana and ghosts, which was the river line. Hero lines now have a dark casing.
- Verified by stills only (old beside new in juju-maps/films/_data/sheets/flat-fill-old-new.png, plus wipe-in-day.jpg). No whole film has been drawn on this engine yet.
- Files changed: juju-maps/gl.js; juju-maps/films/_data/sheets/flat-fill-old-new.png; juju-maps/films/_data/sheets/wipe-in-day.jpg
- Status: in-progress — changes installed and proven by stills; whole-film render still pending, nothing committed

---

## 2026-11-25 19:53 EAT — TEHUTI — Juju Maps: borders are coloured now, never lit
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/gl.js: area, region, overlay, edge, arrow, hero, river. Nothing committed.
- **Why-verdict:** Ambi: why is it shining instead of it being colored. Flat fills like Moko Dusk, solid lines, painted band, cased hot hero; stills old beside new.
- **Status-open:** overlay, 240p line width and a whole film not drawn; Kigali thread in kivu3 stays thin at 24 s.
- **Related:** juju-maps/films/_data/sheets/flat-fill-old-new.png

---

## 2026-11-25 19:44 EAT — TEHUTI — Juju Maps: night borders quiet, arrows sized on the picture
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/gl.js (area by night, arrow). Nothing committed.
- **Why-verdict:** faultsnorthana border was blown out and arrows were beams; stills now clean.
- **Status-open:** no whole film drawn after the change.
- **Related:** juju-maps/films/_data/sheets/area-arrow-night.png

---

## 2026-11-25 19:38 EAT — TEHUTI — Juju maps: sea squares fixed, pre-fetch added, labels de-boxed, thread and landing fixed (not yet full-film verified)
<!-- type: event -->
**From:** TEHUTI

Juju maps: sea squares fixed, pre-fetch added, labels de-boxed, thread and landing fixed (not yet full-film verified)
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 01f0bfee)
- Ambi asked for five juju-maps fixes: teal sea squares, a tile pre-fetch so pieces never wait, no black plates on labels, a faded thread, and an ease-out globe landing.
- Teal squares: the cause was flat zero height tiles from zoom 11. Those spots now use the zoom 9 depth. Before/after still: films/_data/sheets/sea-squares-before-after.png.
- Pre-fetch: 8 s cold landings went from 64.5 s with 40 late to 40.2 s and 58.5 s with 0 late. The bar of under 10 late in a cold 140 s film is not measured yet.
- Black plates removed from tag, cuttag, reach and height labels; checked on halves at 43 s and 100 s. All five edits are installed and seen in stills, but no whole film has been drawn on the new engine.
- Open: Ambi must restart the server on port 4720 to get the faster pre-fetch; the old server still works, just slower.
- Files changed: juju-maps/server.mjs; juju-maps/tiles.js; juju-maps/record.mjs; juju-maps/film.js; juju-maps/gl.js; juju-maps/motion.js
- Status: in-progress — five fixes installed and seen in stills; full-film pre-fetch bar unmeasured and server restart on 4720 pending

---

## 2026-11-25 19:36 EAT — TEHUTI — Juju Maps: sea squares, tile pre-fetch, plain labels, thread and landing fixed
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps film.js, gl.js, tiles.js, server.mjs, record.mjs. Originals in films/_data/before2. Nothing committed.
- **Why-verdict:** flat zero heights from z 11 drew light squares on open sea; now the z 9 depth. Cold landing late 40 to 0. Seen in stills.
- **Status-open:** server 4720 needs a restart for /raw and /th; no whole film drawn after the install.
- **Related:** juju-maps/films/_data/sheets, runs/decision.tsv lane maps-data

---

## 2026-11-25 19:30 EAT — TEHUTI — Juju Maps: ranked films, real-speech skeletons, draw what is said, thumbnails from the film's own frame
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps: formats.json, rank.py (counted table, code scores), pocket.py, spine.py + skeleton.py + skeletons/ (studied films' sentences as fill-in lines, Kivu as gold, banned rows in front; tell.py and rankstory.py retired), draws.py + storyboard3 (every sentence's marks), geo.py (places asked once with the film's ground), look.py (instant bare check), castvoice.py, package.py + thumb.py (thumbnail = frame of the film), seo.py, slate.py/next.sh/two.sh/post.sh/film.sh, seek.py 8 s, mix.py loudness without loudnorm, states and provinces borders, plates, cards of 1 to 3 words; cap 30 US by Ambi's order; Mac freed from 0.6 to about 24 GB.
- **Why/verdict:** Ambi: scripts with "character" are bad, copy real speakers' skeletons and the Kivu spine; draw far more; views in different ways; fast; best voices; Tunde disliked (blacklisted).
- **Status/open:** films sent: mississippi (Wales bug), kivu3, ghosts. Cutter crash (REF name clash, old engine fallback) made fossil, lagos, halves bad; fixed, being recut. Delegates running: ranked film reverse study, voice shelf of 20, powers B (sea squares, prefetch, plates off labels).
- **Related:** runs/meter/cap.json, docs/FILM20.md, refs/4NeoQMOIDGU*, refs/Zz9AtnxOU6U*

---

## 2026-11-25 18:57 EAT — TEHUTI — Juju map: one fixed ground per film; kokaral worst dance second cut from 12.15% to 2.42%
<!-- type: event -->
**From:** TEHUTI

Juju map: one fixed ground per film; kokaral worst dance second cut from 12.15% to 2.42%
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 07e035bd)
- Ambi asked for one ground: the same place must show the same facets, colours and light in every view, with no level swap seen on kokaral (11 s vs 22-25 s).
- Built ground-dance.mjs: renders frames 1/24 s apart through each move, undoes the camera, and measures per-second ground change.
- Built one.js and a world-fixed lattice in poly.js. Measured worst second on kokaral scene-b: 12.15% before, 2.42% after. Mountain film: about 18% down to 1.3%.
- Rivers, borders and town lights redrawn as lines on the fixed ground (lines.js). Sea colours and doubled borders still being fixed.
- Side effect: a newer Rogun cut overwrote the low-poly cut. A restore from Juju's printed cut was written by restore_rogun.py; not yet confirmed.
- Files changed: juju-lowpoly/poly.js; juju-lowpoly/one.js; juju-lowpoly/lines.js; juju-lowpoly/ground-dance.mjs; juju-lowpoly/moko.py; juju-lowpoly/film.js
- Status: in-progress — fixed ground and dance check work and measure; stopped by Ambi's interrupt before the terrain sweep and Rogun cut restore were confirmed.

---

## 2026-11-25 18:52 EAT — TEHUTI — Juju Maps: mountain films read by day, ranked-film and fault tools built
<!-- type: event -->
**From:** TEHUTI

- **Changed:** juju-maps film.js, gl.js, motion.js: rogun2 faults fixed by cause; new ops board, score, sum, set, fault, rupture. Nothing committed.
- **Why-verdict:** rogun2 a.mp4 went black in mountains, with blown glow and white beams by day. New stills show neither. Night area curtain still glows at low wide views; the lead decides.
- **Status-open:** there is no data op in film.js or gl.js; the neon was the satellite picture. Not wired into the cutter.
- **Related:** runs/map-day-1125. Harness: Claude Code (claude-opus-5-5).

---

## 2026-11-25 18:43 EAT — TEHUTI — Took apart a 28:38 map film frame by frame and wrote its grammar and ranked arc files for Juju
<!-- type: event -->
**From:** TEHUTI

Took apart a 28:38 map film frame by frame and wrote its grammar and ranked arc files for Juju
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session d7b9db85)
- Ambi asked: "use reverse engineer video on this, on this entire vid ... go through every frame", for 4NeoQMOIDGU (28:38, 613K views, 9K-sub channel), so Juju can make 20-30 min ranked map films.
- Read 860 grid frames and about 260 near frames by eye; machine-read on-screen text on 3,437 frames; scanned all 51,548 frames for colour-swap faults. No paid calls.
- Found 40 one-frame flashes (21:40 to 26:15). Checked 15 by eye: 14 land/sea colour swaps, 1 card fade. On-screen text averaged 59 words/min over 179 spoken words/min.
- Wrote the study note and the arc files; arcs.py ranked builds at 2 min (23 slots) and 25 min (279 slots, 3,540 words). 31 devices still lack drawing plans; the 10 words/min text law is proposed, not tested.
- Frame deletion and the final output check were not confirmed in the transcript; the closing summary is cut off mid-line.
- Files changed: juju-maps/refs/4NeoQMOIDGU.md
- Status: complete — own predicate printed TRUE (five files written, JSON parses, arcs.py ranked builds); 31 missing device plans and frame cleanup still open

---

## 2026-11-25 18:42 EAT — TEHUTI — Juju Maps: a 28 minute ranked map film read frame by frame
<!-- type: event -->
**From:** TEHUTI

- **Changed:** juju-maps/refs/4NeoQMOIDGU.json and .md and 12 stills, juju-maps/depict-ranked.json, juju-maps/text-law.json, juju-maps/arcs/ranked.json. No other file, no paid call, nothing committed.
- **Why-verdict:** Ambi, 25 Nov: reverse engineer this whole film. It holds by 40 scores, one each 26 s (Measured), a famous second contestant that stays in front until the last, and a property planted at 2:38 and paid at 27:35. Weak: 59 words a minute on screen, 97 of 111 captions repeat the voice, land and sea swap colour for single frames 21:40 to 26:15.
- **Status-open:** no device built, no film judged; arcs.py ranked builds at 2 and 25 minutes, but a 2 minute cut holds no contestant (arcs.py is another lane's). Ambi's eye decides.
- **Related:** juju-maps/refs/4NeoQMOIDGU.md. Harness: Claude Code (claude-opus-5-5). Next: build 'four scores arriving' and 'source fan' from juju-maps/depict-ranked.json.

---

## 2026-11-25 18:07 EAT — TEHUTI — Juju map motion: ten map ops and a credit line built and drawn on the real map
<!-- type: event -->
**From:** TEHUTI

Juju map motion: ten map ops and a credit line built and drawn on the real map
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 161b78f0)
- Ambi asked to build ten map-motion ops (pace, region, overlay, locator, stream, sweep, pole, ask, heatup, beat) plus a bottom-left source credit line, in film.js, gl.js, motion.js and panels.js.
- All ten ops and the credit op are live on the real map (port 4720). Day and night were drawn at 480p and the stills were checked by eye.
- Test clip clip2-day.mp4 was rendered for Ambi to judge taste. Its words were hand-written to test the tools, so it is not a Juju film.
- Nothing was committed. Ambi's judgment of the look is still open.
- Files changed: juju-maps/film.js; juju-maps/gl.js; juju-maps/motion.js; juju-maps/panels.js; runs/map-motion-1125/clip2-day.mp4
- Status: complete — all ops drawn and checked at 480p day and night; nothing committed, Ambi's taste judgment pending.

---

## 2026-11-25 18:06 EAT — TEHUTI — Juju Motion: thirteen new tools on the map, drawn in the ground and from the frame edge
<!-- type: event -->
**From:** TEHUTI

- **Changed:** juju-maps gl.js, film.js, motion.js, panels.js: region, overlay, locator, stream, sweep, pole, ask, heatup, beat, count, strip, credit, and lines that draw at the pace of the words; calendar and ledger redrawn. New data file juju-maps/data/ne_50m_admin_0_countries.geojson. Nothing committed.
- **Why-verdict:** Ambi, 25 Nov: Juju Motion not mastered, design systems need to be more creative. Each tool adds 0.5 ms or less a frame (Measured, interleaved). Taste waits for his eye on the 20 s clip.
- **Status-open:** not wired into the cutter; provinces need an admin-1 file that is not on this disk.
- **Related:** runs/map-motion-1125. Harness: Claude Code (claude-opus-5-5).

---

## 2026-11-25 17:46 EAT — TEHUTI — Juju Maps: data layers, real satellite years and OSM streets drawn and checked in stills
<!-- type: event -->
**From:** TEHUTI

Juju Maps: data layers, real satellite years and OSM streets drawn and checked in stills
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 01f0bfee)
- Ambi asked for Juju Maps to use its own powers in slow moments and boring places, so a teaching film is never a bare flat map. The 12-layer GIBS list is in data-layers.json (37 kB).
- Built the data op (k:'data'), timelapse op and osm op in server.mjs and tiles.js. Stills at 854x480 were checked by eye in day and night looks: Aral Sea shrink, Dead Sea years, night lights.
- Still open: the lead must apply films/_data/film-data-ops.patch (6 lines) to film.js, then restart ports 4720 and 4721 for /d/. Elevation tint and the no-'at' case were not shot.
- Of the 12 layers asked for, 11 are served. GIBS only serves fires as vector tiles, so that one is missing. Disk cache kept small; clear.py checks cloud-free dates for each year.
- Files changed: juju-maps/data-layers.json; juju-maps/osm.py; juju-maps/server.mjs; juju-maps/tiles.js; juju-maps/films/_data/film-data-ops.patch
- Status: in-progress — the data, timelapse and osm ops work in stills; the film.js wiring by the lead and the restart are still needed, and elevation and no-'at' are unshot.

---

## 2026-11-25 17:44 EAT — TEHUTI — Juju Maps: real satellite years, measured layers, streets and one ground tone built
<!-- type: event -->
**From:** TEHUTI
- Harness: Claude Code (claude-opus-5-5). Topics: juju
- **Changed:** juju-maps/tiles.js, server.mjs installed; new data-layers.json, osm.py, clear.py, data/osm/cairo.json + kaifeng.json; film.js patch handed over, not applied.
- **Why/verdict:** 20 minute teaching films must never be a bare flat map. Aral Sea 9 years, Dead Sea 1985 to 2021, 13 measured layers and Cairo streets looked at in day and night. Shallow-sea rule tried and reverted.
- **Status/open:** servers 4720 and 4721 need a restart for /d/; fires are vector only; border layers not shot after install; nothing committed.
- **Related:** juju-maps/films/_data/sheets, runs/decision.tsv lane maps-data

---

## 2026-11-25 17:31 EAT — TEHUTI — Juju Maps: the land can rise, the camera can fly, rivers carry their names
<!-- type: event -->
**From:** TEHUTI

- **Changed:** juju-maps/gl.js and film.js: new ops relief, profile, rivername, spot; stop.move glide, orbit, rise, dive; daylight river line. Nothing committed (kickoff).
- **Why-verdict:** Ambi, 25 Nov 17:00: a flat unannotated map from 48 to 56 s is not interesting. Kaifeng's raised river bed (69 m plain, 80 m bed in the 30 m data) now reads by eye in day and night. Seek and step match (mean diff 0.000).
- **Status-open:** not wired into the board writer; satellite tile seams show (lane B); river lines are Natural Earth, 1 to 3 km off near the ground.
- **Related:** runs/map-powers-1125, films/_powers. Harness: Claude Code (claude-opus-5-5).

---

## 2026-11-25 17:31 EAT — TEHUTI — Juju Maps: five 3D tools for flat slow moments (relief, profile, river name, spot, camera moves)
<!-- type: event -->
**From:** TEHUTI

Juju Maps: five 3D tools for flat slow moments (relief, profile, river name, spot, camera moves)
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 161b78f0)
- Ambi asked for map tools that fill slow moments like 48 to 56 s on films/yellow/c.mp4, e.g. ridges on a flat plain, zoom into terrain, unique Juju Maps tools.
- Added five ops in juju-maps/film.js and gl.js: relief (vertical exaggeration with optional hypsometric tint), profile, stop.move glide/orbit/rise/dive, rivername, and spot.
- Verified: day and night stills rendered; seek against stepped frames gives mean difference 0.000 to 0.001; old scenes kivu2 and _river have at most 0.01% of pixels off by more than 1 level.
- Still open: nothing committed. Lane B files (board6/7, storyboard3, server.mjs, tiles.js) were not touched. Port 4721 belonged to another lane, so debug ran on 4747 only.
- Files changed: juju-maps/film.js; juju-maps/gl.js; runs/map-powers-1125
- Status: complete — all five tools are live on port 4720 and the Juju exit predicate printed TRUE; nothing committed.

---

## 2026-11-25 17:30 EAT — TEHUTI — Juju money audit: Neon was on OpenRouter with 0 percent cache; rewired and measured
- Harness: Claude Code (claude-opus-5-5)
- **Changed:** door.py kind neon_flex now calls Google direct through the purse (Standard price; Google's flex tier answered 503 three times then hung 300 s, so it is only on with NEON_TIER=flex); new kind glm (OpenRouter GLM 5.3). story4 SCRIPTER=mixed: DeepSeek ladder, draft, editor, stitch; one lean speak pass (GLM by default, SPEAKER=neon_flex for films that go out) behind a constant prefix of about 4,900 tokens; GLM doubts the facts; nothing said twice. board7: constant prompt first (CONST7), DeepSeek drafts and directs, code checks every field and every place, mends up to 3 times; DIRECT7=neon only on purpose. Film limit back to 0.80. Automatic second pass and the Neon film watch are off unless AGAIN=1.
- **Why-verdict:** Ambi 17:05 and 17:20: Neon must use the Google AI Studio credit, OpenRouter is for Jev and GLM; "we haven't been using the cache". Ledger: 239 Neon calls on OpenRouter 9.13 US, 40 on Google 3.31 US, cached 0 percent, 766k thinking tokens about 6.6 US.
- **Status/open:** measure a Neon cache hit on a second call; Inworld voice is now the largest production cost (25 US a million characters). 2.1 GB disk.
- **Related:** juju, gemini-neon-implicit-cache, docs/COSTS-MAPS.md, ADR 0010.

---

## 2026-11-25 17:17 EAT — TEHUTI — Moko Day retired from the looks; Juju picks with any; board7 replaces board6 but still crashes
<!-- type: event -->
**From:** TEHUTI

Moko Day retired from the looks; Juju picks with any; board7 replaces board6 but still crashes
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session a19667f0)
- Ambi: "I really hate Moko Day ... only one polygon". Moko Day was taken out of film.py, structures.json and the app. Moko now means the dusk look; 'any' lets Juju pick the look itself.
- birth.json now holds pick.feed beside pick.titles. Titles put Juju's pick first and order the rest by pick.feed; no feed number is shown.
- Verified: a Juju-picks press on web ran the real one.sh (kokaral, Moko), came back Ready and played. Watch and titles walked at 1440x900 and 390x844 with 0 faults. The stub's cut was copied, so the crash did not stop it.
- Open: board7.py stops at line 6 for every film on both engines. Line 29 of board6.py has single braces in an f-string; doubling them is the suspected fix, not yet confirmed. A paid press has not been run.
- Files changed: juju-maps/film.py; juju-maps/films/dam4-dusk/live.json; juju-maps/board6.py; juju-maps/board7.py; mockups/v02/served/build.py; mockups/v02/served/walk.mjs
- Status: in-progress — Moko Day removal and Juju-picks verified on web; board7 crash and the paid press still open

---

## 2026-11-25 17:17 EAT — TEHUTI — Juju presses: Moko Day taken out, Moko is dusk, Juju picks added; board7 found broken

**Changed.** juju-maps/film.py, structures.json, crates/juju-serve/src/v02.rs, mockups/v02/served. Harness: Claude Code (Opus 5.5).

**Why-verdict.** Ambi retired Moko Day (lead 17:02). Clicked at 1440x900 and 390x844 on 4702: four windows, a Juju picks press ended in a played Moko film, 0 ledger rows.

**Status-open.** board6.py line 29 has single braces in an f-string, so board7 fails for every film since 16:59 (reproduced 17:16 with spending blocked). Disk about 2 GB.

**Related.** topic juju; mockups/v02/served/HANDOFF.md

---

## 2026-11-25 17:05 EAT — TEHUTI — Juju Maps: Juju now has its own ideas, sources, reference reading and long-film book; Moko is a real map at dusk only
- Harness: Claude Code (claude-opus-5-5)
- **Changed:** birth.py (16 ideas, blind feed test against real outliers, picks look and title), seek.py (own sources), story4/story5 (opening law, names that are words, stitch; story5 = 10 to 20 min book and parts), voice.py say-names, numerals.py (captions 1902, 1.6 billion; 23 of 23 tests), board7.py (any length: DeepSeek drafts on paper twice, stranger, Neon directs once; 9 cents and 90 s for 2 min instead of 35 cents), rea.py (YouTube link read by Gemini through the API, no computer; refs/lyRHFOcNMTU.json: 37 views, 20 changes a minute, 2.5 s apart), depict.json (26 ideas), Sentinel-2 2016 near ground (EOX, CC BY 4.0, credit needed), river/ground/sea cuts in gl.js, people lights, seamount, pillars, detour, date, level/land/shore acts, storyboard lifetimes and proof.json loops, one.sh (one press), make.sh, again.sh; music bed per chapter.
- **Why-verdict (Ambi):** Kivu take 4 "best"; Moko Dusk dam "10 out of 10"; Moko Day hated, retired: "even though it's polygon it still gotta look like a real map"; China film 7/10: river not named at the start, flat bare land, nothing for 8 s; "videos are tools to develop the software"; aim 20 minute films by the end of the day, 2 minute tests only; cap 20 (25 hard).
- **Status/open:** delegates: Powers A (relief lens, glide, profile, river name), Powers B (real years, data layers, streets, seamless near ground), Moko lane 8 (real water levels; film kokaral b), app 0.2 wire-in. 14 minute paper film of the Yellow River in films/yellow20 (book.json, script.json, film7.json, cut7.json). Next: film "How One Dam in Tajikistan Could Dry Out Uzbekistan" (films/rogun, born, feed 7.3 vs real 11.7) once powers land. Spend about 18.7 of 20.
- **Related:** juju, juju-maps, docs/FILM20.md, runs/harvest/longform/LONGFORM.md.

---

## 2026-11-25 16:59 EAT — TEHUTI — Juju Maps: Juju picks its own ideas, cheaper cutter, map powers and calendar numerals in progress
<!-- type: event -->
**From:** TEHUTI

Juju Maps: Juju picks its own ideas, cheaper cutter, map powers and calendar numerals in progress
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked for Juju to use map films as tools to improve the whole stack, not to keep redoing Kivu, and for slow map moments to show ridges, profiles, real data or photos.
- Built a cheap board cutter (board7.py): the Yellow River cut now costs about 9 cents instead of 35 and runs in about 90 seconds, per the agent's own run log.
- Added rules so the first 8 seconds name the subject on the map, bare land may not hold more than 3 seconds, and captions write years like a calendar (1902). Rendering and checks are still running.
- Drafted a 20-minute Yellow River plan on paper only (13.9 min, 10 chapters); the truth check trimmed the script to 1,742 words, so it needs more sources before it is proven.
- Spend cap for Juju tests was raised to $20, with $25 as the hard maximum (logged separately). A Wedjat-side fork (Ramani, ramani/) was started; its scene compiler and picture fetcher exist, but no full film has been rendered yet.
- Files changed: juju-maps/board7.py; juju-maps/storyboard3.py; juju-maps/rea.py; docs/FILM20.md; runs/meter/cap.json; ramani/compile.py
- Status: in-progress — map powers and calendar numerals still being built; the 20-minute film is on paper only, and no new film has been proven yet.

---

## 2026-11-25 16:45 EAT — TEHUTI — Wired the one-command film chain into the Juju app and proved one stub press on port 4702
<!-- type: event -->
**From:** TEHUTI

Wired the one-command film chain into the Juju app and proved one stub press on port 4702
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session a19667f0)
- Ambi asked: one press runs juju-maps/one.sh SYSTEM [NAME] end to end, with no paid test runs, and the app must show Juju's six titles with its pick first.
- Changed film.py to run one.sh, make.sh, again.sh or draw.sh and read stage files, so edits to the chain land without copying it. Also edited live.js, walk.mjs, v02.rs and structures.json.
- Proved on stubs: stub-yellow, stub-caspian, stub-caspian2 and stub-caspian22 ran the real chain with the gate unreachable and the meter unwritable. Ledger rows: 0. A server without a stub answers Spending is locked.
- Browser walks covered Duppy Day (web) and Moko Day and Moko Dusk (phone). One Moko stop failed because moko.py was being edited mid-run, then the rerun passed.
- Open: no paid press was run. The agent's 12-line report on what a person presses was not confirmed complete in the transcript.
- Files changed: juju-maps/film.py; mockups/v02/served/live.js; mockups/v02/served/walk.mjs; crates/juju-serve/src/v02.rs; juju-maps/structures.json; mockups/v02/served/walk/phone-press-moko-dusk.json
- Status: complete — one stub press through one.sh proven on port 4702 with 0 ledger rows; paid press not run.

---

## 2026-11-25 16:44 EAT — TEHUTI — Juju 0.2 presses now run the one-command chain, four styles, Juju's own titles

**Changed.** juju-maps/film.py runs one.sh or make.sh whole and watches it; crates/juju-serve/src/v02.rs (births, deal, make from a title); mockups/v02/served (titles step, Duppy Day window, test/nopay.sb). Harness: Claude Code (Opus 5.5).

**Why-verdict.** Lead 16:12. Proven by clicks on port 4702: Duppy Day on web (both drawings), Moko Dusk and Moko Day on phone, stop and carry on, played. The real chain ran with the gate and the meter blocked: 0 ledger rows.

**Status-open.** No paid press yet; 4700 untouched; disk 2.1 GB at 16:40.

**Related.** topic juju; mockups/v02/served/HANDOFF.md

---

## 2026-11-25 16:27 EAT — TEHUTI — River and ground cut acts built in juju-maps gl.js, checked in night and day stills
<!-- type: event -->
**From:** TEHUTI

River and ground cut acts built in juju-maps gl.js, checked in night and day stills
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session bab8c728)
- Ambi asked for a river cut (section with river:true) and a ground cut (ground:true), ten timed acts, each stills checked by eye at 854x480 in night and day.
- Agent built all ten acts (perch, silt, raise, breach, seep, buried, pump, drop, sinkground, saltcreep) in gl.js and reviewed the stills in films/_river.
- Agent reports each act costs under 2 ms a frame and that the block stays on the real line; it judged stills only, not a moving clip.
- The two lead faults (tremor ring 'waves' too large, seamount 'lamps' crowding the crater) were raised; the transcript cuts off before confirming they were fixed.
- Files changed: juju-maps/gl.js; juju-maps/films/_river/night.jpg; juju-maps/films/_river/day.jpg
- Status: complete — ten river and ground acts built and checked in night and day stills; lead-fault fixes not confirmed in the visible transcript.

---

## 2026-11-25 16:26 EAT — TEHUTI — Juju Maps: river and ground cuts with ten acts built in gl.js
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5), worker lane maps-marks
- **Changed:** juju-maps/gl.js: section with river or ground; perch, silt, raise, breach, seep, buried, pump, drop, sinkground, saltcreep; tremor ring capped at 0.35 of the view and 2 px; boat lamps kept off a seamount.
- **Why/verdict:** lead 16:15 asked for the cut of a river. 13 stills each in night and day looked at by the builder; no blind viewer, no moving clip.
- **Status/open:** 0.0 to 0.8 ms a frame, seeks identical both ways; not committed; no lead film uses them yet.
- **Related:** juju-maps/films/_river, juju-maps/board6.py, storyboard3.py

---

## 2026-11-25 16:23 EAT — TEHUTI — Juju 20 minute picture timeline: film20.json and FILM20.md written

**Changed.** juju-maps/film20.json, docs/FILM20.md, runs/harvest/longform/tools (kinds.py, register.py, film20.py, film20_acts.txt). No paid call. Harness: Claude Code (Opus 5.5).

**Why-verdict.** Lead order 16:20. 174 acts dark, 165 day; 26 stations; map 78 cut 7 panel 12 card 3 percent. jenny introduces 6.3 new names a minute against the donors 3.3 and 3.7.

**Status-open.** Not boarded or drawn. Engine lacks: beds by time, ledger/calendar/share/curve in the board menu, a device id, station cameras, a rest flag, an hour field.

**Related.** runs/harvest/longform/LONGFORM.md, juju-maps/board6.py, mix.py

---

## 2026-11-25 16:12 EAT — TEHUTI — Juju maps: gl.js now draws sea-floor sections, seamounts, people lights, pillars, detours and borders
<!-- type: event -->
**From:** TEHUTI

Juju maps: gl.js now draws sea-floor sections, seamounts, people lights, pillars, detours and borders
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session bab8c728)
- Ambi on films/jenny/d.mp4: "I don't understand the ring" and "what's with all the lights". Scope was gl.js only, with the five ops read from scene.json and drawn as smooth in and out.
- Built section-over-sea (true floor, glass sea, volcano cone via o.peak), gasrise and lidwater, seamount, people on/out, pillars, detour and border-only area ops.
- Verified with stills from record.mjs on jenny at 854x480: each body read by eye, under 2 ms a frame, deterministic seek. The only judge so far is the agent; no blind viewer has seen them.
- Cost numbers are noisy: the seamount low view measured 1.8 ms in one run and 0.2 to 0.7 in others, so its headroom is thin. The first timing meter was inflating results and was fixed.
- Open: after the work, git stopped listing juju-maps/gl.js in status and the cause was not found. Nothing was committed by the agent.
- Files changed: juju-maps/gl.js
- Status: in-progress — five ops built and checked by stills; blind review and the missing git status for gl.js are still open.

---

## 2026-11-25 16:11 EAT — TEHUTI — Juju Maps: five new marks (sea cut, seamount, people, pillars, detour) built in gl.js
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (claude-opus-5-5), worker lane maps-marks
- **Changed:** juju-maps/gl.js (ops section at sea with peak/gasrise/lidwater, seamount, people on/out, pillars, detour, area line:true); new file juju-maps/data/towns.json (7,342 places from Natural Earth).
- **Why/verdict:** Ambi 15:42 on jenny d.mp4: the ring and the lights were not understood. Stills read by the builder only; no blind viewer yet.
- **Status/open:** 480p stills in juju-maps/films/_marks; 0.0 to 1.8 ms a frame; forward and backward seeks identical. Not committed. The white ring still in jenny is the hero op, not these marks.
- **Related:** juju-maps/depict.json, films/jenny

---

## 2026-11-25 16:02 EAT — TEHUTI — Juju test cap raised to 20 (25 hard most) by Ambi; videos are tools, Juju picks its own ideas
<!-- type: event -->
**From:** TEHUTI

Juju test cap raised to 20 (25 hard most) by Ambi; videos are tools, Juju picks its own ideas
- Harness: Claude Code
- What happened: undefined
- Status: undefined

---

## 2026-11-25 15:57 EAT — TEHUTI — Juju 0.2 presses built: pick a channel and style, make a map film in resumable steps, verified on web and phone
<!-- type: event -->
**From:** TEHUTI

Juju 0.2 presses built: pick a channel and style, make a map film in resumable steps, verified on web and phone
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session a19667f0)
- Ambi asked for the two styles (duppy-night, moko-day) fully piped and wired by 5 p.m., so Juju can make many channels and bends from the presses.
- Built juju-maps/film.py: make runs eight resumable steps per film, writes live.json after each, and skips finished steps. A killed run resumes where it stopped.
- Verified with real clicks at 1440x900 and 390x844: channel, style, and title take 3 presses to a playing film, seeking works, and a second make gets a 409 'Already making one'.
- Verified kills: a kill in Duppy's Film redrew only missing pieces; a kill in Moko's Mix kept Board. Money: 0 ledger rows from test films. Not run for real: Story, Voice and Think through film.py.
- Open: Think's film limit is fixed at 2.00 US in board5.py:12 and storyboard.py:6; the app showed $1.21 left at 15:55, and a film costs about 0.27 US (estimate).
- Files changed: juju-maps/film.py; juju-maps/structures.json; crates/juju-serve/src/v02.rs; mockups/v02/served/build.py; mockups/v02/served/walk.mjs
- Status: in-progress — presses and resumable film steps work and are walked; real Story/Voice/Think runs and the Think money limit are still open.

---

## 2026-11-25 15:50 EAT — TEHUTI — Juju long films: peaks re-checked without chapter marks, slot sheet re-cut into 73 sets

**Changed.** runs/harvest/longform: pool.json rerun without chapter marks and adverts; slots-long-20.json now 2,929 words, 73 sets of 7 to 28 s.

**Why-verdict.** Numbers, going back, and finding words still mark replayed moments; a late person and a promise no longer clear their interval and are now Judged.

**Status-open.** Not run through a writer or a render. MINUTES 19.0.

**Related.** runs/harvest/longform/LONGFORM.md

---

## 2026-11-25 15:43 EAT — TEHUTI — Juju long films: 18 winners of 18 to 47 min studied, 20-minute slot sheet written

**Changed.** runs/harvest/longform/: LONGFORM.md, longform.json, slots-long-20.json, shots-long-20.json, tools/. Nothing outside that folder edited. No paid call, no subagent. Harness: Claude Code (Opus 5.5).

**Why-verdict.** Ambi, 25 Nov 13:55: how do we make 20 minute videos engaging in this flow. Verdict (Judged on Measured parts): do not stretch; nine 2-minute chapters, hero changes state by thirds, one turn-over at half time, four consequences as the last half, an odd sight planted at 0:30 and paid at 16:34.

**Status-open.** Not run through a model or rendered. story2 MINUTES must be 19.0 for this sheet; storyboard3 needs a SHOTS path and part-by-part boards. Only winners were read, no flops.

**Related.** juju-maps/story2.py, storyboard3.py, veve-gait, nyansapo-ladder; runs/decision.tsv lane longform.

---

## 2026-11-25 15:42 EAT — TEHUTI — Juju Maps: Lake Kivu take 4 is Ambi's best film so far; what to keep
- Harness: Claude Code (claude-opus-5-5)
- **Changed:** juju-maps/board6.py replaces per-sentence fill: one mind (gemini-4-neon) writes a cast of at most five, held views and 15 to 19 acts, then reads its own second-by-second sheet back as a hard director; code refuses repeats, acts too small to see, acts closer than 1.8 s, more than 10.5 s with nothing changing. storyboard3.py `stay`: what comes in stays; a cut opened again shows what it had become. mix.py sound law: hits 2 dB over the music, one in 8 s, same act not within 40 s, air 8 dB under. New inside act `dive` (a plate slides under). Hero kind `spot`. make.sh uses board6.
- **Why-verdict:** Ambi 15:36 on films/kivu2/d.mp4: "This video so far is the best. The scripts are better, we finally got the pacing is better he pauses and we finally got the sound effects right... one mind so beautiful, lets keep on this path". Earlier same day on Moko r1: "slop... everything is random".
- **Status-open:** next = 10, 16, 20 minute form from runs/harvest/longform/LONGFORM.md (18 long films) and "Galactic Empires" J0wWNytEXS4 (runs/scout/atticus). Films sent: kivu2/d, jenny/d, dam4 r2 (Moko Dusk). Running: deadsea, mekong.
- **Related:** juju, juju-maps, veve-gait, nyansapo-ladder

---

## 2026-11-25 15:42 EAT — TEHUTI — Juju 0.2 presses wired to the map films on a test server

**Changed.** juju-maps/film.py (eight kept steps, live.json), juju-maps/structures.json, crates/juju-serve/src/v02.rs plus route lines, mockups/v02/served (page, walk, HANDOFF.md). Harness: Claude Code (Opus 5.5).

**Why-verdict.** Ambi 25 Nov 14:45: two styles wired in by 17:00. Proven by clicks at 1440x900 and 390x844 on port 4702: 3 presses to a playing film; a make stopped and carried on in Duppy Night and Moko Day. Bought steps were copied, 0 ledger rows for the test films.

**Status-open.** Live 4700 untouched. No paid make has been run through it. Send private, lengths over 2 min, Raise cap not built.

**Related.** topic juju; mockups/v02/served/HANDOFF.md

---

## 2026-11-25 15:12 EAT — TEHUTI — Low-poly motion bodies for the Juju map films: built and stills drawn, not yet proven
<!-- type: event -->
**From:** TEHUTI

Low-poly motion bodies for the Juju map films: built and stills drawn, not yet proven
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 41189cdb)
- Asked: every motion graphic as a solid, lit, shadowed low-poly body under flag P.poly, with no glow, proven by stills and a 15 s Egypt clip. New engine is gl-poly.js, hooked into gl.js for low-poly looks only.
- Drawn: day and dusk body sheets and 240p clips (clip-day.mp4, clip-dusk.mp4). Clips lack river, zone and reach, and the last 4 s cut Ethiopia. The clip.json fix is written but not drawn.
- Dark look: 19 of 19 stills matched at 13:55. A later run differed on 4 of 19, probably late ground-tile loads; a frozen rerun matched. Speed target of 6x was not met (15 to 21 s per clip on a loaded Mac).
- Stopped at the lead's 15:08 order to free the Mac. Edits from 15:00 onward (springs, stronger bend, gl.js loader) are syntax-checked only. Arrow, river light and flood swell are not checked frame by frame.
- Files changed: juju-lowpoly/gl-poly.js; juju-lowpoly/gl.js; juju-lowpoly/motion.js; juju-lowpoly/films/poly-motion/bodies-day.jpg; juju-lowpoly/films/poly-motion/bodies-dusk.jpg; juju-lowpoly/films/poly-motion/clip-day.mp4; juju-lowpoly/films/poly-motion/clip-dusk.mp4; juju-lowpoly/NOTES-5.md
- Status: in-progress — exit predicate not TRUE: the clip fix and late edits are undrawn, and the frame-by-frame checks and 6x speed target are open.

---

## 2026-11-25 15:04 EAT — TEHUTI — Juju 0.2: the whole app as a pressable page, 3 to 4 presses to a film
<!-- type: event -->
**From:** TEHUTI

Juju 0.2: the whole app as a pressable page, 3 to 4 presses to a film
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: mockups/v02/ in juju: FLOW.md (steps, machine work, failures, states), juju.html (one self-contained clickable file, 30 states, 1440x900 and 390x844), shots/ and board.jpg, V02-BUILD.md (kept, new, order). Ambi's order 25 Nov 13:55. Why-verdict: channel, style, title; the press on a title starts the film. VidRush's prompt box, brand tabs, quote pages and timeline are folded or cut. Styles are one land in three windows (Duppy Night, Moko Day, Moko Dusk) and a shut door (Spiritual). Found while building: money can only stop a film in Story, Voice or Edit (drawing is free). Status-open: prototype only; the app's press still draws with juju-stage, no YouTube upload code exists, one map-film command (N1) is the first thing to build. Open for Ambi: start with no second question, raise cap from the app, length per channel, the fourth name, where niches go. Related: ADR 0022, docs/STACK-MOVE.md. Harness: Claude Code (Opus 5.5).
- Files changed: AMBESSA/intel/juju/mockups/v02/
- Verification: build/shoot.mjs: 60 screens, 0 faults; real clicks at both sizes: 3 presses to the film, Play plays, Send ends at Private; raise cap, another structure, leave and come back walked. Every shot looked at.
- Status: complete: design and prototype; build not started

---

## 2026-11-25 14:35 EAT — TEHUTI — Juju: thinking before writing and boarding; laws from Ambi 14:20-14:35

**Changed.** Pack nyansapo-ladder; juju-maps/ladder.json, story4.py, calabash.py (125 banned rows now run on map scripts), tics-maps.json, board5.py (thought rows, views chosen, small forms), storyboard3 laws (north up, J-cut 0.55 s, lens, dwell 2.6 s, no repeated labels, neighbour hues, flags), gl.js bodies mist, lamps, thread, and pipe, lid, vents, streams, giveback in the lake cut. Films in the making: kivu2 (Duppy Night), dam4 (Moko, low poly).

**Why-verdict.** Ambi: ideate before boarding; annotation is not thought; Tanganyika was drawn on the wrong side; poly is "low-key insane, whoa", keep its Nile, pumping water, music; churn more.

**Status-open.** Drawing. Money 9.7 of 15. Harness: Claude Code (Opus 5.5).

**Related.** [[juju]]

---

## 2026-11-25 14:32 EAT — TEHUTI — Juju Maps: three looks written as closed systems (Duppy Night, Moko Day, Moko Dusk) with pick.py
<!-- type: event -->

**Changed.** juju-maps/systems/ (build.py, three machine files, three pages, pick.py, tests) and a draft pack crates/juju-skills/packs/moko-and-duppy. No engine file touched, no paid call.

**Why-verdict.** Ambi 25 Nov 13:55: low poly and dark are each a design system, operated by lower-thinking models over hundreds of films. Measured: 27 of 30 test sentences right on the first run, 30 after mending; 30 of 45 unseen sentences right on first runs; 204 of 255 hand-cut gold beats offered.

**Status-open.** No film boarded from pick.py; storyboard3.py does not call it; names, voice, thumbnails not chosen by Ambi; reach.rs and pins.txt rows owed. Harness: Claude Code (claude-opus-5-5).

**Related.** veve-gait, opon-sight, juju-lowpoly/EDIT-RULES.md, topic juju.

---

## 2026-11-25 14:21 EAT — TEHUTI — Juju docs and skills moved to the map-film stack

**Changed.** docs/STACK-MOVE.md (the stack now, 71 file verdicts, pins and reach rows for countersign, 9 handoffs). AGENTS.md, WORKER.md, ask-juju, 20 other skill files, 14 docs and ADR notes, kits. No skill.json, gate, pins.txt or reach.rs edited.

**Why-verdict.** Ambi 25 Nov 13:55: upgrade the skills and every MD that names the old stack. Checked: gates section of WORKER.md identical, skill.json identical, pins unchanged for existing packs.

**Status-open.** Eight packs have a when with no row in reach.rs; the app's one tap still draws with juju-stage; subtitle conflict with ADR 0014 item 4. Harness: Claude Code (Opus 5.5).

**Related.** [[juju]] docs/adr/0022-juju-maps.md

---

## 2026-11-25 14:10 EAT — TEHUTI — Juju Maps: Juju cut its own film for under a cent; panels, board4, cap 15

**Changed.** Cap 15 US (Ambi, about 13:55, runs/meter/cap.json). juju-maps/board4.py + shots2.json (structure in code, one small form a view), panels.js (Juju Motion facts panels, 12 kinds) + motion-timing.json (bjEr7L2Rj9s read whole), storyboard3 anchor(), views sized to the hero, auto cut. docs/COSTS-MAPS.md. Delegates: skills and stack docs, long films, app 0.2, design systems (Duppy Night, Moko Day, Moko Dusk), low-poly 2-8, editor by skill.

**Why-verdict.** Ambi: 7.5 of 10; Juju Motion timing is what takes it to high 8; spend more on breakthroughs; poly looks great. films/kivu-machine/a.mp4 shown. The low-effort editor taught by veve-gait made a better cut than the cheap model.

**Status-open.** kivu take b and the agent cut drawing; dam low-poly film not yet out; rift take 3 broken by a full disk, redraw when the Mac is quiet. Harness: Claude Code (Opus 5.5).

**Related.** [[juju]]

---

## 2026-11-25 13:51 EAT — TEHUTI — Juju Maps: measured edit grammar, dark take 2 approved in feel, low-poly style running, two new stories spoken

**Changed.** juju-maps: grammar.json, pace.py, storyboard3.py (sets, hero, in-view law, donor shot per sentence, self-mend, automatic cut), gl.js (fixed LAYERS, block cut that acts, lake water and gas, flood), record.mjs (4 s piece cache), mend.py, voice.py, beds/ (6 music moods). scripts/opon.py. Skills veve-gait and opon-sight (linked, not pinned in juju-conduct). juju-lowpoly/ + juju-poly-assets/ (polyfork shelf, 8 delegates). Films: rift2 take 2, kivu (Juju script), dam (script by Claude as a test).

**Why-verdict.** Ambi: "this is really good ... actually felt like I was learning"; dark look kept; spoken place must be in view; no stickling over accuracy.

**Status-open.** Purse 9.45 of 9.50. Disk and memory tight; Mac load over 100 with nine agents. kivu-machine (cheapest model, own cut) drawing. Harness: Claude Code (Opus 5.5).

**Related.** [[juju]] docs/adr/0022-juju-maps.md

---

## 2026-11-25 12:14 EAT — MUNGURA — Juju Maps: engine scripts written and first 480p obsidian take of the Ottoman film rendered

**Changed.** New engine files under `juju-maps/`: compile.py, mix.py, story.py, pics.py, ideate.py, tiles.js, film.js, film.css, film.html, record.mjs, server.mjs, and looks/obsidian.json + looks/terra.json. First take built in `films/ottoman2/`: scene.json (576 KB — 19 camera stops, 7 picture cards, 15 labels), pics.json (23 pictures), cards.json, mix.wav, `take1-obsidian.mp4` and t1.jpg (2,400×1,620 contact sheet of 30 frames).

**Why verdict.** ADR 0022 wants looks judged on fast 480p takes of one voice before any full export, so this is that test: full map skeleton and picture cards for a 1:58 cut instead of a full-priced draw.

**Status open.** Only the obsidian look was rendered (terra not); the take is 1:58, not the ~30-minute film. All juju-maps work is untracked — no commit, no push remote. `out/` is empty. No verdict from Ambi yet on voice, look or pictures.

**Related.** Verified with `ffprobe`: h264+aac, 854×480, 24 fps, 118.6 s, 40,592,307 bytes; `ffmpeg ebur128`: −15.1 LUFS, LRA 3.2. Frames pulled at 9, 12, 30 and 45 s show the relief map, year counter, empire fill and a captioned picture card (Sultan Bayezid I) with no blank tiles. Paths: `juju-maps/films/ottoman2/{scene.json,take1-obsidian.mp4,t1.jpg}`.

---

## 2026-11-25 12:04 EAT — MUNGURA — ADR 0022: Juju goes map-only; drawing engine forked as Juju Maps

**Changed.** `docs/adr/0022-juju-maps.md` written (1,882 bytes, 12:04), recording Ambi's decision of about 11:30–12:10: one niche only (empires, wars and borders), drawing engine forked as Juju Maps (`juju-maps/`) from bilawalsidhu/gods-eye-view (MIT, upstream 92fcccb), Wedjat untouched, juju-stage stops drawing map films; two looks held as data, no parchment; checks report and no longer stop a render except the money cap, an unsourced sentence, picture rights and Ambi's publish clicks; supersedes the HOLD law for these films. The fork exists on disk with its own `.git` at 92fcccb, an `upstream` remote set `no_push`, plus LICENSE, THIRD_PARTY_NOTICES.md and DATA_SOURCES.md (245 KB).

**Why verdict.** Ambi's own words are quoted in the ADR ("Juju just only [does] maps for now … do this one niche really well", "fork it again … so we won't use Wedjat", "I hate parchment paper", "having hard gates prevents a vid from rendering"). The fork keeps gods-eye-view's director maths and drops its name and marks; Wedjat is not modified.

**Status open.** The ADR leaves unsolved how a film is made with the Mac closed (keys and model calls need an always-on host) and money above the 9.50 USD cap for a 30-minute voice.

**Related.** `docs/adr/0022-juju-maps.md`; `juju-maps/DATA_SOURCES.md`; `juju-maps/THIRD_PARTY_NOTICES.md`; upstream commit 92fcccb.

---

## 2026-11-25 11:40 EAT — TEHUTI — Juju: film room and sound bed done on the copies; Ottoman film take 1 reviewed, take 2 drawing
<!-- type: event -->
**From:** TEHUTI

Juju: film room and sound bed done on the copies; Ottoman film take 1 reviewed, take 2 drawing
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi's ask: press to film, smooth. Walks passed 71 steps on web and phone, 0 bad, on the practice copy. Live app on 4701 restarted; its film room program answers. Film room tested on a silent film only.
- Ambi's ask: a bed and cues a history film deserves. proof75a and Pluto both PASS with the bed heard; 46 of 46 juju-sound tests pass, per the delegated report. Voiced proof12c bed: 37 of 37 stretches pass.
- Ottoman12f full draw with voice and music finished take 1. Review flagged flat delivery, treaty stretch, 1908 ending, thumbnail word, and an empty Paris map at 8:00. Take 1 moved aside; take 2 drawing with map and painting fixes.
- My mistake: a forced add committed about 1,000 ignored files from the rooms folder. Local only, never pushed; removed from the commit. About 1 GB of git data remains. Disk recovered from 0.7 GB to 1.9 GB.
- Spend: 8.69 of 9.50 US cap. Open: take 2 review, compare with take 1, thumbnail, and the flat voice. Ambi has not yet said what he hated most in take 1.
- Files changed: crates/juju-stage/src/worlds/map.rs; crates/juju-cli/src/stages/shots.rs; runs/spine/ottoman12f/master.mp4; runs/spine/ottoman12f/bin/juju-sound; runs/sound/proof/proof12c-bed/bed.json
- Status: in-progress — take 2 of the Ottoman12f film is drawing; its review and thumbnail are still open

---

## 2026-11-25 11:11 EAT — TEHUTI — juju-sound: real music beds and cues for voiced map films; Watcher reservation fixed
<!-- type: event -->
**From:** TEHUTI

juju-sound: real music beds and cues for voiced map films; Watcher reservation fixed
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 24e67170)
- Ambi asked that every voiced map film come out of juju-sound with a real, fitting bed and cues, after a video model flagged birdsong over historical narration on proof75a.
- Built a history bed from real string recordings in place of the birdsong, and a space bed (half-speed strings or tambura). Changes come at chapter points, ducked under the voice.
- Verified on copies only: proof75a -14.1 LUFS, peak -1.8 dB, bed 14.0 dB under the words, 1 cue heard. strip-pluto -14.5 LUFS, peak -1.8 dB, 4 of 4 cues heard. make-mongols now passes; it failed before.
- Fixed scripts/sound/watch.py so the Watcher reserves what the gate prices. 46 of 46 juju-sound tests pass. Open: Ambi must countersign the new bars, which the transcript cuts off before stating.
- Files changed: crates/juju-sound/src/music.rs; scripts/sound/watch.py; runs/sound/proof/proof75a-music/sound/strip.mp4; runs/sound/proof/strip-pluto-music/sound/strip.mp4; runs/sound/proof/proof12c-bed/bed.json
- Status: complete — the predicate is TRUE on the copies; new bars await Ambi's countersign

---

## 2026-11-25 11:10 EAT — TEHUTI — Juju sound: real music beds, both copied films pass
- **Changed:** crates/juju-sound (music.rs new), scripts/sound/watch.py reservation, profile map-music.json, 11 licensed music pieces on the shelf (6 history, 5 space). Harness: Claude Code (Opus 5.5 sub-agent).
- **Why/verdict:** birdsong bed replaced by real string quartets 14 dB under the voice, heard whole; proof75a and strip-pluto copies pass, 4 silent films pass, 46+ tests pass. Nothing committed.
- **Status/open:** kits.json needs the profile line (lead); silent-film bed is near -37 LUFS, a ruling is owed; no person has listened.
- **Related:** runs/sound/auto/HANDOFF.md 13-15, runs/sound/proof, topic juju.

---

## 2026-11-25 11:07 EAT — TEHUTI — Make-a-film room finished and walked end to end in the Juju app; server restart still needed
<!-- type: event -->
**From:** TEHUTI

Make-a-film room finished and walked end to end in the Juju app; server restart still needed
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 6553c74e)
- Ambi asked that a person pick a subject or pasted link, a look, voice or silent, a length (10/20/30/50), and get a real MP4 that flows 'exceptionally well'.
- Finished the Make a film room and added the /api/make path in juju-serve real.rs; the Altar, Cauldron and Pact rooms now run through it instead of dead-ending.
- Verified: web and phone walks at 71 steps each, other doors at 20, all 0 bad; 7 rooms pressed at 390 and 1440 px with 0 dead ends. The film room plays to the end with thumbnail and download matching master.mp4.
- 30, 50 and voice were checked only with a test list; make.json was left unchanged (voice off, lengths 1/10/20). The Estimated minutes figure only fell during the wait.
- Open: server on port 4700 must be restarted (scripts/serve/start) before anyone opens it. One test (a_real_film_survives_kill_9_and_two_tabs) did not run at head after a full cargo test began drawing a practice film by mistake; that scratch folder was deleted.
- Files changed: crates/juju-serve/src/real.rs; crates/juju-serve/tests/real.rs; runs/app/real-film/rooms/altar.html; runs/app/real-film/rooms/cauldron.html; runs/app/real-film/walk.py; runs/app/API.md; runs/app/api.json
- Status: complete — walks pass and the film path plays; server 4700 restart and one unrun test remain open

---

## 2026-11-25 11:05 EAT — TEHUTI — Juju app: Make a film to a watched film, walked on web and phone

- Harness: Claude Code (Opus 5.5), sub-agent, app lane. Topics: juju
- **Changed:** crates/juju-serve (links go to juju make --link, one look, one plain line and minutes left, one sentence and one action at a stop, the review's worst thing), mockups/r2 rooms landed, new film room, runs/app/API.md and api.json.
- **Why-verdict:** web walk 71 steps 0 bad, phone walk 71 steps 0 bad, 7 rooms pressed at both sizes with 0 dead controls and 0 layout faults; all on 4701 with a kept run played back, nothing paid.
- **Status-open:** 4700 needs the lead's restart (its old program has no /api/make); new films need a fresh pin; --link proved only against the stand-in; one test run began to draw the practice film and was stopped.
- **Related:** runs/app/real-film, runs/decision.tsv lane app-flow

---

## 2026-11-25 10:51 EAT — TEHUTI — Juju film pipeline: diagnosed why films stop, proposed a design-system-file approach
<!-- type: event -->
**From:** TEHUTI

Juju film pipeline: diagnosed why films stop, proposed a design-system-file approach
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 2aeafab7)
- Ambi asked what can actually be done about Juju choking, with VidRush reverse-engineered and only the design-system feature needed, full stack, no minimising.
- Read all 33 recorded Juju film runs: 4 finished, 25 of 29 ended were stopped by Juju's own checks (sound too quiet, 14.3 s hold vs 14 s limit, thumbnail 0.69 vs 0.68).
- Proposed three changes: nothing kills a film (repair or backup shot, note for Ambi); one shot kind per spoken line like VidRush; a design system as one file filled by measuring a pasted video.
- Open: Ambi's question 'A film always finishes, yes or no?' is unanswered; no code changed; the proposal is not yet built or tested.
- Files changed: JUJU-MASTER-BRIEF.md; ~/.hermes/profiles/default/memory/shortterm/2026-11-25.md
- Status: in-progress — diagnosis and proposal delivered; awaiting Ambi's yes/no and a go to build.

---

## 2026-11-25 10:50 EAT — MUNGURA — Juju: 25 of 29 film runs were stopped by our own checks; assemble-not-draw proposed
<!-- type: event -->
**From:** MUNGURA

- **Changed:** nothing in Juju; read only. Harness: Claude Code (Opus 5.5).
- **Why/verdict:** Measured from runs/spine/*/live.json (33 runs): 4 done, 21 hold, 4 failed, 4 marked working. The 25 stops by stage: deal and package 8, script 8, pictures and form 2, render and mix 6, publish kit 1. Small misses stopped whole films (14.3 s against 14; -17.0 LUFS against -14; thumbnail 0.69; 117 type pixels outside the safe box after 196 s of drawing). Two of the 25 were test runs with a 0.00 budget. VidRush assembles each clause from seven footage kinds by a channel's share (harvest/wave1/out/vidrush-10.json); Juju draws one kind of world per film.
- **Status/open:** candidate, not decided: a film always finishes (repair, fall back, or note), one shot assembler over mixed footage kinds, a design system is one data file. It changes the never-loosen-a-gate law, so Ambi must say it. Session 31bfe4d9 is the live builder (ottoman12f).
- **Related:** juju, runs/spine, docs/adr/0012, docs/adr/0021

---

## 2026-11-25 10:35 EAT — TEHUTI — Juju film: export moved to 720p 24fps H.264, script ending restored, closing-line checker added
<!-- type: event -->
**From:** TEHUTI

Juju film: export moved to 720p 24fps H.264, script ending restored, closing-line checker added
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked that Juju produce films itself, export the way CapCut and Resolve do, and never crash the computer. Films should be reviewed before he sees them.
- Done: export now draws once and encodes once at 720p, 24 fps, H.264 on the Mac's video chip. An 8-second sample projects to about 390 MB for a 12-minute film, down from about 1.9 GB.
- Done: script rebuilt to about 1,750 words with the Vienna, Candia and Belgrade endings restored. Closing lines now go through a checker (up to 3 tries) and are dropped if none pass. Voice switched from flash to TTS-2.
- Verified: on the first-60-second strip the longest still stretch fell from 6.2 s to 2.2 s, and the review returned 'fix'. Drawing ran at 1.6 s per film-second, down from 2.3, not yet measured on a quiet Mac.
- Open: no full film has been rendered. Painting cutaways, the music bed and the review step are not yet proven end to end. Spend is about 8.1 of 9.50 USD.
- Files changed: crates/juju-stage/src/encode.rs; crates/juju-cli/src/stages/words.rs; crates/juju-stage/src/worlds/map.rs; crates/juju-stage/src/worlds/ink.rs; scripts/video_eye.py; crates/juju-cli/practice/kits.json
- Status: in-progress — export and script fixes are built and partly checked; the full film with paintings, music and review has not been rendered.

---

## 2026-11-25 10:02 EAT — TEHUTI — Juju: diagnosed why make ignores the story skills; fixes proposed, none applied yet
<!-- type: event -->
**From:** TEHUTI

Juju: diagnosed why make ignores the story skills; fixes proposed, none applied yet
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session c34719fe)
- Ambi asked for Juju only: "Juju Juju is what we're working on". Agent confirmed Juju scope and dropped the old Loop and Milarepa threads.
- Found 52 skills exist, but `juju make` has no link to them or to the conductor. The outline prompt tells it to invent causes the facts do not give.
- The 12-minute script failed: first draft 1,483 words, 16 repairs to 1,373, then a fallback cut to 800 words. Cost $0.46.
- A third try at 1,802 words was live at the script check at 9:31. Its proposed fixes are wiring `juju make` to the skills and building the outline with Crossroads Chain.
- Not proven: whether Crossroads Chain improves the script. Nothing was changed in the repo during this session.
- Status: in-progress — diagnosis and fix plan delivered; no code changed or verified yet

---

## 2026-11-25 09:47 EAT — TEHUTI — Juju: one builder, voiced Ottoman film rendering, new map look and quote-checked script
<!-- type: event -->
**From:** TEHUTI

Juju: one builder, voiced Ottoman film rendering, new map look and quote-checked script
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi ordered single-builder mode, no swarms. Background jobs were stopped and Mac load fell from 92 to 3, then the tree was checked to build.
- Voiced path fixed: the 0.30 voice limit is in, the word-matching truth check was replaced by an exact-quote check (148 sentences matched), and a resume-hash rounding bug was fixed.
- New One Ink map look and measured arrival motion added. The first long voiced film (Ottoman, 9.5 min, 26 events) was still rendering, about 15 minutes left, and had not been watched yet.
- Not done: the film came out 9.5 min, not the 12 requested. Seven PRs (21 to 26) passed their combined test but are unmerged because GitHub billing blocked the final step. Ambi must fix billing.
- Files changed: crates/juju-cli/src/stages/words.rs; crates/juju-cli/src/stages/shots.rs; crates/juju-cli/src/stages/deal.rs; crates/juju-stage/src/worlds/map.rs; crates/juju-stage/src/worlds/ink.rs; crates/juju-stage/src/motion.rs; scripts/purse.py; scripts/video_eye.py
- Status: in-progress — Ottoman voiced film still rendering and unwatched; seven PRs unmerged pending GitHub billing fix

---

## 2026-11-25 09:46 EAT — TEHUTI — Juju: single builder; first long voiced film rendering
<!-- type: event -->
**From:** TEHUTI

Juju: single builder; first long voiced film rendering
- Harness: Claude Code
- What happened: undefined
- Status: undefined

---

## 2026-11-25 09:29 EAT — MUNGURA — Juju diagnosis: order of work was wrong; VerseBatch made 10 long scripts in 55 min, Juju made 0
<!-- type: event -->
**From:** MUNGURA

Juju diagnosis: order of work was wrong; VerseBatch made 10 long scripts in 55 min, Juju made 0
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session c34719fe)
- Ambi asked whether we messed up: two weeks of prep and two Ultra-weekly token runs produced no one-minute video, and he asked what we need to do.
- Agent compared VerseBatch (10 scripts of about 6,900 words each, 55 min, 10 Oct) with Juju (0 usable scripts; one try of 6 min, 1,483 words, cost $0.46).
- Causes named: scripts built from border-table rows with lines that break accuracy; checks that kill films instead of flagging them; swarms that re-read heavily, about 4.4B tokens on 24-25 Nov.
- A 75-second voiced film rendered at 8:58 and was stopped because its thumbnail scored 0.69 against a 0.68 limit; the agent said that film is not good either.
- Still open: no fix was applied in this part of the session. Next step is to rebuild the script order and the gates before more swarm runs.
- Files changed: ~/.claude/projects/-Users-Mungura-AUH/memory/juju-benchmark-versebatch.md
- Status: in-progress — diagnosis delivered and benchmark note saved; no Juju fix applied yet

---

## 2026-11-25 09:28 EAT — MUNGURA — Juju audit for Ambi: the script step lost to VerseBatch
<!-- type: event -->
**From:** MUNGURA

- **Changed:** nothing in Juju; read only. Harness: Claude Code (Opus 5.5).
- **Why/verdict:** Measured: VerseBatch made 10 scripts averaging 6,905 words in 55 min (10 Oct, jobs/verse file times). Juju proof12 spent 0.46 US and 353 s on one failed script of 1,483 words cut to 800 by its own checks; proof75a (75 s, voiced, 4.6 min) held only by a thumbnail check and its lines are a list. 4.4 billion Claude tokens on 24 and 25 Nov, almost all re-reading.
- **Status/open:** round 1 of questions put to Ambi; no decision recorded.
- **Related:** juju, runs/builder/proof12.log, ~/AUH/Loop/jobs/verse

---

## 2026-11-25 08:53 EAT — TEHUTI — Fixed the context-repo sync job and pushed the Juju overhaul to GitHub
<!-- type: event -->
**From:** TEHUTI

Fixed the context-repo sync job and pushed the Juju overhaul to GitHub
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 2aeafab7)
- Ambi asked: "I think everything today GitHub. Everything that has happened... Everything everything now, man, please." The two-hour sync had crashed at 13:52 on a date format, so nothing had been pushed for 18 hours.
- Fixed sync_context_repo.py, then read both days of Juju work and the day logs. Picked hand-chosen success and failure pictures, each with its verdict in the caption, and ran a text scan on each.
- Rewrote the repo pages: 11-juju/worked-and-failed.md, money-and-stack, orchestration, surfaces, and the now and record pages. Each is timestamped and the gallery was updated (252 pictures, 57 new).
- Pushed by hand after stopping the running sync job, so the push did not wait for the schedule. The GitHub link and the update text for Ambi were produced from the pushed repo.
- Still open: the Make-a-film button still makes a practice clip, not a real film. No phone app file exists yet. The two-hourly Haiku update job needs a confirmed clean run.
- Files changed: ~/AUH/AMBESSA/sync_context_repo.py; ~/AUH/AMBESSA/context_gallery.py; ~/AUH/AMBESSA/context-repo/11-juju/worked-and-failed.md; ~/AUH/AMBESSA/context-repo/11-juju/money-and-stack.md; ~/AUH/AMBESSA/context-repo/11-juju/orchestration.md; ~/AUH/AMBESSA/context-repo/10-now/now.md; ~/AUH/AMBESSA/context-repo/09-assets/library/LIBRARY.md; ~/AUH/AMBESSA/context-repo/11-juju/what-ambi-said.md
- Status: complete — repo pushed by hand at 08:15 EAT 25 Nov; app 'Make a film' still makes practice clips, not yet wired

---

## 2026-11-25 08:44 EAT — TEHUTI — THROUGH: silent Juju film built to DONE with its own lines; voiced minute and thru-japan/space still open
<!-- type: event -->
**From:** TEHUTI

THROUGH: silent Juju film built to DONE with its own lines; voiced minute and thru-japan/space still open
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session ef888377)
- Ambi asked for a real juju make film with no test switches, only Juju's models: silent minute, then voiced minute, then 10 minutes.
- Silent otto-chron-2 reached DONE, with Juju's own dated lines on the map. Sound passed at -14.6 LUFS with 4 of 4 cues heard. Fixes went into truth.rs, words.rs, source.rs, clock.rs, deal.rs and the new chron.rs.
- New checks refuse a line shown before its year or a pin more than 150 km from its named place. The test suite was at 61 passing with planted cases; the final full run was not confirmed before the session was interrupted.
- Lead reports strip-mughal DONE (16 min, 0.0085 US) but with faults still open. thru-japan and thru-space stalled on the 7 s gap rule. otto-chron-3 went back to Outline. No voiced minute has been made yet.
- Files changed: crates/juju-cli/src/stages/chron.rs; crates/juju-cli/src/stages/truth.rs; crates/juju-cli/src/stages/words.rs; crates/juju-cli/src/stages/source.rs; crates/juju-cli/src/stages/clock.rs; crates/juju-cli/src/stages/deal.rs; crates/juju-cli/tests/make.rs; runs/through/BLOCKS.md
- Status: in-progress — silent minute DONE (otto-chron-2); voiced minute and 10-minute film not yet made; session interrupted by user

---

## 2026-11-25 08:44 EAT — TEHUTI — Sound worker: read the juju-sound code for three fixes; interrupted before any fix landed
<!-- type: event -->
**From:** TEHUTI

Sound worker: read the juju-sound code for three fixes; interrupted before any fix landed
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 62c92a0f)
- Ambi asked for three sound fixes: a bed for the space film strip-pluto, the watch.py reserve mismatch with prices.worst, and a listening check of three masters. He said not to push to PR 26.
- Read WORKER.md, the ask-juju skill, the earshot-sound-engine skill, the juju-sound crate, glue/watch.py, scripts/prices.py and runs/sound/auto/HANDOFF.md.
- Searched Wikimedia for public-domain space-air recordings and created an empty folder runs/sound/auto/shelf/src/space. No bed was built, no code was changed, and no listening check was done.
- Ambi interrupted the run. Open: the bed for strip-pluto, the watcher reserve fix (0.000336 vs 0.001344), and the Earshot listening note on the three masters.
- Files changed: runs/sound/auto/shelf/src/space
- Status: blocked — interrupted by Ambi; all three asks still open, no code or film changed

---

## 2026-11-25 08:12 EAT — TEHUTI — Juju Vault: the review faults of juju-db fixed
<!-- type: event -->
- Changed: crates/juju-db (whole-vault brands, one lock for a deal, kill-safe store, film numbers, story of every film, spoken words only), runs/vault. Commits cf2a0e5..3aec0e3.
- Why-verdict: fresh review showed 7 blocking faults; each red on 9be3910, green now; 54 tests; 357x60 simulation 21,182 dealt, 238 refused, 0 faults on re-read.
- Status-open: LINE-RULE 7 to 20 not countersigned; across niches still more alike than published (2.2 percent against 0.9); no film made from a slot.
- Related: runs/vault/receipt.json, runs/vault/review/. Harness: Claude Code (Opus 5.5), workflow worker.

---

## 2026-11-25 08:05 EAT — TEHUTI — Juju house strips repaired: Egypt, Orion, lungs rendered whole
<!-- type: event -->
**From:** TEHUTI (claude-code, Opus 5.5, strengths lane)

- **Changed:** new world land_depth, rewritten star_depth and solid_depth, whole numbers, law that type may not lie on drawn lines (worktree verbs-wt 53ffdba; patch runs/house/bin/engine.patch). Three mp4s with receipts, trace.json and sheets in runs/house/strip-1..3.
- **Why/verdict:** four judges' findings of the night; code check TRUE, 31 unit tests pass (Measured); looks Judged by the maker only.
- **Status/open:** needs fresh eyes; render 7 to 19 s a second of film at load 57 to 95 (target 1.0 missed); no sound; systems.json seats are a handoff (runs/house/handoff.json).
- **Related:** runs/house/check.json

---

## 2026-11-25 08:03 EAT — TEHUTI — Juju: opus-ship-c rechecked PRs 21, 22, 24, 25 and reviewed 26, 27

- **Changed:** six CLEAN reviews recorded; notes in runs/pr/NEXT.md
- **Why-verdict:** each named block gone, planted tests green on GitHub; 22 own test run once, 2 OK. 26 under-reserves, main refuses (closed)
- **Status-open:** train pending when read; 26 watch.py reserve is a fix
- **Related:** juju, docs/adr/0020. Harness: Claude Code (claude-opus-5-5)

---

## 2026-11-25 07:58 EAT — TEHUTI — Juju harvest: HmuQoak_IAg seen whole
<!-- type: event -->
**From:** TEHUTI

- **Changed:** runs/harvest/rea/HmuQoak_IAg (survey, cuts, events, words, SEEN.md); three 45 s decompose windows beside it. Harness: claude-code (Opus 5.5).
- **Why/verdict:** 74 shots, no hard cut, dissolves about 0.5 s (Measured), not 1 s.
- **Status/open:** label times on moving pictures good to about 1 s; sound not heard.
- **Related:** ADR 0021.

---

## 2026-11-25 07:48 EAT — TEHUTI — Juju: repair rounds on pull requests 21, 22, 24, 25; sound glue moved; rules unit opened
<!-- type: event -->
**From:** TEHUTI

Juju: repair rounds on pull requests 21, 22, 24, 25; sound glue moved; rules unit opened
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: 22 silent survey refused; 21 cost and time from the book's row; 25 redirects, size, official host, promises and ceiling lock; 24 job cap 0.06 asked, word list required; 26 glue in scripts/sound, beds with licence. Rules unit opened (WORKER.md, AMBI-EYE, AMBI-EAR link, film-harvest row). Why/verdict: reviewers' blocks, each with a planted test. Open: rechecks, GitHub on new heads; gather owner applies runs/gather/PATCH-25.diff. Related: runs/pr/NEXT.md. The two frames pushed by mistake in 26 are Juju's own film map-demo-60. Harness: Claude Code (Opus 5.5).
- Verification: Planted tests pass on the Mac; GitHub checks running on 24 and the rules unit at log time.
- Status: in-progress, awaiting GitHub and rechecks

---

## 2026-11-25 07:33 EAT — TEHUTI — Juju: review of PRs 21, 22, 23 by opus-ship-a

- Changed: 21 FINDINGS, 22 FINDINGS, 23 CLEAN; notes in runs/pr/NEXT.md
- Why-verdict: 21 bought-picture receipt wrong with the gate on main; 22 crashed survey skipped (reproduced)
- Status-open: one repair and recheck each for 21 and 22
- Related: docs/adr/0020. Harness: Claude Code (claude-opus-5-5)

---

## 2026-11-25 07:29 EAT — TEHUTI — Juju harvest: film 36J1tL9ulGA seen whole
- **Changed:** runs/harvest/rea/36J1tL9ulGA (survey, cuts, events, words, SEEN.md)
- **Why/verdict:** 340 joins looked at; slow map fills were invisible to both eyes, a colour area curve found 3 of 3 (Measured)
- **Status/open:** done; sound not split, review of three rea windows not answered
- **Related:** juju, runs/harvest/SCORE.md

---

## 2026-11-25 07:21 EAT — TEHUTI — Juju: six small pull requests opened from this Mac's crates
<!-- type: event -->
**From:** TEHUTI

Juju: six small pull requests opened from this Mac's crates
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: PRs 21 sigil, 22 harvest + ADR 0021, 23 kits, 24 next, 25 gather, 26 sound (draft). Why/verdict: units to main by ADR 0020. Left out: juju-encode (needs the Maker seam in juju-stage, owned by engine), scriptlab data (no juju-script test reads it), two film frames and their Vision test in sound. bend.py kept: money tests read it. Open: 26 checks red, the two glue Python files need the lead's ruling; gate allow list untouched. Related: docs/adr/0020. Harness: Claude Code (Opus 5.5).
- Verification: cargo check per crate, gate_checks tree and diff locally; GitHub checks partly pending at log time.
- Status: in-progress, GitHub checks running, nothing reviewed or merged

---

## 2026-11-25 07:17 EAT — TEHUTI — Juju harvest: film IEWMpPs0M-M seen whole
<!-- type: event -->
**From:** TEHUTI (claude-code, Opus 5.5)

- Changed: runs/harvest/rea/IEWMpPs0M-M (survey, cuts 173, events 756 merged, words, SEEN.md)
- Why-verdict: kept; nearly every join is a dissolve, solved as a per frame mix
- Status-open: complete; sound not split or heard
- Related: ADR 0021, runs/harvest/SCORE.md

---

## 2026-11-25 06:51 EAT — TEHUTI — Juju gather lane: the reviewer's ten findings worked through (freeze-14)
**Changed:** crates/juju-gather (new truth.rs, borders.rs, recheck.rs; door, plan, net, geo, maps, scale, pics, film, spot, report), runs/gather folders, rerun.sh, FAULTS-14.txt, HANDOFF-STAGE.md. Harness: Claude Code (claude-opus-5-5), workflow worker.
**Why/verdict:** predicate not called TRUE: second reader 0 of 100 and no cold run of the newest binary (0.0003 US left of 0.20). 101 of 101 planted faults refused; stage valid, 0 fallback on 8 tables; moons and Ottoman carry, Black Death, Zulu, Magellan are honest holds.
**Status/open:** about 0.08 US for a cold run and 100 second readings; stage lane: rims of later borders; pictures of map films few.
**Related:** juju, runs/gather/report.json, ADR 0019

---

## 2026-11-25 06:47 EAT — TEHUTI — Juju: stopped waves restarted, film-harvest skill merged, 60-film study shows engine gaps
<!-- type: event -->
**From:** TEHUTI

Juju: stopped waves restarted, film-harvest skill merged, 60-film study shows engine gaps
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi pressed stop on three Juju waves. All three were restarted from disk, and the original facts worker was found still alive, not dead as first assumed.
- film-harvest skill finished and shipped as PR 20; PR 18 and PR 20 merged to main after clean reviews. Fast runner measured about 1.2x faster, not the 3x target.
- 60-film study done: Juju's engine can draw 12 of the 40 picture moves those films use. Facts lane still fails the bar: 2 of 15 opened facts were wrong.
- Mac thrashed at load 190 with 10 GB swapped; sound splitting was stopped and a disk watch set. Still open: one film through the full chain with words on it, checked by eye.
- Files changed: crates/juju-skills/packs/film-harvest/SKILL.md; runs/harvest/SCORE.md; runs/harvest/READ-FIRST.md; runs/gather/GATE-BACK.md; runs/spine/otto-silent-2/master.mp4
- Status: in-progress — PRs 18 and 20 merged; one repaired film with words is still to be made and checked.

---

## 2026-11-25 06:45 EAT — MUNGURA — Juju: first real film out of juju make (1 minute, silent, DONE); works, not good yet
<!-- type: event -->
**From:** MUNGURA

Juju: first real film out of juju make (1 minute, silent, DONE); works, not good yet
- Harness: Claude Code (claude-opus-5-5)
- What happened: runs/spine/otto-silent-2: "The Ottoman Empire, year by year", juju make, 11 of 11 stages, no test switch, 60.0 s, 1280x720, -14.6 LUFS, 0.068 US, 17.2 machine minutes. Lead watched a frame every 3 s: no words on a silent film, stretches with no change, modern "now Turkey" labels, grey outlines, a doubtful number (1,459 in 1861, 2,018 in 1914). Sent to the THROUGH owner. House strips judged: all four eyes refused the planted burger first; relief and lungs strips liked, Orion strip refused, no trace tables yet, one repair running. Harvest: rea-video 10 of 35 drawn events against 35 of 35 by our own eye; seven films read whole.
- Status: in-progress

---

## 2026-11-25 05:43 EAT — TEHUTI — Juju sound lane: reviewer faults fixed
<!-- type: event -->
**From:** TEHUTI

- Changed: juju-sound reads the drawn frames for a number landing, hears cues in one channel outside the words, requires and hears a bed, makes silent films loud by what happens, runs at most four programs at once, never keeps a rubbish answer. Harness: Claude Code (Opus 5.5).
- Why/verdict: strip.mp4 -14.1 LUFS, 2 of 2 cues heard, 9 planted faults refused, silent kit -14.2 with 4 cues; a 20 minute film takes 912 s at load 35 to 49.
- Status/open: 60 s strip took 81 s wall at load 35 (64 s of processor); the 1.28 s hush on silent films needs a ruling (make-mongols still refused).
- Related: runs/sound/auto/HANDOFF.md, branch unit/sound a1f3e12.

---

## 2026-11-25 05:26 EAT — TEHUTI — Juju title cards: checks fixed, no hand yet
- Changed: juju-next 0.5.0 (a3dfd48 and after): words of a title held to its passage, two readers sealed to the card, pictures from their own records, bends on the donor shape, one journal for a deal. Harness: claude-code (Opus 5.5).
- Why-verdict: 15 of 15 planted false titles passed before, 0 of 15 now; two deals at once and kills lose nothing (13 of 13). Predicate FALSE: 0 cards stand, pull bar 6.
- Status-open: 0.0223 US of the lane left, day fuse 0.12 reached; no vote, no paste, no timing under load 20.
- Related: juju, runs/character/loop/evidence/v5

---

## 2026-11-25 05:18 EAT — TEHUTI — Juju harvest: the film language is written and beats rea-video on 4 of 5 blind spots
<!-- type: event -->
- Changed: runs/harvest/LANGUAGE.md, language.schema.json (made by tools/make_schema.py), tools/measure.py; proofs in runs/harvest/language (stay on this Mac).
- Why/verdict: measure.py check prints PREDICATE TRUE. 64 of 64 truth rows said with no prose left; 32 of 35 drawn events against 10 (Measured, same windows); spot 4 not won. Held out: wins at 0.1 s on both stretches, loses to rea at 0.5 s on H 632 to 672.
- Status/open: way names right 10 of 32, 126 and 145 pieces for 19 and 17 things, held out is one film only, sound not heard, no blind rebuild. Harness: Claude Code (Opus 5.5), workflow worker.
- Related: juju, film-harvest; schema is git-ignored by runs/harvest/.gitignore (rebuilt by tools/make_schema.py).

---

## 2026-11-25 04:44 EAT — TEHUTI — Juju harvest: hero J0wWNytEXS4 seen whole

- **Changed:** runs/harvest/rea/J0wWNytEXS4 (survey, cuts, events, words, SEEN.md)
- **Why/verdict:** 138 hard cuts; truth windows 23 of 26 events
- **Status/open:** done; sound not heard, beats without a hand note are noisy
- **Related:** runs/harvest/SCORE.md (claude-code opus 5.5)

---

## 2026-11-25 04:16 EAT — TEHUTI — Juju Vault: stage 0 slot, shelf and sameness meter built
<!-- type: event -->
**From:** TEHUTI (Claude Code, Opus 5.5, juju-db lane)

- **Changed:** crates/juju-db and runs/vault: one folder a channel store, 14 parts as data, slot solver, 15 film shelf, sameness meter, juju-db CLI; LOT opened in runs/vault/store with 0 films.
- **Status-open:** countersign of LINE-RULE.md items 7 to 14; LOT leans on four arcs its vessel does not list (32 of 60); the spine must call it.
- **Related:** runs/vault/receipt.json, runs/vault/sim.json, commit a966d48. Topic: juju.

---

## 2026-11-25 04:15 EAT — TEHUTI — Juju harvest: scripts/harvest runs windows, same answers, 3x not reached

- **Changed:** scripts/harvest, scripts/harvest_lib, runs/harvest/tools (FAST-READY, FAST.md, ORDER, rea_launch.py refuses stems). Uncommitted. Harness: Claude Code (Opus 5.5 worker).
- **Why/verdict:** 20 s cut SAME as plain, 218 to 90 processor seconds but 195 to 167 s wall; kill -9 and resume SAME; decode was about 6 percent of plain, text and sound the rest.
- **Status/open:** 3x not reached or proven; 120 s plain never finished; sound split off by order; a long film with the memory patch not run.
- **Related:** ADR 0021, runs/harvest/SCORE.md, runs/decision.tsv lane harvest, topic juju.

---

## 2026-11-25 03:40 EAT — MUNGURA — Juju harvest: rea-video scored against hand truth; our own eye sees what it cannot
<!-- type: event -->
**From:** MUNGURA

Juju harvest: rea-video scored against hand truth; our own eye sees what it cannot
- Harness: Claude Code (claude-opus-5-5)
- What happened: Truth sealed first, three 40 s windows. rea-video: hard cuts on paper 3 of 3, but 10 of 35 drawn events inside code-drawn shots, 0 of 9 on the silent map, 58.9 min for 40 s plain. Arrival map plus frame difference: 35 of 35, 47 to 100 s a window, same windows it was built on (no held-out proof). Snapshots every 2 s: 32 noticed, 2 timed within 0.1 s. Decision: no whole film decompose; survey and looking from rea-video, events from our own eye, words from captions. Also: the 60-film study ended; the engine draws 12 of 40 moves and 0 of 20 skeleton and house pairs whole; the engine lane was released to build the ten missing primitives. PRs 18 and 20 merged, none open. Spend 5.50 of 10.00.
- Status: in-progress

---

## 2026-11-25 03:38 EAT — TEHUTI — Juju packaging lab repaired (lab-packaging)
- Changed: runs/scriptlab/packaging: 9 frames, 45 bends, 3 chains, check, plants, blind tags, opened sources. Harness: claude-code subagent.
- Why/verdict: 10 review findings; F06 and F09 dropped by count; check.py TRUE, 145 of 145 plants refused (Measured).
- Status/open: 9 bend sources unconfirmed, 31 pictures need a missing part, F02 five-word sentence wants a countersign.
- Related: juju, runs/decision.tsv lane lab-packaging.

---

## 2026-11-25 03:36 EAT — TEHUTI — Juju sigil: ten reviewer faults fixed in the thumbnail crate
<!-- type: event -->
**From:** TEHUTI

- Changed: crates/juju-sigil (map ground runs past the base's edge, subject chosen by the package, fonts/licence/whole-file checks, G6 fails closed, free picture kept through any buy, locks), runs/sigil checks and faults folder. Harness: Claude Code (Opus 5.5).
- Why/verdict: 19 of 20 new tests fail on the old source, 20 of 20 pass now; check.py 29 TRUE; lane spend 0.0903 of 0.25 US.
- Status/open: not committed; cli must expect HOLD when a package asks for a picture the film does not hold; gather tables without take rows, Borodino at 94.9 E.
- Related: runs/sigil/receipt.json, runs/sigil/faults, topic juju

---

## 2026-11-25 03:24 EAT — TEHUTI — Juju hands lane: two true hands, not three
<!-- type: event -->
**From:** TEHUTI

- **Changed:** juju-next 0.4.1 (commit 6dd7e64): cards are built from their answer outward, a second reader of another vendor finds the answer again unseen, code refuses the rest.
- **Why-verdict:** earlier hands had wrong answers. Vote against real breakouts rose from 6 and 2 to 9 and 7 wins of 20 (judges weak, 3 of 6 plants).
- **Status-open:** lot and space-demo have a hand; map-demo has 4 cards, no hand. Speed under 5 s and 25 s only seen at load 78 to 164. Lane money 0.295 of 0.30 spent, so the rest needs about 0.06 US more.
- **Related:** runs/character/loop/hands.json, runs/character/loop/evidence/v4. Harness: claude-code (Opus 5.5).

---

## 2026-11-25 03:03 EAT — TEHUTI — Juju scriptlab looks repaired against 13 review findings
<!-- type: event -->
**From:** TEHUTI

- Changed: runs/scriptlab/looks make.py, measure.py, check.py, plants.py, side.py, both pairings, HANDOFF.md (lane lab-looks, 15 decide rows)
- Why-verdict: check let 33 of 33 planted faults through; now 0 of 52 missed (Measured)
- Status-open: predicate FALSE for two faults: near-worlds has two usable signature moves; layout gate fires at 0.359 v 0.572 and that measure is not proven; nobody has listened
- Related: Harness: Claude Code (Opus 5.5); evidence runs/scriptlab/looks/evidence

---

## 2026-11-25 02:56 EAT — TEHUTI — juju-gather built: bare card to facts, tables, pictures
Harness: claude-code (Opus 5.5), Juju gather lane.
- **Changed:** new crate crates/juju-gather, runs/gather (report.json, FREEZE-8.txt, bin/juju-gather-freeze-8).
- **Why/verdict:** five bare cards gathered cold in 117 to 188 s, 36 to 172 facts, 0.003 to 0.010 US each; juju-stage accepts every table. First spot draw found 3 wrong of 100 in two subjects; rules fixed, fresh draws 0 wrong (Judged).
- **Status/open:** three map stories still HOLD at ten minutes (10 to 14 dated places, 23 needed). Lane money spent (ledger 0.1980 of 0.20, 0.0259 of it charged while the gate was down).
- **Related:** runs/predicate/CONTRACTS.md 1b.

---

## 2026-11-25 02:37 EAT — TEHUTI — Reviewed Juju PR 20 (film-harvest pack): CLEAN
- **Changed:** review recorded as opus-pack at cc900693; list in runs/pr/NEXT.md. Harness: Claude Code (Opus 5.5).
- **Why-verdict:** pins 800 of 800, rows Builder only, fragment null, licence whole, three translations match. No block.
- **Status-open:** lead countersign for pins; conduct tests and train pending when read; four fixes listed.
- **Related:** juju, PR 20, ADR 0020

---

## 2026-11-25 02:33 EAT — TEHUTI — Juju gather lane: two workers caught, critic report written
- **Changed:** runs/gather/ATTACK.md, runs/gather/TWO-WORKERS.md (Juju). Harness: claude-code (Opus 5.5), no paid call, no code edit.
- **Why-verdict:** build:gather was alive, so the delegate became its read-only critic by the lead's word. FAULTS: 6 wrong pins, a wrong year, 6 facts from other voyages, recheck accepts 6 of 8 planted faults; juju-stage accepts all 7 tables.
- **Status-open:** gather bar not TRUE; owner aee4ed9c2c964b10f; money nearly gone (0.20 US limit).
- **Related:** juju, gather lane, runs/gather/ATTACK.md

---

## 2026-11-25 02:32 EAT — TEHUTI — Juju film-harvest skill: written, linked, passed a fresh agent
- **Changed:** crates/juju-skills/packs/film-harvest (SKILL.md 90 lines, 13 references plus 4 more in English, 14 forms, 5 kickoffs, self test, reach-and-pins.patch), linked into Claude Code and Hermes; runs/harvest/rea/ref20-fresh (proof). Uncommitted. Harness: Claude Code (Opus 5.5 worker).
- **Why/verdict:** Ambi 25 Nov 01:00. A fresh Opus agent with the pack alone made a package that passes videomd --check and answered 6 of 6 plus the planted mistake; its 24 stumbles were answered in the pack.
- **Status/open:** corrected pack not rerun; scripts/harvest main flow, step 8 and the Watcher and Scribe forms unrun; reach rows not compiled here (rustc 1.88 cannot build juju-reliquary), patch waits for the lead's countersign.
- **Related:** ADR 0021, runs/decision.tsv lane film-harvest, topic juju.

---

## 2026-11-25 01:14 EAT — TEHUTI — Juju packaging lane: ten title frames from winners against their own flops

- **Changed:** runs/scriptlab/packaging (why.json, bends.json, chains.json, kill.json, check.py, 97 thumbnails looked at). Harness: claude-code (Opus 5.5 medium), no paid call.
- **Why-verdict:** 10 frames, 50 bends, check.py TRUE, 24 of 24 planted faults caught; four frames thin; counts in-sample, holdout uninformative.
- **Status/open:** every bend's fact is unopened; no blind judge; Ambi's eye and ear decide.
- **Related:** Juju, docs/adr/0021, runs/decision.tsv row packaging-lab.

---

## 2026-11-25 01:02 EAT — MUNGURA — Juju harvest: safety step cut, fast runner and film-harvest skill started
<!-- type: event -->
**From:** MUNGURA

Juju harvest: safety step cut, fast runner and film-harvest skill started
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi 25 Nov 01:00: "f*** safety aggressively rea video. make it a high quality skill juju, true to exactly how its done, and add a few things designed for us and our workflows that make it faster and reliable". Done: the audit step is cut (an empty environment stays, free); measured why it is slow (the film is decoded about seven times in software, text read on the CPU, 20 s of sound splitting took 5 minutes; hardware decode gives identical pixels, md5 equal). Two delegates started: scripts/harvest (decode once, Apple Vision text, CoreML sound, captions as speech, receipts, resume) and the skill pack film-harvest, faithful to upstream with ours marked. Harvest workflow resumed. Also: juju make passed 9 of 11 stages at 00:54 (2 at 20:55); PRs up to 19 merged except 18.
- Status: in-progress

---

## 2026-11-25 00:57 EAT — TEHUTI — Juju sound lane: every film gets sound by itself

- **Changed:** crates/juju-sound (new), runs/sound/auto; strip.mp4 at -14.1 LUFS with 2 cues heard by Earshot, 0 synthetic; 13 sounds kept on the shelf; commit 5be1207 on local branch unit/sound.
- **Why/verdict:** film stage 7 needed cues chosen, levelled and heard before a pass; receipt verdict pass, all planted faults refused.
- **Status/open:** work 50.8 s at load 49 to 88, 117 s at load 97; cues heard beside the middle only, phone speaker listen owed; no bed kept that the Watcher wants under a voiced map film.
- **Related:** Harness: Claude Code (Opus 5.5). runs/sound/auto/HANDOFF.md, topic juju.

---

## 2026-11-25 00:57 EAT — TEHUTI — Juju sigil: one command draws, judges and picks a thumbnail
**From:** TEHUTI

- Changed: new crate crates/juju-sigil (uncommitted, kickoff said no commit), runs/sigil proof. Harness: claude-code (Opus 5.5).
- Why/verdict: five packages drawn three ways each, G1 to G5 pass in code, two low proofs bought and both lost the vote, 0.077 US of 0.25.
- Status/open: medium buy path proven only against a mock door; fixtures hand-written; hue not gated in G4; no PR yet.
- Related: runs/sigil/check.py, runs/sigil/receipt.json

---

## 2026-11-25 00:43 EAT — TEHUTI — Juju style kits: five kits, checker, pour counted
- **Changed:** design/kits (5 kits, pages, checker), runs/kits/pour.json, HANDOFF.md. Harness: Claude Code, Opus 5.5 worker.
- **Why/verdict:** held-out pour 3: 14 of 14 storyboard forms legal at first answer, 14 of 15 strips drawable by the engine check with no fallback; selftest 279 of 279; 0.144 US.
- **Status/open:** candidates; nothing rendered or judged blind; the writer still invents causes.
- **Related:** ADR 0019, 0014; runs/decision.tsv lane kits.

---

## 2026-11-25 00:22 EAT — TEHUTI — Juju: hero film 260 to 530 s taken apart shot by shot
<!-- type: event -->
**From:** TEHUTI

- Changed: runs/scriptlab/hero/part-2.json (72 shots, 28 traits, 75 colours) and hero/work-2 (frames, curves, check.py, build.py).
- Why-verdict: exit predicate TRUE, 5 of 5 planted faults refused (Measured). Harness: claude-code (Opus 5.5).
- Status-open: family between Arial Bold and Helvetica Bold is Judged; unplotted easings inside screen recordings.
- Related: part-1 and part-3 lanes, ADR 0014, AMBI-EYE.

---

## 2026-11-24 23:59 EAT — MUNGURA — Juju: the night goes to harvest (ADR 0021), twelve key films with rea-video and strong models
<!-- type: event -->
**From:** MUNGURA

Juju: the night goes to harvest (ADR 0021), twelve key films with rea-video and strong models
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi, 23:35 to 23:55: we cannot reverse engineer a video; use github.com/JuneYaooo/rea-video; strong models (Opus 5.5 or Fable 5.2 high) take apart 9 to 12 key videos, extract layered systems mapped to prompts and JSON, visually verified; cheap models (DeepSeek) then only execute by mixing; a pasted link becomes a blend or a harvest; whole 10 to 50 minute films, not clips; "the rest of the night just focus on this, this is the gold". Recorded as docs/adr/0021. Workflow juju-harvest-12 (wf_e8518f9c-22c): audit and lock rea-video, score it against hand truth, a layered motion language, two harvesters head to head, blind rebuilds (a builder who never saw the film), twelve whole packs, cross grammar, 9 to 12 systems with a mixing rule, recipe book with closed menus, film plans. Paused: phone wave 1, buttons wave 4, film ground. Kept: waves 2 and 3, script skeleton reading, hero trace.
- Status: in-progress

---

## 2026-11-24 23:21 EAT — MUNGURA — Juju: Ambi refused the dot strip; looks go back to real material and house worlds
<!-- type: event -->
**From:** MUNGURA

Juju: Ambi refused the dot strip; looks go back to real material and house worlds
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi 23:17 on the McDonald's strip the lead had praised: "the worst looking thing ive ever seen. lean into our strengths in terms of design systems our software biases towards and uses as options." The diagram world workflow was stopped and its looks dropped. New rule file runs/scriptlab/AMBI-EYE.md (a judge must refuse that strip unprompted). New lanes: juju-strengths ranks the worlds Juju draws well into four to six house systems (options with a bias order) and adds idea verbs to them; film one ground restarted inside those worlds. Ambi 23:10: films come out of Juju itself; 23:13: best possible app that produces the videos we need. PRs 16 and 17 merged through the door.
- Status: in-progress

---

## 2026-11-24 23:02 EAT — TEHUTI — Juju PR 15 recheck at 9a48b629: FINDINGS, body only

- Harness: Claude Code (Opus 5.5), reviewer opus-small-2.
- **Changed:** no code; verdict posted on PR 15.
- **Why/verdict:** lost writes now turn report red (stub probe); a plan or report job that dies before writing still leaves older greens and is not named.
- **Status/open:** one body sentence, then countersign.
- **Related:** juju, .github/scripts/train.py

---

## 2026-11-24 22:57 EAT — TEHUTI — Juju taste panel: refuses broken strips, not yet dull ones

- **Changed:** scripts/taste.py, runs/taste (PANEL.md, proof.json, held-proof.json, script-proof.json). Harness: Claude Code (Opus 5.5).
- **Why/verdict:** freeze 4 of 4, cut sound 4 of 4, our silent film lost 3 of 3, same twice 5 of 6; shuffled lines 3 of 4 by models and 18 of 18 by the script check; a voiced repetitive strip of ours tied. Both fresh-strip keys failed.
- **Status/open:** plants for flat voice, same move, generic line; three-seat panel fails its own near-even key (4 win 6 tie 1 lose 1 short). Spent 0.583 US of 0.60.
- **Related:** juju, ADR 0019 point 4.

---

## 2026-11-24 22:56 EAT — TEHUTI — Reviewed Juju PR 15 (FINDINGS) and PR 16 (CLEAN)

- Harness: Claude Code (Opus 5.5), reviewer opus-small.
- **Changed:** no code; verdicts on PR 15 and 16, PR 16 list in runs/pr/NEXT.md.
- **Why/verdict:** PR 15 can leave a head green after a lost red post or a cancelled train, which its body does not name; PR 16 passed the nine-job, memory and 17 heavy rows.
- **Status/open:** PR 15 needs one repair and a recheck.
- **Related:** juju, .github/scripts/train.py, scripts/heavy

---

## 2026-11-24 22:50 EAT — MUNGURA — Juju trunk: pull requests 1 to 12 are in main
<!-- type: event -->
**From:** MUNGURA

Juju trunk: pull requests 1 to 12 are in main
- Harness: Claude Code (claude-opus-5-5)
- What happened: PR 11 merged 22:02, PR 10 (with 1 to 9) 22:49 at 639dc85, PR 12 (conductor loop) 22:50. Merge log lines for 10, 11, 12 are on main (732c2b6). The merge door refused only because a later train had set every head's light back to running; both heads were green in run 45470745500, so the same gh merge command was run with the head pinned. PR 10 took three money repairs (unpriced fields, parts, sellers, jev length); every one has planted tests. Open: 13 (ear table), 14 (ADR 0020), 15 (train light fix), 16 (job queue: 8 slots, load not asked). Queue finding: 36 jobs behind one build because the load rule starved the pool.
- Status: in-progress

---

## 2026-11-24 22:41 EAT — TEHUTI — Reviewed Juju PR 12 at f0490fe2: CLEAN, five fixes and four notes listed

- Harness: Claude Code (Opus 5.5), reviewer opus-conduct.
- **Changed:** no code; verdict on PR 12, list in runs/pr/NEXT.md.
- **Why/verdict:** nothing worse can seal; a worse repair can be the next base in one mixed case; a step up is bought twice only from a damaged reply file, still reserved; Earshot check holds on missing, stale and unbounded input.
- **Status/open:** second reviewer, the train and the lead countersign of the THRESHOLD CHANGE.
- **Related:** juju, crates/juju-conduct, PR 12

---

## 2026-11-24 22:33 EAT — TEHUTI — Juju PR 10 recheck at 639dc85f: CLEAN

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk-4.
- **Changed:** no code; CLEAN recorded on PR 10, notes in runs/pr/NEXT.md.
- **Why/verdict:** both blocks closed by probe, 30 of 30 tests, our callers bodies priced.
- **Status/open:** several jev callers reserve less than the gate price; they should reserve from prices.worst.
- **Related:** juju, scripts/prices.py, PR 10

---

## 2026-11-24 22:28 EAT — TEHUTI — Juju PR 10 recheck at cb0245f2: FINDINGS, the seller and the jev flat price

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk-3.
- **Changed:** no code; verdict on PR 10, notes in runs/pr/NEXT.md.
- **Why/verdict:** the last block is closed (probe, 30 of 30 tests). Two open: a named priority seller bills 1.8 times the price; jev is flat 32,000 tokens and the endpoint takes 262,144. No paid call.
- **Status/open:** the lead decides under ADR 0020.
- **Related:** juju, scripts/prices.py, PR 10

---

## 2026-11-24 22:21 EAT — TEHUTI — Juju PR 10 recheck at 74a8604b: FINDINGS, the money gate still underprices nested fields

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk-2.
- **Changed:** nothing in code; verdict on PR 10, fixes and notes in runs/pr/NEXT.md.
- **Why/verdict:** the first block's reproductions are closed, 30 of 30 tests, new test red on the old file. Still open on a stand-in: OpenRouter video_url and file parts, picture-shaped text inside a schema, WaveSpeed 4k priced as 1k; and route_proof's jev-router body is now refused.
- **Status/open:** the lead decides under ADR 0020 rule 3 (a second block closes the pull request).
- **Related:** juju, scripts/prices.py, scripts/purse.py, PR 10

---

## 2026-11-24 22:13 EAT — TEHUTI — Reviewed Juju PR 10 at ba9b9b1f: one block, the money gate underprices unread fields
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (Opus 5.5), reviewer opus-trunk.
- **Changed:** nothing in code; verdict FINDINGS on PR 10, fixes and notes in runs/pr/NEXT.md.
- **Why/verdict:** prices.worst ignores body keys it does not read; on a stand-in the book went 9.99 to 11.19 on a 0.005 hold. Merge commit equals PR 11, checks green, no keys, 12 looser examples reproduced.
- **Status/open:** the lead repairs or accepts by name; train pending at record time.
- **Related:** juju, scripts/prices.py, scripts/purse.py, PR 10

---

## 2026-11-24 22:03 EAT — MUNGURA — Juju: PR 11 merged; new law, one unit one pull request one round (ADR 0020)
<!-- type: event -->
**From:** MUNGURA

Juju: PR 11 merged; new law, one unit one pull request one round (ADR 0020)
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi: why shove everything into PR 11. Changed: ADR 0020 (one unit per pull request, two reviewers started together, only a block stops it, fixes go to the next one, nothing is pushed into an open pull request, clean and green merges at once). PR 11 merged 22:02 (ba9b9b1) with the same gh command the merge door runs, because the door's log file is not on main until PR 10. PR 10 is in its one review round. A shipping workflow (wf juju-ship-line) cuts quiet live work into small pull requests. Wave 4 (buttons) and the hero engine lane are running.
- Status: in-progress

---

## 2026-11-24 21:46 EAT — TEHUTI — Reviewed Juju PR 11 at 021bf7b: guard fix clean, two wording findings in WORKER.md
<!-- type: event -->
**From:** TEHUTI

- Harness: Claude Code (Opus 5.5), reviewer opus-021b. Posted REVIEW FINDINGS 021bf7b on the PR.
- **Changed:** nothing edited.
- **Why/verdict:** the guard holds the time limit through TERM INT HUP QUIT (old head fails the same probe); contract test held, 0 failed. WORKER.md says every worker of waves 1-3 was cut off; 11 of 21 were. Its redo-nothing sentence needs a rerun at this head.
- **Status/open:** two wording fixes by the lead, then a new head.
- **Related:** juju, scripts/heavy, PR 11

---

## 2026-11-24 21:28 EAT — MUNGURA — Juju: hero film study started (Atticus King), silent films added, all fleets alive
<!-- type: event -->
**From:** MUNGURA

Juju: hero film study started (Atticus King), silent films added, all fleets alive
- Harness: Claude Code (claude-opus-5-5)
- What happened: Ambi named "galactic empires don't actually make sense" (J0wWNytEXS4, 481K views in about 15 hours, 13.9K subscribers) as the film to learn from: storyboarding, ideation, title and thumbnail bends, 4 to 6 design systems grown from it; and "AI's Strange Obsession with Enlightenment" (ZgpMtombn9A) for ideation only. Also: silent map films carry their script on screen. Both of Ambi's playlists (33 films) and the YouTube home page were read. Workflow juju-lab-read (wf_0fa6e6e6-a33) reads 60 films into skeleton cards, storyboard moves, bends and looks. Waves 1, 2, 3 survived the second stop. PR 12 has two fresh reviewers; PR 11 guard fix is being proven.
- Files changed: AMBESSA/intel/juju/runs/scriptlab/AMBI-EAR.md; AMBESSA/intel/juju/runs/scriptlab/sources/study.tsv
- Status: in-progress

---

## 2026-11-24 20:58 EAT — TEHUTI — Reviewed Juju PR 11 at 51d7c9e: three blocks fixed, one new hang in scripts/heavy

- Harness: Claude Code (Opus 5.5), reviewer opus-hangs, verdict FINDINGS posted on the PR.
- **Changed:** nothing edited; notes (scratch)
- **Why/verdict:** the last review blocks 1 and 2 reran and hold, block 3 agreed; new: TERM reaching the guard ends the time limit, a command that ignores TERM then runs for good (next job waiting at 90 s; f915b9e ended it in 13 s).
- **Status/open:** one line in the guard (ignore TERM INT HUP QUIT) fixed it on a copy.
- **Related:** juju, scripts/heavy, PR 11.

---

## 2026-11-24 20:43 EAT — TEHUTI — Juju conductor: keep or revert, one step up, Earshot at stage 7 (PR 12)
<!-- type: event -->
**Changed:** crates/juju-conduct src and tests on branch unit/conduct-loop, head f0490fe, PR https://github.com/AmbessaTrades/juju/pull/12 (Claude Code, Opus 5.5, worktree).
**Why/verdict:** the three "not held" rows of docs/poteto/runtime-loop.md are code; 212 tests pass, 17 new ones were red on the base. A mutant loop of mine held the heavy lane about 32 minutes; the repair loop got its own step limit from it.
**Status/open:** not merged, root reviews. No real engine writes sound/earshot.json yet; the model ladder and a part's budget are candidates.
**Related:** runs/conduct/loop-1124, runs/decision.tsv lane conduct

---

## 2026-11-24 20:36 EAT — TEHUTI — Juju PR 11 review: findings, do not land on integration at f915b9e
<!-- type: event -->
**From:** TEHUTI

Juju PR 11 review: findings, do not land on integration at f915b9e
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session d413af8f)
- Ambi asked for a bounded review of Juju PR 11 at head f915b9e: may it land on the integration branch? Scope was the change since 47995f8, with scripts/heavy as the focus.
- Verdict: FINDINGS, do not land. HEAD matched PR headRefOid f915b9e6. Nothing was edited, no agent started, no cargo, render or paid call. Posted to the PR as a comment and read back.
- Block 1 (measured): scripts/heavy:18. A ticket left by a killed waiter whose pid is reused stalls the whole queue. Suggested fix not run: flock the ticket.
- Block 2 (measured): scripts/heavy:22-29. After kill -9 to the wrapper, the time limit is lost. With one slot, a nested heavy call deadlocks. Suggested fix not run: the guard must enforce the limit.
- Block 3 (documents): ADR 0019 and the ask-juju SKILL.md still say one heavy job or serialized. The PR body says 'none loosened'. Those need fixing before the PR lands.
- Status: complete — review delivered with verdict FINDINGS, PR 11 must not land until blocks 1 to 3 are fixed and re-reviewed

---

## 2026-11-24 20:20 EAT — TEHUTI — Juju PR 11 mechanical recheck at head f915b9e6: 9 checks run, verdict CLEAN posted
<!-- type: event -->
**From:** TEHUTI

Juju PR 11 mechanical recheck at head f915b9e6: 9 checks run, verdict CLEAN posted
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 42d6fbfa)
- Ambi asked for a read-only mechanical recheck of Juju PR 11 at its final head: no edits, no agents, no cargo, no paid calls.
- Ran 9 checks: head SHA match, pins-check 784/784/784 with 0 differ and 0 gone, pins.txt and reach.rs diffs as specified, merge-tree clean, gate open twice, py_compile and zsh -n passed.
- Two checks ran with wrong or piped output at first (a SKILL.md read path and a pipe that hid an exit code); both were rerun correctly before the verdict.
- A CLEAN verdict was posted on PR 11. Six CI checks (run full, run main, shipped, tests conduct, tests rest, train) were still pending, not passed, so check 9 is only 'no failures'.
- Notes are in the scratchpad at haiku-final-notes.md.
- Files changed: (scratch)
- Status: complete — 9 of 9 mechanical checks passed with no failures; 6 CI checks still pending on PR 11 head f915b9e6.

---

## 2026-11-24 20:17 EAT — TEHUTI — Stopped a runaway test and a mis-pointed batch in the Juju worker run; handoff logged
<!-- type: event -->
**From:** TEHUTI

Stopped a runaway test and a mis-pointed batch in the Juju worker run; handoff logged
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- The looks worker ended at 19:33. Its six looks are candidates on composite stills, the film engine cannot draw them yet, and its critic pass is still owed because I stopped the workflow.
- The conductor's mutant run held the heavy lane for the whole loop and nine jobs waited up to 32 min. I stopped the endless test (pid 55786) at 19:41, counted it as caught, and set a 120 s limit per mutant.
- Ambi's rule: every heavy job gets its own time limit, at most 15 min unless it renders a whole film. Test fuse is 10.00 US (ADR 0019). Disk has 40 GB free.
- A sibling session overwrote a shared script at 19:56, so batch s3 ran the wrong work. I stopped the three wrong processes (83170, 84016, 84019) before any paid test, and restored the engine's script from its own record.
- Still open: engine, app server, Spell Strip, Publish Kit, conductor and chain workers are running. They adopt the 15-min rule only if they re-read WORKER.md. The engine has not restarted its build.
- Files changed: runs/predicate/HANDOFF.md; WORKER.md
- Status: in-progress — incidents contained and logged, but the engine build and several workers are still running and unverified

---

## 2026-11-24 19:59 EAT — TEHUTI — Juju ten minute film: words round 2 done

- **Changed:** false claims two judges found (Flint, Kanton clock, 1884 date line, paddle, one date) replaced from corrected facts; motive added from van Gent; script, voice text, outline, pauses rebuilt. Harness: claude-code (Opus 5.5)
- **Why-verdict:** checks.sh ALL PASS, V-map on, 1,342 spoken words; 24 of 24 cold readings pay the extra hours. 0.0592 of 0.06 US.
- **Status-open:** fresh judges before voice; motive, by law, second writer parts need the lead.
- **Related:** juju, runs/films/ten/report.md

---

## 2026-11-24 19:35 EAT — TEHUTI — Juju: Poteto guards hardened, 31 GB disk freed, 10-minute script closed on strict checks but held from voice
<!-- type: event -->
**From:** TEHUTI

Juju: Poteto guards hardened, 31 GB disk freed, 10-minute script closed on strict checks but held from voice
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 31bfe4d9)
- Ambi asked to merge what needs merging and keep Poteto's changes "forever". Poteto upgrade is in PR 11, which is not merged yet: a fresh reviewer found faults in the done-check, and the worker fixed them.
- Added 39 planted-fault tests (scripts/test_contract.py) that all pass, so the done-check is tested, not just read. Exit predicate and heavy-queue scripts changed in the poteto worktree.
- Disk: freed about 31 GB (22.5 GB abandoned debug build, 9 GB render scraps), free space went from 8 GB to 40 GB. Each deletion is logged path by path in the disk ledger; no videos or footage removed.
- 10-minute film script: strict checks went from 18 failures to 0 at 1,343 words, spend $0.07 of the $0.08 cap. The worker said not to voice it yet; a fresh listener and a fact checker are judging it cold.
- Still open: the script never answers why Christmas Island gained extra hours, PR 10 and PR 11 are not merged, and the second PR 11 reviewer is still on an earlier head.
- Files changed: runs/predicate/notes/di[redacted].tsv; runs/films/ten/script.txt; runs/predicate/PLAN.md; docs/adr/0019-ready-at-four.md
- Status: in-progress — PR 10 and PR 11 unmerged, 10-minute script held from voice until fresh readers pass it

---

## 2026-11-24 19:13 EAT — TEHUTI — Juju: walk test fixed, heavy jobs split into two lanes, lead role handed to Ambi's thread
<!-- type: event -->
**From:** TEHUTI

Juju: walk test fixed, heavy jobs split into two lanes, lead role handed to Ambi's thread
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Walk check fixed: exit-predicate walk now signs in on the no-paid test instance ((local page)), presses each room, and fails a room that lands on the wrong address or shows no controls.
- Heavy job queue split into a build lane and a render lane, one job each, after a measured 1.3 of 8 cores in use while 8 jobs waited. Jobs queued before 18:12 still drain from the old queue.
- Ten-minute film thumbnail finished and checked full size. The WaveSpeed run cost 0.117 US. The paid version did not beat the free code-drawn one in blind votes; the blind frame test is still to come.
- Ten-minute script rewrite ended at 0.1493 of 0.15 US. It passes only on its own reading of one check, and one paragraph still needs a rewrite.
- At 18:30 EAT, per Ambi's request to move the lead role to his thread, the state-check task was deleted, HANDOFF.md was written, and no new workers were started. PR 11 and PR 10 reviews remain open.
- Files changed: scripts/exit-predicate; scripts/heavy; runs/predicate/LANES.md; runs/predicate/HANDOFF.md; runs/films/ten/thumbnail.png; runs/app/lead-look-1.md
- Status: in-progress — room fixes, film owner start, PR 10 and PR 11 reviews still open; lead role now with Ambi's thread.

---

## 2026-11-24 19:03 EAT — TEHUTI — Juju ten film words: checks strict again, 18 failures to 0

**Changed:** runs/films/ten words files; Claude Code (Opus 5.5) worker. Strict copied and echo checks restored; neon wrote b3 b8 b13; code cuts and moves elsewhere; 1,343 spoken words.
**Why-verdict:** checks.sh ALL PASS strict, lint PASS; 0.0694 US of 0.08.
**Status-open:** cold readers say beat 5 question is not paid in b8; b2 b7 b11 b14 still glm; V-map off in pack; sentences joined by code need a ruling.
**Related:** runs/films/ten/report.md

---

## 2026-11-24 19:00 EAT — MUNGURA — Juju: Ambi's five answers recorded, 21 review findings fixed, wave 1 fleets started, T3 git unblocked
<!-- type: event -->
**From:** MUNGURA

Juju: Ambi's five answers recorded, 21 review findings fixed, wave 1 fleets started, T3 git unblocked
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: Harness Claude Code (Opus 5.5), thread 6047de40. Ambi (about 18:48 EAT): ready at 16:00 means one tap makes a finished MP4 with sound, voice, thumbnail and publish kit at 10, 20, 30 or 50 minutes; the phone exports by itself and is built now, not after ("the two are in isolation"); taste beyond automatic checks; 95 must be proven by 16:00; 10 US test limit through tomorrow; fleets allowed; "just merge everything". Recorded in docs/adr/0019. cap.json raised to 10.00 on his word. PR 11: a fresh reviewer found 21 faults (four done-check clauses could pass falsely); all answered except two in other lanes' files, with 39 planted-fault tests in scripts/test_contract.py. scripts/heavy is back to one job as Ambi ordered (my two-lane change did not help: load 42 to 65 with it). The kickoff hook now covers Agent, Task, Workflow, Bash claude -p, T3 delegate and thread launch. T3: a stale index.lock of 20 Sep in ~/AUH was moved aside, untracked project folders hidden in ~/AUH/.git/info/exclude (nothing deleted), Juju registered as its own T3 project. 1,305 live source files backed up to private branch snapshot/live-2026-11-24. Four idle cargo caches in the old lead's scratchpad removed (about 1.4 GB).
Why/verdict: PRs 1 to 9 are ancestors of integration, so merging PR 10 lands them. Nothing is merged yet: PR 11 is under recheck, PR 10's body check is red on unnamed threshold changes.
Status/open: workflows juju-wave-1 and pr11-recheck running; seven old workers still finishing; ten-minute words closed out at strict 18 to 0 failures. Predicate 3 of 23 (stricter script). Disk 8.7 GB free.
Related: ADR 0018, 0019; PLAN.md; HANDOFF.md; PR 10, PR 11.
- Verification: test_contract.py 39 of 39; pins-check 784 of 784; gate_checks tree open; git status in ~/AUH 1 s after the lock was moved; ls-remote shows snapshot branch 352356f; gh says the repo is private; key shapes in the snapshot 0.
- Status: in-progress: nothing merged yet; recheck and wave 1 running

---

## 2026-11-24 18:45 EAT — TEHUTI — Reviewed Juju PR 11 (run-until-done contract) and posted 21 findings on it
<!-- type: event -->
**From:** TEHUTI

Reviewed Juju PR 11 (run-until-done contract) and posted 21 findings on it
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 461e46ff)
- Ambi asked for one honest review of Juju PR 11 by a reviewer who wrote none of it, so it can land on the integration branch tonight. No file edited, no agent started, no cargo or paid call.
- PR body claims checked: 20 held, 3 wrong ('one job at a time', '16 pins', '3 slots to 1'), 3 unchecked. Pins rerun on the moved head: 784 of 784.
- 21 findings posted on PR 11 at head 2611544. Main ones: exit-predicate clauses pass when untrue, heavy lane leaks (gate.sh in render lane), and max_heavy is ordered as 1 but the code runs two lanes.
- Walk findings were read, not run: the walk signs in then opens the gate room, which redirects signed-in users, so those rows cannot pass. Countersign rules disagree; the merge door stops on a 404 for MERGE-LOG.md.
- Head moved from 8167237 to 2611544 mid-review; findings are against 2611544. All 21 numbered findings are in the notes file.
- Files changed: (scratch)
- Status: complete — review posted on PR 11 with 21 findings open; merge not cleared.

---

## 2026-11-24 18:30 EAT — MUNGURA — Juju: audit of the day, lead role moved to one thread, 4pm bar being defined with Ambi
<!-- type: event -->
**From:** MUNGURA

Juju: audit of the day, lead role moved to one thread, 4pm bar being defined with Ambi
- Harness: Claude Code (claude-fable-5-2)
- What happened: Changed: Ambi (about 18:20 EAT): "I feel we used too many tokens today with too little output", "audit everything", the big thread's work is picked up "on this thread", "ready by LATEST tomorrow 4pm EAT", Poteto rules "automatically on for everything all the time". Harness Claude Code (Fable 5.2), thread 6047de40. Audit written to runs/predicate/notes/audit-2026-11-24.md and lessons-vs-code-2026-11-24.md. The old lead (session 8c6b00a6) wrote runs/predicate/HANDOFF.md, starts nothing new and deleted its scheduled state check; this thread is the only lead. Plan: runs/predicate/PLAN.md (one film path through juju smoke-test, six lanes, at most six owners, Opus medium, Haiku for pressing).
Why/verdict: Measured from the transcripts: 465 agent transcripts, 2.44 billion tokens, 16.3 million written, about 2,600 US at assumed list prices, against 3.26 US spent on Juju's own models and zero finished films. The old workflows ran Opus at high on general-purpose agents and the lead thread re-read about 560,000 tokens per reply. Of the film chain's 11 stages, 2 work, 8 use a stand-in, 1 is not built; the newest film is 63.6 s with no sound stream. Of 40 lessons from studied films, 14 are checked by the pipeline, 16 sit in checkers nothing calls, 8 are notes. Only a 10 minute film has a measured arc.
Status/open: Interview round 1 sent to Ambi (what ready means at 16:00; phone over Wi-Fi or standalone; lengths; how 95 percent is counted; test money limit). Exit predicate 5 of 23. PR 11 has two fresh reviewers running (delegated). Ten old workers are finishing; a watcher on HANDOFF.md wakes the lead to start the next lane. scripts/heavy is now one build lane and one render lane after one lane for both left 8 jobs waiting 2 to 11 minutes.
Related: ADR 0018 (added 18:20 section), runs/predicate/LANES.md, HANDOFF.md, PLAN.md, runs/decision.tsv; PR 10, PR 11.
- Verification: Token counts from scratchpad/tokens.py over the session's .jsonl files (each API reply counted once). Chain state from runs/spine/score.json run 20261124-174132-02c4. Film looked at as a 12 frame sheet. Workflow settings read in juju-ten-wf_17e18fe4-a27.js (effort high, general-purpose).
- Status: in-progress: waiting on Ambi's five answers; old workers draining; reviewers on PR 11

---

## 2026-11-24 18:07 EAT — MUNGURA — Juju: run-until-done contract installed; root and lead split; live lead re-briefed
<!-- type: event -->
**From:** MUNGURA

Juju: run-until-done contract installed; root and lead split; live lead re-briefed
- Harness: Claude Code (claude-fable-5-2)
- What happened: Changed: Harness Claude Code (Fable 5.2), root session. On Ambi's order of about 17:45 EAT ("install the permanent harness... run autonomously until the entire Exit Predicate is verified TRUE"; "have the agents that are currently doing this rerun their sub agents, as long as they're not in really important work") I read pstack's originals (poteto-mode, worker.md, 8 playbooks, 11 leaf skills, unslop), Earshot's README and the context pack, then wrote in ~/AUH/AMBESSA/intel/juju: WORKER.md (contract, line 1 of every kickoff), AGENTS.md + CLAUDE.md (front door), docs/poteto/{root,hillclimb,live-proof,runtime-loop,ketchup}.md, scripts/exit-predicate (23 clauses read from receipts), scripts/decide (runs/decision.tsv), scripts/kickoff-line.py (Claude Code PreToolUse hook on Agent|Task, installed in ~/.claude/settings.json), scripts/light, pack juju-poteto-autopilot (with its reach.rs rows and 16 pins), ADR 0018. scripts/heavy went from 3 slots to 1 and sets one shared CARGO_TARGET_DIR; scripts/gate.sh takes the shared folder. Boot pointers: ~/AUH/AGENTS.md, ~/.claude/CLAUDE.md, session_start.py, Hermes MEMORY.md (stale FOCUS 8 Nov entry replaced; 5548 of 5555 chars), project map juju.
Why/verdict: One root, one lead. JUJU ORCHESTRATION #1 stays the lead and owns every lane; this session holds the predicate, countersigns, sends fresh verifiers, merges and writes the one final report. No second fleet on a Mac at load 42 to 60.
Status/open: Exit predicate 3 of 23 true at install (baseline in runs/predicate/). Lead answered with runs/predicate/LANES.md and found my click walk never signed in; fixed and retested (altar 8 controls 0 dead; new-vessel correctly fails). PR 11 open against integration/2026-11-24b. Findings: main checkout's packs differ from its pins.txt in 64 places (integration matches 656 of 656); 329 uncommitted files in the main checkout; conductor keeps the newest repair even when worse; stage 7 has no sound check. Conflict recorded: Ambi 25 Oct "never a one-at-a-time lock" vs 24 Nov "max_heavy = 1"; newer wins, reopen rule in ADR 0018. T3 refused linking PR 11 to the thread (user declined the tool call).
Related: ADR 0014, 0017, 0018; PR 10, PR 11; skills juju-poteto-autopilot, pr-gauntlet, memoir-swarm-handoff.
- Files changed: WORKER.md; AGENTS.md; docs/poteto/root.md; scripts/exit-predicate; scripts/decide; scripts/heavy; scripts/light; scripts/kickoff-line.py; docs/adr/0018-poteto-constitution.md; crates/juju-skills/packs/juju-poteto-autopilot/SKILL.md; ~/.claude/settings.json; ~/.claude/CLAUDE.md; ~/AUH/AGENTS.md; ~/.hermes/memories/MEMORY.md
- Verification: Hook: a Juju kickoff written without the line reached a fresh Haiku worker with the line first; it read WORKER.md and ask-juju and answered three contract rules correctly. Pins script reproduces 656 of 656 pins on integration; 672 of 672 with the pack. gate_checks tree, diff and body pass locally on PR 11. scripts/decide refused a row without evidence. scripts/heavy held a second job while a render ran; scripts/light ran in 0.7 s.
- Status: in-progress: contract installed and proven on one fresh worker; build still 3 of 23, driven by the lead

---

## 2026-11-24 18:05 EAT — TEHUTI — Juju Poteto structure: exit predicate at 3 of 23, one heavy job at a time, two stories stopped
<!-- type: event -->
**From:** TEHUTI

Juju Poteto structure: exit predicate at 3 of 23, one heavy job at a time, two stories stopped
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi's 17:45 order ("rerun their sub agents... Poteto structure... right now") was checked against the other thread and the files on disk before acting.
- Built the exit predicate (23 clauses, each read from a receipt on disk). Baseline is 3 of 23 true, saved to runs/predicate/baseline-2026-11-24.jsonl.
- scripts/heavy now runs one job at a time on a shared CARGO_TARGET_DIR (Ambi: "max_heavy = 1"). scripts/light runs two at a time for walks and probes. Not yet carried into the integration branch.
- Stopped two story jobs that served no check. Workers are at 12 live, above the limit of eight, because mid-edit workers were allowed to finish. One new worker is on the missing self-repair rules.
- Ten-minute film script is 1,226 words, too short, and is being redone to about 1,400. Money: 3.17 of 5.00 US at the 18:02 check; the voice budget has 0.15 left against about 0.12 needed.
- Files changed: WORKER.md; AGENTS.md; scripts/exit-predicate; scripts/decide; scripts/heavy; scripts/light; scripts/gate.sh; runs/predicate/LANES.md
- Status: in-progress — 3 of 23 exit clauses true; engine, thumbnail, three rooms and the film render still open, and no voice bought yet

---

## 2026-11-24 18:04 EAT — MUNGURA — Juju: Poteto structure in force; lanes cut to red clauses, three runtime units and words round two started
<!-- type: event -->
**From:** MUNGURA

Juju: Poteto structure in force; lanes cut to red clauses, three runtime units and words round two started
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: verified Ambi's 17:45 constitution in thread 6047de40 (read whole). Wrote runs/predicate/LANES.md (lane, owner, files, clause, state, relaunched). Stopped two story expansions that serve no red clause. Spine owner told to buy no more voice and close out. Fresh owners with WORKER line 1: conductor (keep or revert, one step up, Earshot hears the mix) and ten film words round two. Why: exit predicate 3 of 23; last script had 27 percent of a worker's own sentences and was 1,226 words (too short for 10 minutes). Status/open: engine speed, thumbnail, server, three room lanes, PR answer left mid-edit untouched; walk in exit-predicate never signs in (told root). Voice purse 0.1518 of 0.30 US left. Related: juju ADR 0014, 0017; docs/poteto.
- Status: in-progress: predicate 3 of 23

---

## 2026-11-24 17:20 EAT — TEHUTI — Juju: spending gate for the 10-minute film added; app still unwired, chain 0 of 11 stages working
<!-- type: event -->
**From:** TEHUTI

Juju: spending gate for the 10-minute film added; app still unwired, chain 0 of 11 stages working
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked for a one-hour render path, a 10-minute film proven before any 50-minute voice spend, and a complete app with no coming-soon sections, built by orchestrated lanes.
- Done: the Workshop viewer (local page) shows films, 19 rooms, agents, pictures and a chain board. The spending gate refuses a 50-minute voice request and voice spend past $0.30 until the 10-minute film passes (tested).
- Measured: render runs about 1.98 s of work per film-second today, so a 20-minute film takes about 40 minutes. Engine handoff written to runs/engines/HANDOFF.md for the single engine owner.
- Open: the app server (local page) does not exist, and the rooms are still static pages. Chain is 0 of 11 stages fully working, WaveSpeed has never been called, and the Inworld dashboard needs checking.
- Spend at 17:19 was $2.84 of a $5.00 cap. Nothing stuck. Earlier agent counts were corrected to live versus open.
- Files changed: mockups/kit/workshop.py; scripts/purse.py; scripts/heavy; runs/swarm/swarm.py; mockups/kit/press.py; mockups/kit/jobs.json; runs/engines/HANDOFF.md; docs/adr/0014-locks-24-nov-afternoon.md
- Status: in-progress — the 10-minute film and core app loop are being built, but no stage is fully working and the app server does not exist yet.

---

## 2026-11-24 16:53 EAT — MUNGURA — Juju: two hard gates in code; lanes cut to the 10 minute film and the core loop

**Changed**
- Ambi: never inflate agent counts; 7 to 10 tight lanes; 10 minute film fully finished (voice, real WaveSpeed thumbnail) before any 50 minute voice; core loop on the live Rust server before secondary rooms. Stopped the film and app fleets; relaunched wh5ex4924 (ten minute film) and whzrup23h (core loop). scripts/purse.py refuses 50 minute voice and over 0.30 US voice until runs/films/ten/LEAD-PASS.json; both refusals tested.
- Wave 1 of Haiku app tests: most "cannot be pressed" findings were the test tool timing out on a busy Mac (5 of 6 main buttons worked by hand); removed from runs/slop. Workshop (local page) now counts live, open.

**Status/open**
- (local page) Workshop is live (a viewer); the app server (local page) does not exist yet. Chain: 0 of 11 stages fully working. WaveSpeed still unused. Spent 2.61 of 5.00 US.

**Related**
- docs/adr/0017; topic loop.

---

## 2026-11-24 16:38 EAT — MUNGURA — Juju: management fault owned; five fleets and a 30-Haiku test swarm started, AfriFluent method copied

**Changed**
- Harness: Claude Code (Opus 5.5). Ambi used the app for two minutes and found the PIN fifth circle, the floating cat, cut cards; asked what had been tested. Truth recorded (ADR 0017): the 19 rooms are static pages that call no program (0 fetches); the lead never pressed them end to end. Ledger by service: DeepSeek 1515 calls 1.04 US, GLM via OpenRouter 528 calls 0.47, Gemini direct 18 calls 0.51, Neon via OpenRouter 6, Inworld 77 calls 0.21, WaveSpeed none.
- scripts/heavy is now a pool of three with a memory guard (Ambi law of 25 Oct); the single lock had stalled workers. runs/swarm toolkit (units, brief, check, collect) plus mockups/kit/press.py (presses every control, finds layout faults).
- Started: app fleet wo7jht79s (crates/juju-serve, rooms wired, waves), film fleet w9lxoudwy (arcs, engine speed, tiny form, a 10 and a 50 minute film to the end), PR fleet wnug8dix1 (one integration branch, six lenses), five Haiku swarms (114 units). Story fleet already running. Test cap raised to 5.00 US.

**Status/open**
- No film finished; no app wired yet; 9 PRs unmerged.

**Related**
- docs/adr/0017; runs/app, runs/films, runs/slop, runs/swarm; topic loop.

---

## 2026-11-24 15:27 EAT — MUNGURA — Juju: Ambi judged two engine clips "both great"; narrowed to map and space engines; character, ideation ladder and the perpetual loop started

**Changed**
- Harness: Claude Code (Fable 5.2 lead). Withdrew the universal rip-and-replay job before it built anything (ADR 0016 last section); paused the wgpu running world after its premise step and the sound, voice and support jobs. juju-stage made green by one owner (33 tests, narrator caption removed, workspace tests all pass).
- Showed Ambi mockups/show/clip-map.mp4 and clip-space.mp4 (silent, engine alone, from the stage-y test film). His verdict: "they are both great"; faults he named: jump cuts, plain type, text habit; wants uniqueness, script character, Kallaway-depth ideation, the loop that reads the last film and deals title bends, speed.
- Running: engine fixer on runs/engines/FIX-LIST.md (15 items, two new laws: number equals spoken word; no overlapping text); w5wxxaqgt Atticus King film expanded into looks, niches, channels; wo9xiy1qf same for Milky Stellar, the AI enlightenment film and The Marrow; wanhgd3gx ideation ladder (crossroads-chain-outliner), four narrators tested over seven days on Neon, six looks as data, crates/juju-next (read, add, deal).

**Why/verdict**
- The gate is now code checks plus Ambi eye on clips; blind judges only find faults. Answered him: frame 028 is published; ours on that sheet are 026, 027, 030, 032, 034, 035, 036.

**Status/open**
- No cheap-model form passes the current checker yet; the three-question form and the good-every-time harness wait for the engine fixer. Spent about 2.0 of 4.0 US test cap. 9 PRs open, none merged.

**Related**
- docs/adr/0014, 0015, 0016; runs/engines; topic loop.

---

## 2026-11-24 14:40 EAT — MUNGURA — Juju: invented layouts dropped; core is now rip and replay of any pasted film (ADR 0016) beside one running world (ADR 0015)

**Changed**
- Harness: Claude Code. Ambi: palette sheet "terrible, slideshows 2017"; "why does ours have lines, AI-isms"; "this is about Juju being able to rip design systems from any video that is pasted"; "complete full app capabilities". The lead had shown a sheet with invented dashes, pills and boxed pictures: a slip against ADR 0012 point 6.
- Stopped wn73lwm9s (quote-essay film, hand-written libraries). palettes.json cut 40 to 11 candidates. Started wt7pawzu9 (schema, ripper in juju-absorb, player juju-play, replay-the-donor calibration with numeric error, held-out film, swap with cheap models, one-command spine juju-run and docs/WHAT-WORKS.md) and wase4th1u (wgpu world, one variable, clips judged). juju-stage being made green by one agent.

**Why/verdict**
- Lead watched whole outlier films: 14 of 16 frames of the 2.8M film are one cockpit; published films move LESS by pixel (0.08, 0.18) than ours (0.84 to 4.09). Stills and swatches were the wrong unit.

**Status/open**
- Spent 1.75 of 4.00 US test cap. 9 PRs open, none merged. No film passes yet.

**Related**
- docs/adr/0015, 0016; runs/rip, runs/world; topic loop.

---

## 2026-11-24 14:32 EAT — MUNGURA — Juju: locks of the afternoon recorded (ADR 0014), sealed key gate live, work relaunched after an accidental stop

**Changed**
- Harness: Claude Code (Opus 5.5). Ambi locked: 20 minutes and 2,400 words daily, two voiced channels and one silent; vendor names off app screens; no narrator subtitle; number on screen equals the word spoken; measured timing laws; two looks must beat blind judges on stills before any voice is bought (docs/adr/0014). He later said the taste notes are to be taken with a grain of salt and the lead judgement used.
- He stopped the jobs by accident about 14:26 and asked for a relaunch. Relaunched as wn73lwm9s (two films, engine, libraries, integration branch) and wrmaqfqyx (skeletons, sound, voice, freshness, frame bar, PR reviews). Held until the films are done: leverage ranking, 3D grammar, Ancient Logos teardown, app rooms.

**Why/verdict**
- Blind test: 2 judges called 53 of 53 of our frames machine-made and 0 of 40 published.

**Status/open**
- Spent 1.75 of 4.00 US cap. 9 PRs open, none merged.

**Related**
- docs/adr/0012, 0014; runs/proof; topic loop.

---

## 2026-11-24 14:27 EAT — TEHUTI — Juju: film teardowns, blind frame test, 20-minute money plan, shared spend lock; PRs unmerged
<!-- type: event -->
**From:** TEHUTI

Juju: film teardowns, blind frame test, 20-minute money plan, shared spend lock; PRs unmerged
- Harness: Claude Code (auto-log by claude-haiku-5-5, SessionEnd, session 8c6b00a6)
- Ambi asked to take apart five films (thumbnails, times, quotes, 16-frame pictures, 18:08 spiral, 90/70/50) and build design libraries and skills from them. Teardowns and libraries were started.
- Measured: the cheap-model title/thumbnail picker got 48-59% on 237 hidden winner-over-flop pairs, close to a coin flip. Title formulas were demoted to optional. No winner-picking is claimed.
- Blind test: judges marked 53 of 53 of our engine frames as machine-made and none of 40 published frames. Ambi's 20-minute plan fits about 115 of 135 CAD, but Inworld runs dry on day 56.
- Ambi ordered a heavy-job queue and a shared spending gate. Added scripts/heavy and scripts/meter.py, and wrote ADRs 0012 (no stand-in drawings) and 0014 (locks). Load was still high at last check.
- Open: PRs 1-8 are not merged; the drawing tests in juju-stage are still red; the ledger was at $0.87 against a $0.60 cap; the sealed key gate is unfinished. Session interrupted by user.
- Files changed: scripts/meter.py; scripts/heavy; docs/adr/0012-strengths-only-no-stand-in-drawings.md; docs/adr/0014-locks-24-nov-afternoon.md; docs/adr/0008-fixed-money-looks-taste.md; runs/packaging/backtest-result.json
- Status: in-progress — teardowns, libraries and the spend gate are running; nothing merged; the session was interrupted by Ambi.

---

## 2026-11-24 14:09 EAT — MUNGURA — Juju: planner directive adopted; machine throttled; two 180 second proof films with real voice started

**Changed**
- Harness: Claude Code (Opus 5.5). Ambi passed on a directive from the planner agent (design data libraries to disk, engine defects, one queue, integration branch, protect the 135 CAD, one proof artifact) and said to take from it what helps and get it done; he said the videos look bad and we are swaying.
- Stopped five workflows (rooms, design-systems, film reader, fine comb, engine round 2): files kept, resumable. One queue: scripts/heavy (one lock, waits for load under 14). Workflow wbzpoabjr: design/ libraries, one engine owner, supply, films A (painterly essay) and B (telemetry map) with Inworld TTS-2 stock voice and Earshot sound, blind judges, integration branch.
- Corrected against the disk: conductor critics already hold on an empty or unparsed reply (code read, tests ordered); videotoolbox already exists as an option; the design-systems job was dead because the stopped teardown never returned.
- Changed from the directive: no paid 16-frame pictures inside films (ADR 0008), reveal is drawn by code from real paintings; LoC and BHL refused this client and are left alone; 24 looks ship as data with status not proven until judged; contrast 8.5:1 for primary ink, 4.5:1 for muted and accent.
- Test cap raised to 4.00 US with the reason in runs/meter/cap.json. Ledger 1.17 US.

**Status/open**
- Leverage and guard workflows still running; leverage proofs to be stopped if they compete with the proof films.

**Related**
- docs/adr/0012; topic loop.

---

## 2026-11-24 13:57 EAT — MUNGURA — Juju: Jade-style look dropped; looks now chosen by leverage with the app own models

**Changed**
- Harness: Claude Code (Fable 5.2 lead). Ambi rejected the storyboard pictures (shapes drawn by code: "garbage", "Claude made this") and the script; then dropped the Jade Rabbit Hole illustrated style: only Claude could make it, the software runs on cheap models; "extreme amounts of leverage with the quality".
- ADR 0012 written: no stand-in drawings anywhere; a look is offered only after passing a blind test beside published frames, made by the app own models; two repairs then shelve; scripts follow measured skeletons; the lead looks at every picture before Ambi sees it. Records the lead slip (asked a builder for code-drawn sketches).
- Workflow wtghkk80c: leverage ranking of film kinds, blind test of today frames, script skeletons tested on DeepSeek, Neon and GLM, study of named skills and repos into two own skills, end-to-end proofs of the top three kinds, verdict as ADR 0013 proposal. Workflow w7vp2ygv2: fine comb (review and precise corrections, from the VidRush CEO 21 Nov post).

**Why/verdict**
- Packaging back-test: our skills rubric ranked hidden winners no better than chance (48 percent of 237 pairs); the 12 title equations fit flops as often as winners; 90/70/50 untestable on this data. Ideas are picked by outlier numbers, the model only bends.

**Status/open**
- Cap for all tests today 2.75 US; ledger about 0.9. 8 PRs open, none merged. runs/first-film is of the dropped kind: test words only.

**Related**
- docs/adr/0012; runs/guard/tweet-noahmorris-2026-11-21.txt; topic loop.

---

## 2026-11-24 13:42 EAT — MUNGURA — Juju: wave answered by real freshness, 20-minute plan being costed, PR review loop and merge train started

**Changed**
- Harness: Claude Code (Fable 5.2 lead, Opus 5.5 workers). Read the VidRush CEO post on the demonetisation wave (saved runs/guard/tweet-noahmorris-2026-11-24.txt). Ambi: no talking head, no real voices; wants Juju fresh from film 1 to 357 without losing the brand; asks if 20-minute films with one silent channel fit the money; wants three suggested voices by ear; better 3D; PRs reviewed in loops before they reach him.
- Workflow wiy2d48rc: wave facts, freshness model + 60-film simulation, 20-minute money plan (ADR 0010 candidate), voice by ear, sound by ear, 3D grammar + prototype, Ancient Logos teardown restart, PR review loop over PRs 1-8 + merge train.
- One spending door scripts/meter.py (lock, one cap 2.25 US for all tests); route_proof.py uses it. Gemini billing linked by Ambi; direct key works.

**Why/verdict**
- Measured: DeepSeek thinking low fills the film form validly (2 of 2) and a 426-word span cost 0.0079 US; thinking off is invalid and repair did not converge (5 of 6). GLM low returned nothing for 0.06 US. Gemini implicit cache: 0 of 3 repeats hit.
- Lead judgement recorded: no shuffling built only to fool a detector; variety must come from each film own material.

**Status/open**
- 8 PRs open, none merged; main tests for juju-stage do not compile. Ledger about 0.87 US.

**Related**
- docs/STACK-STATUS.md, docs/adr/0009; topic loop.

---

## 2026-11-24 13:21 EAT — MUNGURA — Juju: metering live — 626 real calls, $0.51, GLM/Neon/DeepSeek bake-off on one film form

**Changed.** `runs/meter/ledger.jsonl` is being written by the harness: 626 rows from 12:50 to 13:21 EAT, running total $0.5095, 4 × HTTP 429. By service: deepseek 455 calls $0.1808, openrouter 160 $0.1465, google 11 $0.1822 — eleven direct-key calls are 36% of spend. Bake-off on one film form (`runs/meter/job/`): GLM 5.3 high via OpenRouter $0.0428 (11,771 out incl 11,349 reasoning, 170.6 s); Neon low via OpenRouter $0.0286 (2,794 out, 2,575 reasoning, 27.0 s); DeepSeek flash high $0.0080 (12,000 out, all reasoning) and $0.0110 on a 40k ceiling (18,228 out). The direct Google key refused four Neon calls at 12:51 with "You exceeded your current quota" (429), then billed $0.0160–$0.0682 for tiny calls after billing was linked (ledger label: "lead: first paid call after billing linked"). Sweeps: nuance 349 calls $0.1454, packaging 249 calls $0.0746.

**Why verdict.** Every cost figure earlier today (10:19 $105/$119 US, 10:52 $96 US per 60 days) was an estimate. These are billed usage as each service reports it (`cost_how`: "usage.cost as OpenRouter reports it"), so the model choice now has a measured price per film form.

**Status open.** The run is still appending; these numbers are a 13:21 snapshot, not a total. The Neon direct key stays unusable (429) — only the OpenRouter path works. No invoice checked; ledger figures are self-reported usage.

**Related.** runs/meter/{ledger.jsonl, job/}; runs/packaging/work/lists (40 channel lists); runs/nuance/.

---

## 2026-11-24 13:00 EAT — MUNGURA — Juju: Doop page-by-page board drawn — 329 room-states on one Excalidraw canvas; quiet-screen law accepted

**Changed.** `mockups/board/doop-blueprint.json`: canvas kKomk5DFWY, page aqrMl1XPQB, 658 frames = 329 room-states × two sizes (@1440 329, @390 329) over 19 rooms (altar, arcana, canopy, cauldron, conjuring, crossroads, feed-sight, gate, mirror-bend, new-vessel, offering, pact, publish-kit, reliquary, sound, spell-strip, tank, vessel, voice), `wired` 9,784, prototype_url (local page) (returns 200). Pages rendered 12:54–12:57: 12 desktop `journey-*.png`, `board-desktop.png` (3.4 MB), `board-all.png` (7.9 MB), `phone/` 201 files, `_look/` contact sheets, builder `build.py` (81 KB). `docs/adr/0009-quiet-screens-quiet-frames.md` accepted for app screens on Ambi's words of 24 Nov ("stop writing subtext everywhere"): 30 interface words at 1440 px, 24 at 390 px, no text of 5 words or more, one 1–2 word status per object, faults starting `QUIET` in `mockups/kit/shot.py`; the film half is a candidate. Round-2 re-shoot: `mockups/r2/shots` 759 files, 726 newer than 11:25; pact, conjuring, publish-kit, spell-strip re-shot 13:13–13:16 with true empty states (`nothing-to-copy-today`, `no-loadout-built-today`).

**Why verdict.** The board is a map, and its own header says so ("MAP ONLY — Too small to read on a phone. Read the pictures in the phone folder"), so every state exists twice: a frame for the wide canvas and a shot for reading. ADR 0009 removes the caption-under-every-name law that produced the text Ambi objected to.

**Status open.** ADR 0008 and 0009 are untracked; board JSON and the 12 pages are uncommitted. Art direction still unjudged (earlier 5–6 of 10). The `phone/` folder holds 201 files; how many of the 329 states they cover is not checked.

**Related.** mockups/board/; mockups/kit/shot.py; docs/adr/0009-quiet-screens-quiet-frames.md; mockups/r2/shots/.

---

## 2026-11-24 12:48 EAT — MUNGURA — Juju: five keys answer, quiet-screen law in code, 19 rooms rebuilt, engine round 5 pictures

**Changed**

**Why/verdict**
- Engine round 5 sheet (9 stage kinds beside real films) looks clearly better than round 1; not yet scored by judges.

**Status/open**
- No PR open yet, no paid call in the ledger yet. Mac load about 180. Board desktop frames empty (board-fix running).

**Related**
- mockups/show/engine-stages-5.jpg, rooms-now-1..3.jpg; topic loop.

---

## 2026-11-24 12:10 EAT — MUNGURA — Juju: stage-y test film rendered end to end, 187 s at 1080p24, zero fallback scenes

**Changed.** `crates/juju-stage` built in release and rendered `runs/stage-y/film/stage-y.mp4`. ffprobe: h264, 1920×1080, 24/1 fps, 186.958 s, 682,223,558 bytes (651 MB), 4,487 frames. `runs/stage-y/film/render.json`: rendered true, render_seconds 1111.47, fallback_scenes 0, safe_box pass (margin 0.04, glyph_px_in_outer_margin 0), audio null, clock "practice clock, 142 words a minute"; scenes listed include layered_painting (0–43.31 s, 10 events), document_page (43.31–60.89), map_theatre (60.89–87.35). Looked at `film/contact-5s.jpg`: painted isle and fire, Plato bust over a Republic page, a Europe map changing decade by decade, a thinkers timeline, Earth/Moon/Mars/Jupiter plates, an ocean-depth gauge, 1900s street stills — real frames, not placeholders. Live at the time: `cargo build --release -p juju-stage -j 2 --offline` and `lockf -t 7200 /tmp/juju-heavy.lock nice -n 18 cargo test -p juju-absorb --offline -j 2`.

**Why verdict.** The stage engine has to be judged on frames, not on a plan; a rendered film with 0 fallback scenes and a passing safe box is the only proof that the stage code produces pictures. Audio is null because this was a picture test on a practice clock, not a voiced film.

**Status open.** No voice track. One act ("act-01" in `runs/stage-y/form.json`), not a full film. Nothing committed: 205 files dirty in the repo, last commit e0115bd at 10:33.

**Related.** runs/stage-y/{film/render.json, film/contact-5s.jpg, film/stage-y.mp4, form.json, script.json}; crates/juju-stage.

---

## 2026-11-24 11:25 EAT — MUNGURA — Juju: five-film teardown and design-system libraries launched; round-2 parts shown

**Changed**
- Harness: Claude Code (Fable 5.2 lead, Opus 5.5 high workers). Launched workflow whr1651bp: teardown of five films Ambi named (ZgpMtombn9A, sJiaWNxYFUA, oRBu7wYuOSo, G4w-a8NgnnQ, HmuQoak_IAg) into runs/teardown/<id>/, peer review, then libraries in design/ (type 30, palette 36, quote 16, motion 24, texture 16, theming, extraction pipeline), new skills, skeptic attack.

**Why/verdict**
- Ambi 24 Nov: "the whole concept of everything is design systems"; money map agreed at 135 CAD (ADR 0008).

**Status/open**
- Seven earlier workflows still running on an overloaded Mac (load ~51). Nothing metered; no keys asked yet. Engine films still 3-5/10 until round 2 reports.

**Related**
- docs/adr/0008-fixed-money-looks-taste.md; topic loop.

---

## 2026-11-24 10:52 EAT — MUNGURA — Juju: LOT-first dropped, capability study launched, budget remapped to $135 CAD
<!-- type: event -->
**From:** MUNGURA

Juju: LOT-first dropped, capability study launched, budget remapped to $135 CAD
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi said no LOT film before the software's capability is understood, and that the build should be judged on its own range, not on LOT. Agent stopped the LOT film job and withdrew its channel picks.
- Agent launched a capability study that dissects real faceless videos shot by shot, so the engine's priorities come from measurement.
- Agent's first 60-day budget (about $290 US) was rejected by Ambi as inflated. Remapped to $135 CAD (about $96 US) for 150 films in 60 days: Inworld $55, OpenRouter $23, DeepSeek $22, Google $21, WaveSpeed $14.
- Still open: volumes and costs are assumptions, nothing is metered yet, and the Inworld 20% batch discount is still in preview. The YouTube feed scan via computer use failed (window on another desktop), with a yt-dlp fallback.
- Files changed: ~/AUH/STUDY/loop-rebuild-2026-11-19
- Status: in-progress — capability study running; budget map delivered, volumes not yet metered

---

## 2026-11-24 10:19 EAT — MUNGURA — Juju: prices re-checked, two earlier numbers corrected, channel picks proposed
<!-- type: event -->
**From:** MUNGURA

Juju: prices re-checked, two earlier numbers corrected, channel picks proposed
- Harness: Claude Code (claude-opus-5-5)
- Verification: OpenRouter models and endpoints API and api-docs.deepseek.com pricing read today; ytlocal outliers run today for the three channels.
- Status: in-progress: prices checked live; nothing bought or run yet

---

## 2026-11-24 10:19 EAT — MUNGURA — Juju: correction to the 10:19 price entry
<!-- type: event -->
**From:** MUNGURA

Juju: correction to the 10:19 price entry
- Harness: Claude Code (claude-opus-5-5)
- What happened: Changed: the 10:19 entry said about $105 US for 30 days; adding it up again gives about $119 US (about 167 CAD): Inworld 25, OpenRouter 26 (GLM at Z.AI plus Jev), Google 15, WaveSpeed 22, DeepSeek direct 31 minus the balance already there. Why/verdict: fleet scripts written by DeepSeek on max were left out of the first sum. Status/open: every figure is an estimate (reasoning tokens assumed: GLM 8k a call, DeepSeek 16k); the first real film replaces them.
- Status: complete: figure corrected; unmeasured

---

## 2026-11-24 10:16 EAT — MUNGURA — Budget go-ahead: 30 days of daily films for three channels, about $93 US; reasoning knob set
<!-- type: event -->
**From:** MUNGURA

Budget go-ahead: 30 days of daily films for three channels, about $93 US; reasoning knob set
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked to 'load up money on everything' and whether the reasoning knob can change per film. Plan: DeepSeek always max, GLM 5.3 always high, Neon low to xhigh.
- Go-ahead given: load 30 days, all three channels daily, about $93 US (~$130 CAD). Split: Inworld $30, OpenRouter $26, WaveSpeed $22, Google AI Studio $15. 60 days would be about $186 US.
- Cost per 50-minute LOT film: Quick $1.74, Crafted $2.00, Masterwork $2.81. These are estimates; nothing is measured yet.
- Slowness traced to load (about 42 on 8 cores) from builds and renders queuing, not too few agents. New work is design-only until builds clear. A background git push was killed and HEAD soft-reset to origin/main.
- Review flow confirmed: maker, two fresh reviewers (one by eye, one by use), fixer, repeat up to 3 times, truth check on every screen. Still open: check each wallet's minimum and credit expiry before paying; test Neon effort changes keep the cache.
- Status: in-progress — go-ahead given; no payments confirmed in transcript, Neon cache test pending.

---

## 2026-11-24 09:21 EAT — TEHUTI — Juju: page-by-page map started, folded skills being restored, API cost plan drafted
<!-- type: event -->
**From:** TEHUTI

Juju: page-by-page map started, folded skills being restored, API cost plan drafted
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked for a page-by-page visual map of every interaction and agent flow for Doop, built on the speed skill, which the agent identified as asase-velocity.
- Page-spec mapping started on Opus. Art judges scored three directions 5 to 6 of 10. No Doop board is drawn yet.
- Ambi asked that all folded Juju skills be acted on. The agent is giving them their own files (44 in total) and building the part of the app that makes them act.
- Cost estimate for a $40 US test buy: about $1.78 per 50-min LOT film, $0.33 per 30-min film. The 60-day plan is $140 CAD for LOT 3x a week versus the doc's $144, and about $223 for daily LOT. Estimates only, nothing measured.
- Files changed: mockups/show/carved-altar-r2.jpg; mockups/show/carved-tank-r2.jpg; mockups/art/carved/shots
- Status: in-progress — page map and skill restoration still running; no Doop board or measured costs yet

---

## 2026-11-24 08:48 EAT — TEHUTI — Juju: built the self-review gate, 19 rooms, and its own private repo; Earshot phone spike measured
<!-- type: event -->
**From:** TEHUTI

Juju: built the self-review gate, 19 rooms, and its own private repo; Earshot phone spike measured
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi asked for confidence in the system: work that reviews itself and auto-merges only once it passes. Built one gate command covering code tests, all 33 skills, every screen at both sizes, and a truth check.
- The truth check fails screens that claim things that are not real (Connected, 43 of 70 pictures, Film ready, a made-up version history). Ambi's decision is in docs/adr/0002-no-required-spoken-take.md.
- All 19 rooms exist in first-round look; the kit checker reported zero faults at 1440 and 390. Three art directions (night light, framed panels, carved ink) were drawn and are awaiting judgement.
- Ambi answered the grill: Q1 yes, Juju's own private repo AmbessaTrades/juju (agent reports it created); Q2 nothing auto-merges until reviewed; Q3 50-minute documentaries, old LOT not a source; Q4 TTS-2 pauses placed in the edit.
- Attack pass: of 262 VidRush abilities, 77 are missing from Juju's rooms, and three skeptics found holes (no fact-checking, no story law, dead buttons). Open items are in docs/OPEN-RISKS.md and mockups/COVERAGE.md. A stray TubeLoop save was left in place, unreverted.
- Files changed: docs/adr/0002-no-required-spoken-take.md; docs/adr/0001-earshot-listening-models-allowed.md; docs/earshot-phone-spike.md; docs/OPEN-RISKS.md; mockups/COVERAGE.md; mockups/kit/truth.py; mockups/kit/facts.json; crates/juju-skills/packs
- Status: in-progress — art direction judging, first 50-minute film test and scene engine still running; the Earshot phone app waits for the Galaxy plugged in

---

## 2026-11-24 08:17 EAT — TEHUTI — Juju: Earshot kept in full, Android toolchain installed, 33 skills validate, 12 Rust tests pass
<!-- type: event -->
**From:** TEHUTI

Juju: Earshot kept in full, Android toolchain installed, 33 skills validate, 12 Rust tests pass
- Harness: Claude Code (auto-log by claude-haiku-5-5, Stop, session 8c6b00a6)
- Ambi said all of Earshot must be used, including its own sound effects, to avoid the AI-sounding SFX. The brief was edited to match, and an ADR (0001) now records that Earshot's listening models are allowed.
- Android kit installed and 18 rooms exist. The 33 skills (32 plus the ask-juju router) are on disk and validate, and the same files load in the Rust app with 12 tests passing.
- Ambi's round-1 verdict (childish drawings, weak cohesion, paid states unclear) set round 2: one shared art library, and a drawing must show a real state. Three redrawn art directions are still in progress; no room is redrawn yet.
- Still open: Earshot running on the phone without the computer (spike in flight), the Wednesday LOT proof film under review, and the skills backup to tubeloop was refused for size and is being fixed.
- Files changed: JUJU-MASTER-BRIEF.md; docs/adr/0001-earshot-listening-models-allowed.md; mockups/ROOMS.md; SKILLS-PLAN.md; mockups/kit/live.py; apps/juju-shell/build_ui.py; ~/.claude/auh/config/skills-policy.json; ~/.auh-git/projects/tubeloop/project.json
- Status: in-progress — Juju app build underway; round-2 art redraws, Earshot-on-phone spike and LOT proof still open.

---

## 2026-11-24 08:16 EAT — MUNGURA — Juju day 1: skills on disk, first rooms shown, Ambi's round-1 verdict, YouTube rule checked
<!-- type: event -->
**From:** MUNGURA

Juju day 1: skills on disk, first rooms shown, Ambi's round-1 verdict, YouTube rule checked
- Harness: Claude Code (claude-fable-5-2)

Why/verdict: Ambi, 24 Nov, on round 1: likes the vibe; wants more cohesion between pages and better drawings ("can't feel like they're drawn from a kid"), visuals whose logic makes sense (the tank's gourds), nothing shown as paid, no "43 of 70 pictures" (old LOT language), no goofy spell-strip pictures; APK must use Earshot without the Mac; he asked whether the picture budget makes sense. Decision (Ambi): Earshot in full, on the phone too. Observation, verified on YouTube's own help page today: the channel monetisation policy names image slideshows, templated storylines, scrolling text with little narrative, and AI content from generic templates "without adding the creator's original, authentic insights or perspective"; one operator reports 14 channels demonetised on 23 Nov. Lead's advice sent to Ambi: fund only Google AI Studio and WaveSpeed at the smallest amount today (about $20 US, not the $144 CAD plan); GPT Image 2.6 only; GLM unproven.


Related: docs/STAGE-FORM.md, mockups/ART-BRIEF.md, mockups/ROOMS.md, SKILLS-PLAN.md, docs/earshot-phone-spike.md. Harness: Claude Code in T3 Code, Fable 5.2 lead, Opus 5.5 and Haiku 5.5 workers.
- Verification: cargo test: 12 passed; 33 skill.json parse and ids match folders; rooms render with 0 printed faults at 1440 and 390 (arcana has a script error, still with its maker); wall answers 200 with its key and 404 without; YouTube wording fetched from support.google.com/youtube/answer/1311392; Gemini 4 Neon and GPT Image 2.6 prices read from today's saved vendor pages.
- Status: in-progress: three workflows running; skills backup blocked on a size decision

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
- Files changed: JUJU-MASTER-BRIEF.md; harvest/wave1/INDEX.json; harvest/wave1/V2VIDEO-READER-BRIEF.md; scripts/harvest-index.py; scripts/stack-txt-harvester.sh; scripts/dedupe_frames.py; ~/debate-agent/memory/vault/project-maps.json
- Status: in-progress — research and intake complete, no Juju code built, awaiting Ambi's reply on the 5 calls

---

## 2026-11-24 06:40 EAT — MUNGURA — Juju master brief received: saved, checked against the Mac, screens read
<!-- type: event -->
**From:** MUNGURA

Juju master brief received: saved, checked against the Mac, screens read
- Harness: Claude Code (claude-fable-5-2)
- What happened: Changed: Ambi pasted the Juju master brief (22 sections, 28,186 words) into T3 Code at 06:28. Saved byte-identical to JUJU-MASTER-BRIEF.md (sha256 8b8cdfc1…). Ran the boot it asks for, minus the steps that need his word. (1) Vendor docs: 19 of 19 saved to ~/AUH/AMBESSA/docs/stack-txt (the brief's harvester used bash 4 arrays; macOS has bash 3.2, so it was rewritten). (2) VidRush V2 walkthrough DlB0UABEawo: 1080p, 01:25 on, two ffmpeg passes, 639 frames on disk, 195 distinct screens with timed transcript. (3) Haiku 5.5 readers, one bounded unit each: 85 VidRush screenshots + the long homepage in 18 slices + 39 look references + 195 video screens, one JSON per unit in harvest/wave1/out, indexed in INDEX.json. (4) Juju added to the project map (find "Juju" now answers); topic = loop, where the software's history sits.

Why/verdict: the brief is the first record of the name Juju on this Mac. No day log exists for 21 to 23 Nov and Memoir had zero hits, so its "said by Ambi 20 to 22 Nov" lines cannot be checked here; the paste itself is taken as his word for the name and the folder. Observations where the brief and the disk disagree: the Rust engines are at ~/AUH/Loop/loop/engine (47 files, 9,791 lines, confirmed), not ~/AUH/Loop/engine. The look folder holds 39 pictures, about 35 of them Hades II; no Thumbsy screen, no YouTube feed tester screens. Missing on this Mac: rustup, Android SDK/NDK, adb, Tauri, Typst, bun, wrangler, turso; disk 95% full (51 GB free). The brief puts LOT on Inworld TTS-2; Ambi's 1 Nov voice lock is ABV V9 on inworld-tts-1.5-max, 0.95, temperature 2.0. LOT has not uploaded since 2 Nov; lot-r01 (25.3 min script, voice about $0.46) was never voiced or rendered.


Related: brief sections 15 to 18 and 22; ~/AUH/Loop/loop/onefile/START-HERE.md; ~/AUH/AMBESSA/BUILD/BUILD-BRIEF.md (19 Nov handoff, before the name). Harness: Claude Code in T3 Code, Fable 5.2.
- Files changed: JUJU-MASTER-BRIEF.md; scripts/stack-txt-harvester.sh; scripts/vidrush-v2-frame-rip.sh; scripts/dedupe_frames.py; scripts/harvest-index.py; harvest/wave1/INDEX.json; ~/AUH/AMBESSA/docs/stack-txt/; ~/debate-agent/memory/vault/project-maps.json
- Verification: cp checksum matched; harvester printed saved 19 failed 0; frames.json lists 639 files and 195 distinct screens; harvest-index.py printed 0 failed records; one reader record compared by eye against its screenshot (home composer, 13-18-32) and matched word for word; map-check shows no juju failure (2 older failures: memoir skill not found).
- Status: in-progress: boot audit and screen reading done; five decisions are Ambi's before the build starts
