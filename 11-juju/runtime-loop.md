<!-- copied from the Juju repo: docs/poteto/runtime-loop.md, last changed 14:15 EAT, 25 Nov 2026. Private lines removed. Do not edit here. -->
# The loop inside Juju

> **Map films (25 Nov 2026, ADR 0022 item 7):** in `juju-maps/` a check reports and the render goes on. What stops: the money cap; a sentence with no source (left out); a picture without rights (left out); Ambi's click to publish. The loop below is `crates/juju-conduct`, unchanged.

How Juju's own models make a film with nobody watching, on the Mac or the phone. This is the same discipline the
builders follow, held by `crates/juju-conduct` in code. A rule here that is only prose is a defect: move it into the
conductor with a test.

## The players

| Name on screen | Job | Never does |
|---|---|---|
| Elder | plans the outline, writes with character | judge its own writing |
| Griot | long drafting when Elder is over budget | judge its own writing |
| Scribe | fills small closed forms, critiques other families' work | write a whole act |
| Watcher | looks at frames and thumbnails | pass a frame it cannot describe |
| Tongue | speaks, once, cached | speak a line that failed lint |
| Pigment | paints the thumbnail only | draw a film frame |
| Earshot | makes sound and listens to it | pass a sound it did not hear |

## The loop, per part

1. **Small closed step.** A model fills one form with a fixed shape: a multiple choice, a short list, one paragraph.
   Target: 95 percent legal at the first answer. A part too big to check is cut smaller before it is retried.
2. **Measure in code first.** Shape, lint, claims against sources, counts, timing, overlap, loudness. Code decides
   everything code can decide.
3. **Then a judge of another family.** A critic never shares a vendor family with the writer. Every look carries one
   planted defect. A critic that misses the plant is blind, and its silence holds the stage.
4. **Surgical repair.** Only the sentences or scenes that failed are sent back, each with the one finding it failed on.
   At most two rounds.
5. **Keep or revert.** After a repair, measure again with the same checks. Fewer findings: keep it. The same or more:
   discard the repair and keep the earlier output. A repair is never kept because it is newer.
6. **Escalate or hold.** Still failing after two rounds: try once on the next model up for that role. Still failing:
   the stage holds, says what failed and what a person can do. A held stage costs nothing more until someone acts.

## What never happens

- A failed scene is never covered by the scene before it or a plain text card so the film can finish. A scene that
  cannot be drawn fails the film, and the fallback count in `faults.json` stays 0.
- A stage never passes on an empty, unparsed or blind critic reply.
- A sound never ships unheard. The mix is measured at -14 LUFS and each cue is checked by the listening model.
- A paid call never starts without a reservation, and a replay never pays twice for a reply already on disk.

## What code holds today, and what it does not (24 Nov 2026, read from `crates/juju-conduct/src/run.rs`)

| Law | State |
|---|---|
| closed forms, shape checks | held |
| critic of another family, planted defect, blind critic holds | held |
| repair only the failed sentences, two rounds, then hold | held |
| keep or revert after a repair | **not held**: the newest repair replaces the output even when it finds more |
| one step up a model before holding | **not held** |
| a covered scene fails the film | held while a pack's `max_fallbacks` stays 0, the default in `crates/juju-stage/src/lib.rs`; a pack that raises it lets a covered scene through, so that number is a gate |
| Earshot hears the mix before the film passes | **not built**: stage 7 has no sound check |

Each "not held" row is one unit of work: a failing test with a mock provider first, then the smallest change that
turns it green, in the lane that owns the file, with a reviewer who did not write it.
