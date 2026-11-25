# 0012 Strengths only; no stand-in drawings

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

**Status:** accepted direction (Ambi's words, 24 Nov 2026). The bar numbers are the lead's and are candidates.

## What Ambi said, on the storyboard picture (ours beside the cheap model's)

"Both the cheap model and ours look very bad [...] look at the differences between this one and the outliers of Jade
[Rabbit Hole] [...] the ideation behind these drawings, bro [...] both of them are garbage." "It just looks so 'oh,
Claude made this'. I hate the obvious stuff. Whenever something is obvious I'd rather just choose another niche or
another way." "That design system is terrible. We should just abandon that if we're gonna have that kind of crappy
quality, and you should be able to understand that as well, and use the Asase principles to just think: okay, we can
leave that alone, let's pick up these design systems." "You should lean towards what your strengths are [...] if
you're really good at doing star stuff, then it can lead towards specific things." "Also the script is not that
great. You gotta mimic the flow of the other scripts as well. Why does the skeleton of this work? What is it about
these words, sentences? How is Neon gonna interpret this, GLM, DeepSeek?" "If you advise your sub-agents properly and
really review their work and make it absolutely ironclad [...] how Juju understands a video link and absorbs the
content, then strips it down in different JSONs, and how that's actually used for the next video with ours [...] it
has to actually be good." "We have lists of repos and skills designed to help you fix this [...] see what makes the
skill work and make our own design specifically for Juju, like 10 times better."

## Decision

1. **No stand-in drawings, anywhere.** Juju and its builders never draw a person, a body, an animal or an object in a
   code-made hand (shapes, outlines, stick figures, flat icons) as a film frame, a storyboard, a thumbnail or a sample.
   A frame is made of: real pictures and footage with a named source (paintings, photographs, pages, maps), worlds
   drawn from real data (space, terrain, maps, charts, instruments), lettering, and, where a channel's look needs
   illustration, paid pictures in that channel's own dialect inside the thumbnail budget only (ADR 0008). A planning
   board uses the real candidate pictures or stills the engine really drew. If neither exists, the row is empty.
2. **Strengths only.** A kind of scene, a look, or a design-system entry may be offered to a model or shown to Ambi
   only after it passes the bar: shuffled blind among frames of published films, judges cannot pick it out as
   machine-made more often than chance allows, and they find no tell (lead's candidate: at most 1 of 3 judges flags
   it, and no judge names a tell twice). Whatever fails is switched off in the data, not hidden.
3. **Fail fast (Asase).** Two repair rounds. If it still fails, it is shelved with its reason and the work moves to a
   kind that passes. Nobody hammers a weak look.
4. **The idea before the picture.** A picture that only shows the noun in the sentence is the "obvious" he rejects.
   The storyboard relation list (cause, consequence, contrast, scale, held back) is used, and "shows the thing" is the
   exception, counted.
5. **Scripts are absorbed, not invented.** A script follows a skeleton measured from films that work (what each
   stretch does, how long, where the question, the turn, the number and the quotation sit), filled with our own
   subject and facts. A skeleton is kept only if the cheap models can follow it, shown by blind comparison.
6. **The lead looks first.** No picture goes to Ambi before the lead has looked at it at full size against a real
   frame of the kind it claims to be.

## Slip this records

The lead asked a builder for "a clean plain thumbnail sketch of the framing in one consistent hand" where the engine
could not draw a moment, then showed the result. That request is what this decision forbids.

## Added the same hour (Ambi, 24 Nov): the Jade Rabbit Hole style is dropped

"The Jade Rabbit Hole style of video can only work for Claude. We can learn things from his ideation, storytelling,
storyboarding, but only Claude would be able to do that, so our software won't be able to do it [...] our software
won't be running on what you're running on. So we should drop that and look at other niches for different design
systems that would give us the highest leverage. We need extreme amounts of leverage with the quality that we're
able to produce."

7. **Dropped as a look:** the illustrated underworld walkthrough (painted figures made per scene). Kept from it: how
   he chooses ideas, tells and boards a story. The sample film in `runs/first-film` is of that kind; it stays only as
   test words until a sample from a kept look replaces it, and no room or picture presents it as what Juju makes.
8. **The measure for choosing a look is leverage:** how good the result is when the cheap models and code make it
   alone, per dollar and per minute of machine time, judged blind beside published films. A strong model's ability to
   make something is not evidence. Every test of a look is run with the models the app will run on.
