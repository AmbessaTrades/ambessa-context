# ADR 0022: Juju makes map films, and only map films, for now

Working document, changes with conversation. Decided 25 Nov 2026, about 11:30 to 12:10 (Ambi): "Juju just only [does] maps for now ... do this one niche really well", "fork it again ... so we won't use Wedjat", "literally called juju maps", "I hate parchment paper", "two design systems is fine", "having hard gates prevents a vid from rendering", "360p or 480p dozens of times rapidly ... on only 1 voiceover", "COPY THAT EXACT SCRIPT TEMPLATE and fill in our own stuff per video", "let's build on top of this", "run on my mac and ... the phone".

1. (Superseded by ADR 0023 items 1 and 2, 25 Nov 21:20.) One niche: empires, wars and borders, anything a map can show. The other niches wait; nothing is deleted.
2. The drawing engine is **Juju Maps** (`juju-maps/`): a fork of bilawalsidhu/gods-eye-view (MIT, upstream 92fcccb), shrunk to its director maths; their name and marks are not used. Wedjat is untouched. `juju-stage` draws no map film once Juju Maps is wired in.
3. The order of work in a film: script, voice, word times, storyboard, maps and motion, pictures, quotes and numbers, sound effects, music.
4. Two looks, as data. No parchment.
5. The script skeleton is J0wWNytEXS4's structure (`wrong-picture`): its beats, order and shares. Its words, drawings, name and subject stay its maker's.
6. Length: about 30 minutes, about 5,000 words.
7. Checks report; they do not stop a render. What still stops: the money cap, a sentence with no source (it is left out, the film goes on), rights of a picture (it is left out), Ambi's clicks for publishing. Supersedes the HOLD law for these films.
8. Looks are judged on fast 480p takes of one voice before a full export. Export target: 20 minutes of work for a film.
9. Open: how a film is made with the Mac closed (keys and model calls need a place that is always on); money above the 9.50 cap for a 30 minute voice (the test cap is 15.00 since 25 Nov 13:55, `runs/meter/cap.json`).
