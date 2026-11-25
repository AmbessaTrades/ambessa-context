# 0016 Rip and replay: measure the pasted film, play the measurements

> **25 Nov 2026 (ADR 0022):** the engine for maps is now `juju-maps/`, and its edit is measured on one donor (`grammar.json`). Cloning a film's words, drawings or marks is still out.

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

**Status:** the product's core as Ambi restated it, 24 Nov 2026: "Again, this is about Juju being able to rip design
systems from any video that's pasted." "Why does ours have lines? I think there's a lot of AI-isms going into the
generative code [...] imagine how the lesser models are going to." "What they're doing is a little bit more 2.5D."
"They think about storyboarding as well. How do we create stories like that." "Juju must produce good." The method
below is the lead's.

## The diagnosis

The dash over a quote, the pill round a name, the boxed picture, the dye wash: none is in the studied films. Builders
invented them, because they were asked to design. A model asked to design falls back on its habits; a cheaper model
falls back harder. So nothing on screen may be invented.

## The method

1. **Rip.** A pasted film becomes `rip.json`: each shot as layers with measured numbers only. Ground; pictures (region,
   feather, scale and position over time, depth order); lettering (box, size, weight, case, tracking, ink, when and how
   it arrives and leaves, as a sampled curve); data worlds (map, chart, flight, instrument) with what drives them; cuts;
   holds; sound events; what the voice is doing.
2. **Replay.** One player draws any `rip.json`. First test: replay the donor's own content and compare with the donor,
   frame by frame. This needs no taste: the error is a number per layer. It is a private test, never output.
3. **Swap.** Same measured film, our own subject, words, pictures and data. Slots are closed; the cheap model fills
   slots and nothing else. A slot it cannot fill well drops its shot; nothing is improvised in its place.
4. **Held-out proof.** A film the builders never saw goes through with no code change. That score is the honest measure
   of "any video". Layers the player cannot draw yet are listed, not faked.
5. **Ours, not theirs.** A channel's look is composed from at least two rips and its own colours, type and subject;
   words, pictures, marks and names of a donor never appear in output.

## Purged (Ambi and the planner, same hour)

Pastel and bright walls; dye washes over pictures (pictures keep their colour); boxed or bordered pictures; dashes over
quotes; pills or badges; paragraphs beside maps; picture-left-text-right as a default. `design/palettes.json` cut from
40 to 11 candidates; the 40 are kept in `design/work-palettes/` as rejected. The design libraries stop being written by
hand: an entry may only come out of a rip.

The running world (0015) goes on beside this: it is the player's data-world layer.

## Stopped the same hour (lead, 24 Nov, about 15:00)

Universal rip-and-replay is withdrawn before it built anything: it was a second new renderer and the riskiest idea of
the day. Ambi: "Why don't we play to our strengths? World maps and science channels are excellent [...] three to six
niches [...] refine the hell out of them [...] you guys have to learn how to test."

What stands instead:
1. **Few engines, hand-tuned once, in `crates/juju-stage`:** first the map engine and the space engine (route, scale,
   instrument), because that code drew the frames he praised (026 and 027 of the blind sheet). More only after these
   two are good every time.
2. **Absorb = measure, then nearest engine plus knobs** (pace, words a minute, script skeleton, colours, title shape,
   thumbnail geometry, sound mood). `juju-absorb measure` already measures; nothing is cloned pixel for pixel.
3. **The gate is code checks plus Ambi's eye on a clip.** Blind judges find faults; they do not decide.
4. Still banned from the purge above: dashes, pills, boxed pictures, dye washes, pastel walls, drawn people and props.
The running world (0015) pauses after its premise step until the two engines are proven.
