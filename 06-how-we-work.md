# 06 — How we work

Updated 25 November 2026, 08:15 EAT.

## Talking to Ambi

Answer first. Number the steps. Five items at most. Plain words, no jargon, no preamble, no closing lines. Pictures over text. He asked for "very
minimal" feedback and images as work moves. He speaks by voice: read through garbled words. A hot tone is context, not a new direction.

## Deciding

- Nothing is decided unless he said it. Write candidate, open, estimated. Never state a candidate as a plan.
- He does not want to be asked for a green light on ordered work. Decide, run, record the choice.
- When it is truly his call: at most five questions, each with a recommendation, then stop.
- Do not recommend channels or niches. "Assume there is going to be something that you do not expect."

## The build's review loop

1. A maker builds. 2. Two fresh critics: one looks, one presses every button. 3. A fixer. Up to three rounds. 4. A director looks at the whole set.
5. `truth.py` fails any screen that claims what is not real. `shot.py` fails words (quiet) and layout faults. `gate.sh` runs all of it.
6. Every defect becomes a rule, so it cannot come back.

Since 24 Nov 18:07 a contract (ADR 0018) sits over this: a 23-clause exit check, one change and one measurement, proof on the live thing, no loosened gate. Since 22:03 one unit is one pull request with one round of two fresh reviewers (ADR 0020).
Films count only when they come out of Juju with its own models.

Goal, in his words: a pull request reaches him and "it can just auto merge". Nothing auto-merges; the lead merges through one door after both reviews and green checks.

The same loop is being built **inside the app** (`juju-conduct`): make, check, critique, repair, learn, with a receipt that says which rules were enforced.

## Laws every agent on Juju follows

1. Quiet: names and verbs. A drawing that needs a caption is a wrong drawing.
2. One hand: every drawn thing comes from the shared art library.
3. True: an empty state, never a made-up number.
4. Speed is a feature (the Asase Velocity skill): tap budgets, parallel acts, 60 second proof cuts before full renders.
5. "Nuance" must become a number, a closed choice or code. Two cheap models reading one line differently means the line is wrong.
6. Nothing from old LOT as an example.
7. Real people only in real photographs. No faked records, reviews or countdowns.
8. Study other films for structure; never copy pixels, faces, logos or wording.
9. Test with as little money as possible. Every paid call goes in the ledger.

## Models

Building: Opus 5.5 at medium, a lead that orchestrates (high only for taking films apart, ADR 0021), Haiku 5.5 readers for bulk text, Fable 5.2 as adviser at times. **Running the app:** no Claude model. Gemini 4
Neon, GLM 5.3, DeepSeek Flash, Jev 1.14, Inworld TTS-2, GPT Image 2.6 for thumbnails only.
