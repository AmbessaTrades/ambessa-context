<!-- copied from the Juju repo: docs/STAGE-FORM.md, last changed 19:24 EAT, 26 Nov 2026. Private lines removed. Do not edit here. -->
# The stage form: how a weak model makes a strong film

> **Retired for map films 25 Nov 2026 (ADR 0022):** replaced by the hero, sets and beats of `juju-maps/` (`docs/STACK-MOVE.md`, pack `veve-gait`). Still the form of the app's older chain, `crates/juju-stage`.

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.
> Status: candidate design by the lead, 24 Nov 2026. Being tested, not decided.

## The idea in five lines

1. A film is a few **stages**. A stage is one drawn world that stays on screen (20 to 200 seconds) while **one thing
   in it changes**: a hand moves, a line grows, a marker walks a road, a quote is inked word by word.
   Evidence: the films in the gallery (plates 007 to 010) hold a cockpit, a solar map or a planet and move one state.
2. Strong builders make each stage type once, as Rust code with its motion built in, and look at the pixels.
3. A channel pack lists which stage types that channel may use, its fonts, colours, pacing and sound mode.
4. Per film, a cheap model only **fills a form**: for each paragraph, pick a stage type from the pack's list and fill
   its slots. Code checks every answer and re-asks or falls back. The model never draws, times or styles anything.
5. Code renders. Code gates the pixels. A person watches three spans and approves.

## What old Loop got wrong, kept out by this form

"70 pictures, one every 25 seconds" is a slideshow: YouTube's monetisation policy names image slideshows, templated
storylines and scrolling text with little narrative. A stage film has no picture count. It has scenes with change.

## The form (per film)

```json
{"film":"lot-r01","pack":"lot","scenes":[
 {"stage":"object_table","from":"You push the bowl away.","to":"no towels.",
  "slots":{"object":"bowl","title":"Hour one."},
  "events":[{"at":"push the bowl","do":"reveal","part":"object"},{"at":"Hour one","do":"write","text":"Hour one."}]}
]}
```

- `stage`: one of the pack's allowed types (closed list). Catalog starts with what the 85 second proof already drew:
  `object_table`, `dial`, `curve`, `road`, `rule_card`, `panels`, `chapter_title`, `footage`, `quote_canvas`.
- `from` / `to`: exact words from the script where the scene starts and ends. Scenes must cover the script with no gap.
- `slots`: typed per stage. A picture slot takes an id from the candidate list code gives the model (real files with
  their licence). A text slot must be words that are in the script, or the pack's own fixed labels.
- `events`: something changes. `at` is an exact phrase in the script; code turns it into a time from the word clock.

## What code enforces (the model cannot break a film)

1. Every enum, id and phrase must exist. A wrong one is re-asked alone, twice, then replaced by the pack default.
2. **Change law:** no stretch longer than 7 seconds with nothing new on screen. Code adds the pack's default event.
3. **Variety law:** each 60 second window differs in stage or layout from the one before, unless the pack is a
   "held world" channel (one cockpit, one map), where the moving state must keep moving instead.
4. **Number law:** a number on screen equals the number spoken at that moment.
5. **Source law:** every picture has a named source and licence; real people only as real photographs.
6. Text stays inside the safe box; at most the pack's fonts; contrast measured, not assumed.

## How a pack is absorbed from a reference video (measured by code, labelled by a model)

Speech present or not (decides the sound mode once, for the life of the pack: narrated, sparse radio, or silent with
subtitles) · shot lengths · what stays fixed across cuts (stamps, HUD, caption line) · what moves · colours · words on
screen. A model then labels each shot with a stage type from the catalog; a shot no type fits becomes a request to
build a new stage type. The pack must predict three held-out videos of the same channel before it can be used.

## The experiment (24 Nov)

Three separate weak-model fills of the first three minutes of `lot-r01`, each rendered unattended, then judged by
fresh eyes against the gallery films. Reported: answers right first time, re-asks, fallbacks, gate results, and what
the judges saw. That report is the honest odds.
