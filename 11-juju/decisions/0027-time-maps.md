# ADR 0027: time maps, a channel type of their own

Working document, changes with conversation. Decided 26 Nov 2026, about 00:05 (Ambi, after films/tm-africa and tm-output): "this is definitely the way to go for another design system that can host a whole bunch of different niches"; "these can be like 20 minute videos every day"; "concepts and channel structures that don't use subtitles"; "I'm proud of that rust engine".

1. Two sibling design systems, one engine: **kingdoms** (who held what land; Africa: "absolutely beautiful", "almost perfect") and **wealth** (who made or held how much; the world's output). "We never lose the ability to do these two things"; one channel may use both. Working names.
2. Praised: the maps, the zoom ins, the colours, the idea and the moving share. Wanted: less text ("each layer 1%" is over-explaining), smaller text with zooms in place of big letters, better fonts and captions, smoother motion where things rise and fall, a clock that does not speed up and slow down awkwardly and gives its time to expansions and wars, Juju Poly assets that feel placed (finance things for finance, gold and what was made), facts that pop up at a place, cooler map tricks, colour themes that carry their own fonts and inks in the app, accurate data, pockets that last 20 minutes, neighbouring sub-niches.
3. No glitches. Both films are to be made again, better, and more to follow at 240p.

Open: names of the two systems; how they are grouped in the app; length per film.

## Added 26 Nov 00:50 (Ambi)

4. Voice grades are named **Àṣẹ Regular V 0.3** and **Àṣẹ High V 0.3**; "any improvement only ever goes up by 0.3".
5. Ideas of the kind the systems must hold: "I simulated Atlantis' complete timeline", "I simulated the Sahara region's ancient trade routes", "I simulated how Mansa Musa got rich" (ideas, not final titles; the first is the strongest). They come from the manner of youtube.com/@Jacopist. Space maps later, not now.
6. "Don't break what's working": the two systems coded on 25 Nov (Night and Day, and the time maps) are never put at risk by tidying the stack. Changes to the stack are added beside, checked against the gold films (`juju-maps/stack/golden.py`), and nothing that works is moved or rewritten for neatness.

## Added 26 Nov 01:30 (Ambi)

7. DeepSeek at low thinking is fine for writing ("Okay, yeah, low is fine"). 
8. Night and Day are not given up: "I need to see a really extreme level of consistency"; they may "not need to do so much" if what they do is more consistent. It is not either or: Juju's capability to hold many niches is the aim.
9. Testing is for scale, not for one pretty film: "make sure that everything is calculated ... scalable". Test money is fine when the films seen are excellent and work for different niches. "We need to get more videos pumping for more critiques."

## Added 26 Nov 01:40 (Ambi, after eight time maps and the six themes)

10. "The maps and numbers are blocking so much of the ability to see the map"; the log (the strip at the foot) "blocks sometimes", and the top text too. The camera must know what it has to show: "capture a little bit more of this area", "re-angle the camera in unique ways that kind of capture this point". Where a strip stays, "the camera work has got to be so good that it avoids that kind of stuff".
11. "The pacing has to be much much slower" (the two minute films ran far too fast).
12. "A motion banner at the bottom and at the top just muted", "creative and carefully put but in a subtly different way than the video that we reverse engineered".
13. "Not every text has to be giant": text is sorted into places and sizes by rule, inside Juju Maps and Juju Motion, for every topic.
14. More Juju Poly in the slow moments, Juju Motion to annotate points, "different kind of cool unique zooms", better captions. Charts and data points that show themselves at a moment are liked.
15. All six themes stay ("all of those themes deserve to be there"; the white one "has its uses"). They are updated with items 10 to 14.
16. Open: whether Night and Day are rebuilt round this stack (asked 26 Nov 01:40).

## Answers, 26 Nov about 02:00 (Ambi)

17. Night and Day are redesigned round the time maps' way: "We should redesign night and day around this." Keep the globe for what it is exact at (lakes, rivers, towns, cities, mountain ranges), take the clean drawing of the time-map engine ("the quality of the rust ones just feel like 10 times higher"; the globe's textures "feel weird", "blurry", "the 3D kind of feels weird"), and find a division between them, with a smooth mode that can be switched on.
18. The drawing engine is part of Juju Maps, not a separate thing: "it's within juju maps", "a feature within juju maps design systems", part of the Juju Powers. A name of its own inside Juju Maps is open (Ambi offered "Juju Maps Rust Extend" as a placeholder).
19. A chart usually stays: someone watching from the start would miss it if it vanished; a moment without it is allowed, never a sudden loss.
20. Banners thin; type sizes restructured, thought through in layers.
21. Camera work is a skill of its own: an agent writes and runs the storyboard program; angles, pockets and moments are storyboarded even with no voice.
22. Test now: states. How the American states formed (and Canada's provinces), with the right Juju Poly, Juju Ear and Juju Motion for war (troops marching, small blasts), purchases, trade inside the country, ships to and from the ports; a dive to one place for about two minutes, then back up. Then states for every country, to open about ten more niches; then judge which design systems spawn the most niches.
23. Two or three channels with no voice at all, if the ideas are very well made. Finance aimed at America and its states is one such niche.
24. The six themes stand as named; each must carry these rules and know how to use every Juju Power.

## Added 26 Nov about 02:15 (Ambi, on the 7 minute Africa)

25. At 1:27 the film left Egypt while Persia took it and Egypt drove Persia out: "you didn't annotate that, you were focused on something else". The crucial changes must be seen: "if anything is changing ... we want to see what changed", above all when time is stretched; a run of conquests and recoveries is told whole, in good copy, true to the people's own sources. Juju needs a structure for this: mental models, design systems, stacks, the reasoning behind its storyboard, its copy and its camera.

## Added 26 Nov about 05:20 (Ambi: "assume ur in full control ... make decisions and wire up juju by urself")

26. Lead decisions under that authority, reversible, each open to Ambi's veto: (a) Night and Day take two grounds (stack/GROUNDS.md): the clean drawing plus exact lines for wide views, the plain globe up close, behind `smooth: true`; nothing changes for a film without the field. (b) Working name of the drawing engine inside Juju Maps: Juju Ardhi (folders keep their names). (c) A simulation on real land starts from the real cultures in the world book; imagined peoples only on imagined land (Atlantis, sunken lands), per ADR 0028.
27. Ordered the same hour: every part of the stack runs alone without Claude Code (one command per film, a doctor per part); the app makes films from one tap with every button clicked; more design systems are churned; then launch.

## Added 26 Nov about 05:45 (Ambi, after the 11 minute Africa)

28. "A real video production has no room to say still missing": Juju always gives the best finished product in every design system. A gap is closed before drawing (fill it, or choose the span and subject the sources cover); a film never shows or speaks a gap.
29. "[dates about]" is not liked: be confident. Brackets stay, used for other nuances that matter.
30. The motion of any expansion, conquest or change must be better: when land fills or moves between parts of the map, the viewer must see it happen.
31. The stacked layers (slabs) suit other parts of the design system; here ask what they show that a flatter land could not, and use them only where they carry meaning.
32. A quick outline of the modern country or empire, now and then (not on a rhythm; when the engine judges it helps, above all on zoom-outs), so the viewer can compare the time map with today's map.
33. The year at the top left may pulse or flash subtly at crucial moments, chosen by the storyboard.
34. "I love the camera work." The 11 minute Africa "looks really really good" and can be refined further, using every Juju Power.
35. Rewrite how the stack, design systems, Juju Powers and skills are written and flow with one another, inside Juju's own JSON and MD files, so they are one cohesive system ("13 of 13").
36. (Ambi, about 05:55) A 28 minute film must feel like it "could only have been possible in 28 minutes": ideation, pockets, copy, storyboard, direction and camera, never an 11 minute film stretched. Lead's design (exploring, sent to the long-form lane): one spine question answered three or more times; braided threads that cross at real turning points; setups that pay later, checked by code (a pocket nothing later depends on is cut); a scale ladder with a dive at the heart of each act; lens changes; camera craft held back so each act brings something new; copy that grows from naming to connecting; a novelty meter per minute.

## Added 26 Nov about 06:10 (Ambi, on the US states film, before sleeping)

37. The US film "doesn't look good visually": borders and layers lie on top of each other with no flow; the colour theme does not fit this sub-niche or drive interest (it worked for Africa); the circles (4:06) do not do their job; contested claims need a better way to be shown; spreading borders look weird; it feels laggy and glitchy. A different design approach for this subject, using a good combination of the powers, smooth.
38. Juju may make its own choices inside a film: "maybe we need this, this isn't needed, this would be stronger over here, this would be stronger if this waits for this". Think of interactions, flow, ease of use and speed.
39. Exports at 720p, 1080p and 2K (1440p): "no one ever really wants to export a 480p". 240p stays only for Juju's own quick takes.
40. Before he wakes: log all of this, execute it; the stack and design systems updated; films churned with the updates; Juju's flow working well in the actual app, its buttons and flows well ideated.
Lead's measured read of the US film (06:10): the Native cession layer (Royce 1899) is drawn semi-transparent over the states and territories layer (Newberry), two sources with different edges, so slivers and double edges show; a pastel colour per state on a loud brown relief means nothing; the rings are event markers with no meaning of their own; morphs step. Lead's mark: 4.5, not 6.5.
41. (Ambi, about 06:20, on the Fort Sumter dive) While the camera moves, the Juju Poly assets drift slowly against the map; they must look stuck to the ground. Every body, ring and dot is locked to its ground point (checked by code: under half a pixel at 1080p).
42. (Lead, under Ambi's full-control order, about 07:30) Export speed: measured 1.0 CPU second a 1080p frame; reuse caps at 1.2x, a single sample a pixel changes the picture. Approved: single sample for 240p looks only, x264 veryfast for exports, all cores for exports when the Mac is quiet (the 4-thread cap was the lead's overload fix, not Ambi's). A sized bet: port the drawer to the graphics chip (Metal), kept only at 5x or better with identical-looking frames; stopped if the first two passes gain under 10x.
