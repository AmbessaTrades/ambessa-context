# ADR 0031: the skills reach the engine; High Juju runs the same way as Gris-gris

Working document, changes with conversation. Nothing here is a requirement until Ambi says so.

## Said by Ambi, 28 Nov 2026 about 16:30 EAT

1. Kingdoms and wealth stay, "but if ... none of them [the skills] reach the engines then how can they stay as they are. Things need to change and be updated and upgraded so that the necessary skills to make something much better reach the engine without needing a Claude Code sub."
2. High Juju (the dear grade, Claude) "needs to work in the same way that Gris-gris does" on the app and on the web: through the API, not through a Claude Code session. (Restates his 26 Nov word: "High Juju on the APK and web must be a direct API call, since the Mac will be closed.")
3. Bending must be "more lifelike while still niche bending ... with Kallaway's principles too".
4. In one channel, "one video from the next video needs to be ideated quite completely differently in different unique ways".
5. 90/70/50 (Echo Decay) is "only if we get out there": it starts after a real outlier, never as the default plan.

## What the audit measured (28 Nov)

None of the 59 packs reaches a model when the app makes a film. The models read prompt text written inside `juju-maps/*.py` and its hand copy in `crates/juju-core/src/plan/`. The depth ladder is asked as one turn of thought and checked by no code. `crates/juju-skills` already compiles packs into the binary (`include_dir!`, `src/lib.rs:5`), but the map chain never loads them.

## Lead's design, *candidate* until Ambi accepts it

1. **Seat cards.** Each thinking step (idea, bend, title and thumbnail, outline, script, storyboard, check) has one seat card compiled into juju-core: the fixed text the model reads, the answer's shape, and the checks code runs on the answer. A skill that teaches film craft becomes part of a seat card or is parked. Builder skills stay separate and short.
2. **Depth is an answer field, not a request.** The ladder's rungs (consequence, cost, blind spot, turn), the hook and its payoff, and the living people in the story are fields the model must fill; code refuses an answer whose fields are missing, repeat the title, or do not turn.
3. **One engine, two drivers.** Gris-gris runs the seats in a fixed order, one cheap call each. High Juju runs the same seats with Claude through the Door's API key, and may also look at its own 240p take and revise within a set budget. Same engine, same seat cards, same checks, on phone, web and Mac.
4. **Variety is enforced by code.** Each film in a channel is described on a few axes (kind of story, way in, format, frame, hook, title form). A new idea that matches the channel's recent films on too many axes is refused before it is shown.
5. **Echo Decay waits for an outlier.** The 90/70/50 chain arms only after a film passes 2 times the channel's usual views.
