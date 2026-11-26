<!-- copied from the Juju repo: mockups/ART-BRIEF.md, last changed 19:24 EAT, 26 Nov 2026. Private lines removed. Do not edit here. -->
# Art brief, round 2 (after Ambi saw round 1)

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

## What Ambi said, 24 Nov 2026, in his words

"I like the overall vibe, but there needs to be a little bit more cohesiveness between the pages and better graphic
drawings. I can tell you're drawing them yourself."

"There's some gourds that are like falling off of the string, I don't get it. The logic behind the visuals has to make
a lot more sense and they have to be better fit and more beautiful and just absolutely S tier. They can't feel like
they're drawn from a kid. I like the real feel but it just feels a little bit childish sometimes, but I do like how
they match the logo brand, so if we can keep that going."

"When you click through buttons it has to feel fun to use."

"43 out of 70 [pictures]: that reminds me of old LOT language." "What's with those goofy spell strip images."

"For the tank, I didn't pay for those APIs yet."

## Why round 1 looked childish (the lead's diagnosis; test it with your eyes on `passB/shots/*.png`)

1. Six makers drew about eighteen unrelated objects (jars, gourds, a stall, pots, a drum, a tree), each in their own hand.
2. Thin wobbly outlines with no weight, no light and no depth read as doodles. The wobble filter makes it worse.
3. Drawings were decoration first. Several carry no meaning: a gourd on a cut cord, a jar pattern, a pot shape.
4. The references (the game screens in ROOMS.md) are structure first: crisp framed panels, strong type, small exact
   emblems, one lit focus, deep layered dark. Illustration is rare and excellent.

## Laws for round 2 (they add to MAKER.md; where they differ, these win)

1. **One hand.** Every drawn thing comes from one shared library file, `art.js`, in your direction's folder. Rooms
   compose from it and draw nothing of their own.
2. **A drawing must carry a state, or it goes.** Say in one line what each object's shape, fill, light or position
   means. A reader who has never seen the app must guess it right. If words or a number say it better, use those.
3. **Craft.** Confident geometry, deliberate line weight, real light and shadow, depth in layers, texture that is
   designed. No wobble filter on small things. Nothing that could be mistaken for a child's drawing or for clip art.
4. **The cat is the brand.** Ambi's logo (in `kit/kit.js`) is used as drawn. Everything else must look like it belongs
   in the same world as that mark without imitating its naive line.
5. **Own art.** Learn structure from the references. Reuse none of their characters, ornaments, icons, names or text.
6. **Sameness across rooms.** Room name, channel name, back, close, the one primary action and the bottom bar sit in
   the same place and look the same in every room, at both sizes.
7. **True on screen.** Nothing is paid, connected or funded yet. No film, voice or picture of ours exists; only a
   script. Library of Tehuti: 277,000 subscribers, 3,700 median views. Anything else is absent or clearly a sample.
8. **Films are not picture counts, and nothing comes from old LOT.** A film is scenes in acts. Never "43 of 70
   pictures". No fasting walkthrough, no red monk, no `lot-r01`. The sample film is `runs/first-film/film.json`; real
   frames come from that film once the engine has drawn it. Until then a film frame is an honest empty plate.
9. **Feel.** Pressing, picking, sealing and finishing each have a small, quick, physical response. Reduced motion respected.

## The tank, since he named it

It answers three questions at a glance: how much money is left in each service, what today cost, and whether spending
is locked. Today every service is unfunded and unconnected, and that must look calm and correct, not broken. The
picture for "money left" must be one a person reads without thinking (a level, not a thing hanging or falling).
The plan, not spent: voice 45, pictures 44, scripts 22 and 23, checker 10 (CAD, brief 16.1). The lead's advice to Ambi
today is to fund only scripts and pictures at the smallest amount, so do not show the plan as a to-do list of payments.

## Added 24 Nov, after Ambi saw the round-2 parts

"It looks beautiful, it looks gorgeous, but you can't have text everywhere." "There doesn't need to be subtext
everywhere, just stop writing subtext everywhere." "Why is there text beside wallets, and then sample numbers."
"On a mobile it looks worse." "I don't want that to bleed into how we do things."

10. **Quiet.** MAKER.md law 2. The drawings now carry the states, so the words that explained them go. A reviewer's
    first question on every room: which words can be removed with nothing lost? Remove them.
