# 02 — The software: Juju

State at 08:15 EAT, 25 November 2026. Live numbers: [10-now/status.json](10-now/status.json).

## What it must do

Ambi, 24 Nov: "If I put any video in there, a faceless video, it will know exactly how to strip it down, wire it up, and make
our own version of it in every way." The aim he named: 52 minute, TV-style films that a sixty year old watches on the couch, and then
**the Offering**, a companion product the film earns.

It must not need a strong model to run. Strong models build it now. Cheap models fill closed forms later, and code checks every
answer. "This is supposed to be designed to produce a really high level of video without even a Claude model."

## The shape

1. **Vessel**: a channel profile. Eight separate, versioned design layers (the Ghost Onions: pacing, motion, layout, transitions, data
   grammar, type, colour, emotion), a voice, thumbnails, sources, a point of view. A Vessel is data, never code.
2. **Crossroads**: five dealt cards (the running app; the brief said seven), each a title with its thumbnail and its proof. Take one.
3. **Pact**: one receipt before any money is spent.
4. **Conjuring**: outline, acts in parallel, voice, pictures, picture checks, scenes, render. Safe to leave.
5. **Spell Strip**: watch the film, fix single scenes. No timeline: a film is scenes in acts.
6. **Publish Kit**, **Canopy** (what the numbers say), **Offering**.

Nineteen rooms in all: [11-juju/page-map.md](11-juju/page-map.md), pictures 105 to 123 in the library.

## The three surfaces

| Surface | State, 08:15 EAT, 25 Nov |
|---|---|
| **Web app / rooms** | A Rust server runs and answers. Eight core rooms (Gate, Altar, Crossroads, Cauldron, Pact, Conjuring, Spell Strip, Publish Kit) work when pressed at desktop and phone size. **Every path still ends at the same practice minute**; a worker was put on making "Make a film" start the real film at about 08:00. The other eleven rooms make no server call. [buttons](11-juju/buttons.md) |
| **Mac app** | Tauri shell around the same rooms. No release build shown. |
| **Android APK** | The phone job ran on an emulator (the lead, 24 Nov 23:14: 19 checks pass, 3 fail). Paused for the harvest night. No APK in the main folder, nothing on a real phone. It must make and export films with the Mac off (ADR 0019). |

## One command makes a film

`juju make` runs eleven stages: slot and rest, deal and package, pact, outline, script and heal, clock and voice, pictures and form, render and mix, review, publish kit, measure. 24 Nov 18:35: 2 of 11 worked.
25 Nov 06:45: 11 of 11 on one subject, silent, one minute. Every run: [10-now/films.md](10-now/films.md).

## The engine, crate by crate (Rust; line counts in [status.json](10-now/status.json))

| Crate | Job | State |
|---|---|---|
| `juju-cli` | the one command | makes a one-minute silent map film |
| `juju-stage` | checks, heals and draws scenes | map and space engines liked by Ambi; 12 of 40 moves; depth worlds being added |
| `juju-next` | reads films, deals title cards, bends titles | two sealed readers; few cards survive its truth checks (PR 24) |
| `juju-gather` | bare title to sourced facts, map tables, pictures | fast and cheap; facts bar not called true yet (PR 25) |
| `juju-script` | writing checks | catches the refused line; refuses too many good published films |
| `juju-sigil` | thumbnails drawn by code, gates G1 to G5 in code | 29 of 29 code checks; thin when the film's data is thin (PR 21) |
| `juju-sound` | beds and cues heard by Earshot, -14 LUFS | works on test strips; a money reserve fault on main (PR 26) |
| `juju-db` | the vault: slots, resting shelf, sameness meter | stage 0 built |
| `juju-conduct` | make, check, critique, repair; keep or revert; step up one model | merged, PR 12 |
| `juju-serve` | the app server | 117 route checks pass |
| `juju-reliquary`, `juju-absorb`, `juju-core`, `juju-skills` | archive pictures, film measuring, vessel data, embedded skills | used by the above |

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

1. Any film a person would publish. 2. Voice in a real film. 3. Ten minutes or more. 4. A pasted link becoming our own film. 5. Anything on a real phone. 6. Speed: about 3.2 machine seconds a film second in a full run (target 1.0).
7. That 135 CAD carries 60 days.
