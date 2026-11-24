# 0009 Quiet screens, quiet frames

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

**Status:** accepted for the app's screens (Ambi's words, 24 Nov 2026). The film half is the lead's reading of
"I don't want that to bleed into how we do things" and is a candidate until he sees films.

## What Ambi said

"I'm seeing a lot of text everywhere [...] you're not that great at copy." "I love the nuances of Juju language of
course, but there doesn't need to be subtext everywhere. Just stop writing subtext everywhere." "This random subtext
that says 'every part a room may use in every state it can be in': remove all this stupid subtext." "Opus and Claude
models have this thing where when they're doing design systems or designing UI they tend to just put text everywhere.
Beside wallets, why is there text beside wallets, and then 'sample numbers'." "On a mobile it looks worse." "It looks
beautiful, it looks gorgeous, but you can't have text everywhere." "I don't want that to bleed into how we do things."

## Decision

1. **Screens.** A room at rest shows names and verbs only. No line under a title, no line beside a heading, no
   sentence explaining a part, a drawing or a state, no "sample" tags. Limits, checked by code in
   `mockups/kit/shot.py` (faults that start `QUIET`): 30 interface words at 1440 px, 24 at 390 px, no text of 5
   words or more, a name plus at most one status of 1 or 2 words per object. Made-up numbers are not shown at all,
   so nothing needs a "sample" tag; a true empty or asleep state is shown instead. Outside text (film title, channel name, a number) is
   marked `data-d` and not counted. The numbers 30, 24, 5 and 2 are the lead's; Ambi set the direction, not the numbers.
2. **Why it kept happening.** The old maker law asked for a plain-English line under every Juju name. That law is
   removed. A drawing that needs a caption is a wrong drawing.
3. **Design-system sheets and library pages** (type, palette, quote, motion) follow the same law: a name per entry,
   the specimen, nothing else. Notes live in the JSON, not on the sheet. Specimen text (the sample words set in a
   type system, a quotation in a quote structure) is content, marked `data-d`; a quotation is never shortened to pass.
4. **Films (candidate).** Words appear in a frame only when the words are the content: a title, a quotation, a
   name or number the picture needs. No caption that repeats the voice, no label on every object, no line under a
   chapter title, no badge, no corner text unless the channel profile fixes one. The measured text limits in
   `docs/ENGINE-2.md` (Text law) stay; this adds: at most one text element arriving at a time, and a library entry
   that needs explanatory text to be understood is not built.
5. **Agents writing for Ambi** show pictures and few words for the same reason.
