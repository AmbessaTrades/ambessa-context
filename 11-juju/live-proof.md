<!-- copied from the Juju repo: docs/poteto/live-proof.md, last changed 14:15 EAT, 25 Nov 2026. Private lines removed. Do not edit here. -->
# Live proof: what counts as finished

> **Map films (25 Nov 2026, ADR 0022):** the film is in `juju-maps/films/<name>`; read its frames with `scripts/opon.py` on every take. The receipts and pass lines below are unchanged and still name `runs/films` (open: `docs/STACK-MOVE.md`).

A thing is finished when the real thing was run and a receipt on disk shows it. `scripts/exit-predicate` reads the
receipts below. The maker writes the receipt with the tool named. A verifier who did not make it reruns the tool.
Sources: pstack `principle-prove-it-works` and Visual parity, read 24 Nov 2026. ADR 0001, 0014.

## A screen

1. The room is served by the Rust server at `/r2/<room>.html`. A `file://` page proves nothing.
2. `scripts/exit-predicate walk` signs in on the no-paid test instance (`scripts/serve/start test`, port 4701, the same
   server program), presses every visible control at 390x844 and 1440x900 and writes `runs/predicate/walk.jsonl`.
   A room that ends at another address, or shows no controls, fails. Presses never run against the paying instance.
3. Pass: 0 dead controls (a press that changes nothing on the page is dead), 0 layout faults, 0 page errors,
   0 `SAMPLE` tags, at most 2 `Soon` marks in the whole app.
4. Look at one screenshot per room and size yourself. A count never replaces the look.
5. Close and reopen during a running film. The room shows the true stage. That is part of the walk for Conjuring.

## A film

Fix faults on a strip of 60 to 90 seconds first. Render the whole film only when the strip is clean.
Receipts live beside the film in `runs/films/<name>/`.

Every receipt holds `film_sha256`, the sha256 of the film file it was made from. A film drawn again needs its receipts made again.

| Receipt | Made by | Pass |
|---|---|---|
| `FINAL.json` | the owner | `film`, `film_sha256`; `voice` {`wav`, `wav_sha256`, `ledger_times`}; `thumbnail` {`file`, `sha256`, `ledger_times`}. The times are the `time` fields of the paid ledger rows that bought it |
| `render.json` | the render command's own clock | `wall_s` over 0, `film_s` within 1 s of the file, `wall_s / film_s` at most 1.0 |
| `faults.json` | code that reads the film's scene data and frames | `frames_read` over 0; 0 each of `jump_cuts`, `labels_crossing_borders`, `ghost_text`, `readout_mismatches`, `fallback_scenes`, `overlapping_text_boxes` |
| `timing.json` | code that reads the word clock and cut list | `lead_s_median` about 2.5 over at least 10 `leads_measured`, `turn_gap_s_median` about 1.28, `chapter_gap_s_median` about 3 |
| `earshot.json` | Earshot's listening model on the mixed track | `verdict` pass, `cues_heard` over 0, `synthetic_cues` 0, `listening_model` named |
| loudness | `ffmpeg ebur128`, read by the predicate itself | -14 LUFS within 1, true peak at most -1 dB |
| `blind.json` | three judges of another vendor who saw no earlier round, 12 of our frames mixed with 12 published | `ours_called_machine` no more than `published_called_machine` plus one look in ten; `frames_each`, `judges` |
| `LEAD-PASS.json` | the lead, after watching all of it | `who`, `when`, `says`, `watched_whole` true, `role` "lead" |
| `ROOT-PASS.json` | a reviewer who built none of it, after watching all of it | the same, `role` "outside reviewer", another name |

The published frames come from real breakout films already studied: hands, Atticus King, Milky Stellar, Bygone
Philosophy, Jacopist. Judges get frames only, never file names.

## A sound

Make or build it with Earshot. Then run Earshot's listening check on the file and keep its words and numbers.
A cue the listening model calls synthesized, a bleep or a chip tone, fails unless the look is openly chip sound.
Voice is Inworld TTS-2, bought once and cached by the hash of its text.

## A thumbnail

A real WaveSpeed call in the ledger, the file at 1280x720 or larger, and `feedsight-otsu-g1-g6-critic` passed at
feed size. Low proof first, then at most two medium renders.

## The baseline is the spec

The frozen harness, the published frames and the receipts' pass lines are not edited by a maker. If a baseline looks
wrong, stop and send it to the lead.
