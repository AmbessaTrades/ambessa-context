<!-- copied from the Juju repo: mockups/COPY.md, last changed 12:01 EAT, 24 Nov 2026. Private lines removed. Do not edit here. -->
# Juju words

> Working document. Nothing here is a requirement until Ambi says so. The list itself: `kit/copy.json`. ADR 0009, MAKER law 2.

1. A room's title is its Juju name and nothing else. The rail, the back label and every "Open" use the same name.
2. A person reads names, verbs and a few status words. The drawing carries the rest: glow, lid, flame, shimmer, seal, strike.
3. Each room shows one action, a verb plus at most two more words. A price sits beside it as a number, never inside it.
4. An object shows its name, at most one status of one or two words, and its number marked `data-d`.
5. Each meaning has one word everywhere. Asleep means a wallet with no key. Resting means put away. Bare means a tree with no films yet.
6. A room has one name, never a nickname: not "the receipt", "the pot", "money and keys" or "the making".
7. No sentences, no captions, no "sample", no "about". A guessed price shows "≈" before the number.
8. Pages never name a vendor. The key sheet behind a wallet shows the service's web address as data (NAMES.md).

## Lines the flows put under things, and what replaces them
- cauldron, banned subject, line under the pot: status **Banned** on the pot, verb **Change it**.
- cauldron, silent film of mostly archive pictures, line under the sound choice: status **Looks reused** on Sound.
- feed-sight, layout only, line under the feed: status **Layout only** on that version.
- new-vessel, read passed, sound finding on its own line: status **Passed**; the finding is its own gong drawing with Play and **Keep this sound**.
- conjuring, waiting for you to read, "Pictures carry on. The voice waits here for you.": the Pictures card keeps moving, the Voice card turns amber with the cat on it; status **Unsure** with the count.
- tank, line under the level, "Less than one film": the wallet's film count reads `0 films` and the level turns gold.
- tank, done, "Back to the film" under the levels: the one action becomes **Carry on**.
- pact, line under the price, "Covered" or what is missing: covered is a jade glow on the price; anything missing shows its one status (Asleep, Low, Locked or Burnt out).
- crossroads, phone, To the pot as a line under the button: a small pot emblem beside the action, no words.
- mirror-bend, phone, Skip the thumbnail as a line under the button: a small **Skip** beside the action.
- sound, the line under a part, the recording it found or "Nothing found yet": the recording's wave, or **Nothing yet**.
- conjuring, things added after the seal listed under the pact: rows in the Pact sheet, with date and price as data.
- offering, line under the reason: the person types it in a blank field. No placeholder sentence.

## The other "one line" sentences, grouped by meaning (109 in the flows)
- No network, no internet, no signal, needs a connection: **Offline**. Any Mac that is asleep, closed, off or out of reach: **Mac closed**. A file or key that exists only on the Mac: **Mac only**.
- Spending is locked: **Locked**. The test money is used up or burnt out: **Burnt out**. A wallet under three days of films: **Low**.
- Every "Nothing … yet" or "No … yet" (pot, deck, shelf, wall, film, kit, and the offering's "Nothing to sell yet" with its counts as numbers): **Nothing yet** beside the room's own empty drawing. The canopy's "Waiting for film one": **Bare**.
- Being built, or "Two looks must be Ready": **Being built**, with done and needed as numbers.
- Not checked, not cleared, not reviewed, free test not passed, and "9 sounds wait for one listen": **Unchecked**.
- "Not read yet" and "Film 1 has no day 30 reading": **Unmeasured**, with the verb **Add numbers**.
- Every "Practice: stand-in voice…", "nothing can be painted" and "not for YouTube": **Practice**.
- "From the next film" and "Past films keep theirs": **Next film**. "For this film" and "This film only": **This film**.
- "Same layout as your last film": **Held**. "Guessed N of 3": **Passed** or **Failed**, with "N of 3" as data.
- Sound check, "Heard as…": **Passed**, **Nearly** or **Failed**, with what was heard as data. "Health lines will be written out": **Health lines**.
- "Safe to leave", "Leave the lid open", "Timing it": gone. The action **Leave it working** already says it, and the time appears once it is measured.
- Reason chips when a card is rejected (inside the sheet): **Wrong claim**, **Wrong picture**, **Wrong tone**, **Unclear**, **Seen before**.

## Words that cannot be avoided
- **YouTube**: it is where every film goes, so a person must recognise it. Used only in "Open YouTube"; elsewhere it is "Channel link".
- Units next to real numbers (subscribers, median views, films, views, asks, min, words, left). Law 3 asks for them.
- Catalogue names (looks, loadouts, voices, ways of speaking, thumbnail styles, outlier titles) are content and marked `data-d`. They live in their own catalogue, not on any screen.

## Open, for Ambi
- The current pages say "The Altar", "The Pact" and "The Sound Shelf". This list says "Altar", "Pact" and "Earshot" (ROOMS.md: "sound | Earshot").
- The way of speaking "Elder brother" sits close to the writer mind "Elder". The catalogue name was left as it is.
- "Copy" means both copy-to-paste (Publish Kit) and make a second vessel or voice. The flows use it both ways.
- copy.json has no place for words inside sheets (the lists in More, key sheet rows, option values). Those sheets stay quiet under the same law.
- The canopy's Key sheet (Asleep, Holding, Glowing…) is dropped. A blossom shows its glow and its real multiple.
- The pact flow's practice button says "Make a free practice film". Here it stays **Incant**, with the status Practice and a price of $0.00. "Wake" (a resting vessel) sits close to "Wake it" (a wallet with no key). "Numbers" is used for a layer, a kind of look, and channel figures.

## How words_at_rest is counted
Words are counted with kit/shot.py's rule: two or more letters, `data-d` not counted. The count includes the frame: rail 3, the Tank chip, and the back label if the room has one. Phones show 1 or 2 fewer words because the back and Tank labels hide. Worst room is the Tank: 25 words on desktop, 23 on the phone. A room's objects, status and tabs lists hold every name it may show across all its states; no single screen shows them all.
Other verbs shown at rest, all from the shared verb list: gate Reset PIN; altar Wake Elder, Open Vessel, More; crossroads Reject, Deal seven; mirror-bend Repaint, Skip; feed-sight Blink, Squint, Bend again; cauldron Change it; arcana Watch, Absorb; pact More; conjuring Stop; publish-kit Open YouTube; Earshot Build, Throw out; voice Find a voice; reliquary Find, Add.
Each count is taken in the room's fullest normal state: gate ready, altar today, new-vessel ready-made open, vessel normal, crossroads Echo awake, mirror-bend Ready painted, feed-sight Ready, cauldron from_card, arcana at_rest, pact ready, conjuring drawing, spell-strip ready to watch, publish-kit ready, canopy Growing, offering Ready, Earshot Passed, voice In use, reliquary Filled, tank Ready.
