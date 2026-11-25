<!-- copied from the Juju repo: runs/app/BUTTONS.md, last changed 19:48 EAT, 24 Nov 2026. Private lines removed. Do not edit here. -->
# Buttons: every control, and the units that fix them

> Working document. Subject to change through continued conversation. 24 Nov 2026, about 20:00 EAT. Each control, its state, decision, unit and proof: `BUTTONS.json`.

**Counts (measured).** 573 rows: 545 from the census (its text reached this job cut short; all 19 rooms were recovered from the run's journal), 16 controls it missed, 7 rows for what the kit builds in every room, 5 controls that do not exist yet. 303 rows pressed, called or read by the writer, every *does nothing* and *endpoint missing* row among them.
States: sample 160, dead 131, view 113, real 112, missing 43, display 5, absent 5, misleads 4. Decisions: remove 378, keep 98, wire 79, build 18. Soon marks: 0 of 2.
Census corrections: 47 not checked, now settled; 104 real that only change their own page; 15 wrong otherwise. 23 controls say they saved or did a thing and do not (worst: the Tank's *Locked. Nothing can spend.*).

## What is true

1. The eight core rooms work: one dead control (Back on the Pact after a card). But every road ends at the same practice minute: the card, the idea and the length shape nothing.
2. The other eleven rooms make 0 calls to a server between them, and the server sends all of them to the Altar. A person cannot reach them today.
3. The one tap path lacks five controls: a door to paste a link, Deal again, Voice or silent, Save film, a door to Mirror Bend.
4. Prices and waits on the Pact are constants in cards.rs. Lengths are 10 and 20 only; 30 and 50 wait for the arc checker and a render that fits 90 minutes (ADR 0014.14, 0019.3).
5. **Which copy to edit:** the main checkout on disk. mockups/r2 and crates/juju-serve are untracked on main; the same bytes are on unit/phone and snapshot/live-2026-11-24. integration/2026-11-24b has no juju-serve and older core rooms, so merging it does not bring the live app to main.

## Room by room

| Room | Controls | Real | Screen only | Broken | Keep | Wire | Build | Remove |
|---|---|---|---|---|---|---|---|---|
| gate | 8 | 7 | 1 | 0 | 8 | 0 | 0 | 0 |
| altar | 14 | 9 | 1 | 4 | 9 | 4 | 1 | 0 |
| crossroads | 11 | 10 | 0 | 1 | 9 | 1 | 1 | 0 |
| cauldron | 8 | 8 | 0 | 0 | 6 | 2 | 0 | 0 |
| pact | 14 | 6 | 1 | 7 | 5 | 7 | 2 | 0 |
| conjuring | 8 | 8 | 0 | 0 | 7 | 1 | 0 | 0 |
| spell-strip | 18 | 18 | 0 | 0 | 18 | 0 | 0 | 0 |
| publish-kit | 26 | 23 | 1 | 2 | 22 | 2 | 2 | 0 |
| new-vessel | 35 | 0 | 8 | 27 | 2 | 4 | 4 | 25 |
| feed-sight | 23 | 1 | 2 | 20 | 0 | 21 | 2 | 0 |
| mirror-bend | 41 | 1 | 10 | 30 | 5 | 25 | 4 | 7 |
| tank | 42 | 2 | 9 | 31 | 2 | 11 | 2 | 27 |
| vessel | 69 | 3 | 4 | 62 | 0 | 0 | 0 | 69 |
| canopy | 39 | 3 | 14 | 22 | 0 | 0 | 0 | 39 |
| offering | 37 | 2 | 14 | 21 | 0 | 0 | 0 | 37 |
| reliquary | 35 | 1 | 6 | 28 | 0 | 0 | 0 | 35 |
| arcana | 34 | 4 | 18 | 12 | 0 | 0 | 0 | 34 |
| sound | 51 | 1 | 11 | 39 | 0 | 0 | 0 | 51 |
| voice | 53 | 0 | 17 | 36 | 0 | 0 | 0 | 53 |
| kit | 7 | 5 | 1 | 1 | 5 | 1 | 0 | 1 |

## Units, in order. No file is in two units.

Server units start after S1 lands its stubs. The four opened rooms are served on test at once and on 4700 only when their unit passes. Room units of the same step can run side by side. Exits are in BUTTONS.json.

| # | Unit | Files | Controls | To fix | After |
|---|---|---|---|---|---|
| 1 | S1-door | routes.rs, lib.rs, api.json, API.md, prove.py, ROUTES-PROVED.md, rooms-open.json | serves 14 |  |  |
| 2 | K1-kit | kit2.js, api.js | 42 | 14 | S1-door |
| 3 | S2-cards | cards.rs | serves 12 |  | S1-door |
| 4 | S3-donors | donors.rs | serves 22 |  | S1-door |
| 5 | S4-real | engine.rs, work.rs, real.rs, film.rs | serves 3 |  | S1-door, S2-cards |
| 6 | S5-paint | paint.rs, kit.rs, paint.py | serves 19 |  | S1-door |
| 7 | R1-gate | gate.html | 8 |  |  |
| 8 | R2-altar | altar.html | 7 | 4 | S1-door, S2-cards |
| 9 | R3-new-vessel | new-vessel.html | 33 | 31 | S1-door, S3-donors, K1-kit |
| 10 | R4-crossroads | crossroads.html | 9 | 3 | S1-door, S2-cards |
| 11 | R5-cauldron | cauldron.html | 6 | 2 | S2-cards |
| 12 | R6-pact | pact.html | 11 | 8 | S2-cards, S4-real |
| 13 | R7-conjuring | conjuring.html | 6 | 1 | S4-real |
| 14 | R8-spell-strip | spell-strip.html | 16 |  | S4-real |
| 15 | R9-publish-kit | publish-kit.html | 19 | 3 | S5-paint, S1-door |
| 16 | R10-feed-sight | feed-sight.html | 19 | 19 | S1-door, S3-donors, S5-paint, K1-kit |
| 17 | R11-mirror-bend | mirror-bend.html | 38 | 33 | S1-door, S3-donors, S5-paint, K1-kit |
| 18 | S6-money | money.rs, ledger.rs | serves 11 |  | S1-door |
| 19 | R12-tank | tank.html | 40 | 38 | S1-door, S6-money, K1-kit |
| 20 | R13-cut | the seven cut rooms, kit-sheet.html | 319 | 319 | K1-kit, R3-new-vessel, R10-feed-sight, R11-mirror-bend, R12-tank |

## Proof rules
- Press the selector over http at 1440 and 390, reload, and read the saved value back (a GET or the page). A toast is not proof. Removed: the selector counts 0.
- `press.py` is not enough: it presses the first 40 controls only and counts a fake toast as alive; `live.py press` on a hidden room follows the redirect and presses the Altar.
- Paid arms (real, paint, deal) answer 403 locked on 4701. The lead makes the one real press of each, on 4700, with a reservation.

## Open
- **Cutting seven rooms** (vessel, canopy, offering, reliquary, arcana, sound, voice) is this job reading ADR 0014.16, not a word of Ambi. WIRING.md of this morning cut or folded five of them and kept vessel and arcana; it also cut mirror-bend and feed-sight, which stay here because a thumbnail is now asked for (ADR 0019.1). Nearest to real if wanted: voice (196 voices, samples on disk), arcana (six looks; no look reaches the engine).
- **S4 waits on crates/juju-cli** (phone lane B owns it): `juju make` has no --card and no --idea, and its thumbnail, mix and review are stand-ins.
- The Pact's Missing list (2 today) names engine parts that do not run; it is not counted as a Soon mark. New vessel opens as a link reader for Library of Tehuti: nothing can make a film for a second channel, so naming one would be a dead control. Its name on the screen is open.
- The phone app must answer the new routes too (juju-phone api). The Mac shell app still opens the old passB pages. A saved master is 264 MB a minute, so a phone may need watch.mp4.
