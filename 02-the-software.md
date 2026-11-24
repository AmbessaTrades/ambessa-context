# 02 — The software: Juju

State at 13:30 EAT, 24 November 2026. Live numbers: [10-now/status.json](10-now/status.json).

## What it must do

Ambi, 24 Nov: "If I put any video in there, a faceless video, it will know exactly how to strip it down, wire it up, and make
our own version of it in every way." The aim he named: 52 minute, TV-style films that a sixty year old watches on the couch, and then
**the Offering**, a companion product the film earns.

It must not need a strong model to run. Strong models build it now. Cheap models fill closed forms later, and code checks every
answer. "This is supposed to be designed to produce a really high level of video without even a Claude model."

## The shape

1. **Vessel**: a channel profile. Eight separate, versioned design layers (the Ghost Onions: pacing, motion, layout, transitions, data
   grammar, type, colour, emotion), a voice, thumbnails, sources, a point of view. A Vessel is data, never code.
2. **Crossroads**: seven dealt cards, each a title with its thumbnail and its proof. Take one.
3. **Pact**: one receipt before any money is spent.
4. **Conjuring**: outline, acts in parallel, voice, pictures, picture checks, scenes, render. Safe to leave.
5. **Spell Strip**: watch the film, fix single scenes. No timeline: a film is scenes in acts.
6. **Publish Kit**, **Canopy** (what the numbers say), **Offering**.

Nineteen rooms in all: [11-juju/page-map.md](11-juju/page-map.md), pictures 105 to 123 in the library.

## The three surfaces

| Surface | Built with | State now |
|---|---|---|
| **Web app / rooms** | HTML rooms on one shared parts kit, desktop 1440 and phone 390 | Round 2. All 19 rooms drawn with working buttons and many states. No real film, wallet or voice behind them. Second-round review still running. |
| **Mac app** | Tauri v2 shell (`apps/juju-shell`) around the same rooms and the Rust crates | Shell and icons exist, with two commands (skills, card reading time). No release build shown. |
| **Android APK** | Tauri v2 Android, target Galaxy S20/S21 | Android kit installed, `gen/android` folder exists. **No APK file built. Nothing has run on a phone.** Must make and judge sounds with the Mac off (ADR 0001). |

Ambi uses the Mac and the phone; the phone must also render. Phone rendering is unproven.

## The engine, crate by crate

| Crate | Job | State |
|---|---|---|
| `juju-core` | loads a Vessel, word clock | small, tested |
| `juju-skills` | embeds the 44 skills so the app acts on them | 44 valid |
| `juju-stage` | checks, heals, draws and gates film scenes ("worlds") | nine worlds drawn; not judged since round 1 |
| `juju-script` | lint against AI writing, story, claims, new-thing and order gates | four attack rounds; see [script-gates](11-juju/script-gates.md) |
| `juju-conduct` | runs every skill of a stage: make, check, critique, repair, learn | good film passes on mock models; critics still break it |
| `juju-reliquary` | finds and licence-checks archive pictures | 112 kept, 0 bad |
| `juju-absorb` | strips a pasted video into a channel profile | being built |

Full detail: [11-juju/README.md](11-juju/README.md).

## Hard rules

- Rust first. Thin glue elsewhere.
- **Quiet screens**: names and verbs only. No line under a title (ADR 0009, checked by code).
- **Design systems**: type, palettes, quotes, motion and textures are libraries of data. Nothing invents a one-off style (ADR 0008).
- No film is a picture count. No slideshow. A stage holds and one thing in it changes.
- Sounds come from Earshot, never from a toy-sounding generator.
- Nothing on screen claims what is not real: the truth check fails "Connected", "Film ready" or made-up numbers.
- The money is fixed. The app lowers effort before a wallet runs dry; it never asks for more.

## What is not proven

1. A full run, script to finished film, on the paid services. 2. Any film a judge scored above 5 of 10 from a cheap model. 3. Speed: measured
0.42 times real time on a busy Mac against a target of 4 to 8. 4. Anything on a phone. 5. The absorber on a new channel. 6. That the
135 CAD carries 60 days: voice and the number of films are not yet in the sums, and Gemini's cache saved nothing in 3 tries.
