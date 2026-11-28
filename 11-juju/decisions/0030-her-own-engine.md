# ADR 0030: she has her own engine; one engine runs everywhere

Working document, changes with conversation. Nothing here is a requirement until Ambi says so.

## Said by Ambi, 28 Nov 2026 about 16:30 EAT (answer to "should the Mac make every film?")

2. This restates ADR 0019 item 2 (24 Nov: "an Android app that draws and encodes the film on the phone, with the Mac off") and PHONE-CORE (26 Nov: "the app is supposed to work without my computer AT ALL").

## What went wrong (audit, 28 Nov, Measured: `~/AUH/AUDIT-REPORT-2026-11-28.md`)

PHONE-CORE already planned **one** engine: "on the Mac: the same crate, so a film on the phone matches a film on the Mac". In practice the Mac kept its Python chain (`juju-maps/`) and new film kinds were built there first. The phone engine (`crates/juju-core`, 3,630 lines) was left with two kinds. The idea screen deals from the Mac's list, so the phone is offered films it cannot make.

## Lead's design, *candidate* until Ambi accepts it

1. **One engine.** `crates/juju-core` is the only engine the app calls, on the phone, on his phone and on the Mac. The Mac's server calls the same crate.
2. **A kind exists when the engine has it.** A film kind, format or look reaches a screen only when juju-core makes it. The can-list (one data file) is read by the idea dealer, the confirm sheet and the engine, so nothing undeliverable is dealt.
3. **The Python chain becomes the lab.** `juju-maps/` keeps prototyping new looks and formats at 240p. Nothing in it is called by the app. A lab result reaches the app by becoming data the engine reads (a format file, a design system file) or by a port into the engine.
4. **Formats are data, so the engine stays small.** A new niche should be a new format file, not new engine code (see `docs/PLAN-0.5.md`).
5. **the phone is her kitchen.** The web orders to the phone that owns the channel (today's design). Her films, ideas and spend are hers in the Door.

## Open

- Whether the 3D globe looks (Duppy Night and Day, drawn by Cesium in a hidden browser on the Mac) must also run on the phone, or stay Mac-only until the Rust drawer can draw them.
