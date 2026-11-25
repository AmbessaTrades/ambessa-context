# ADR 0029: the world book is built ahead, so films are fast and true

Working document, changes with conversation. Said by Ambi 26 Nov 2026 about 02:25, after the 7 minute Africa.

1. Africa's time map was "so inaccurate": before 1000 BC it showed only Egypt and Kush, Kush appeared "out of nowhere", Ethiopia (which attests itself as an empire tied to Israel for thousands of years) was never shown as an empire, Punt only passed, the Sahara's lost states, the trade routes, southern Africa and the boats coming and going were missing. "You're not realizing how rich Africa's empire systems were." He means fully realised states and empires, not tribes.
2. The same holds for every region: people who know Latin America would tell the Olmec's true timeline; "how do we tell their stories in our history as well".
3. He asks how DeepSeek finds this, to truth, sourced, "under a few minutes where videos get pumped out immediately": "design a system for it, make it happen, juju needs upgrade here."

Lead's design, *exploring* until Ambi accepts it: research is done AHEAD, once per region, into a sourced world book (Juju Roots lane, `juju-maps/roots/book/`); per film the cheap writer only queries the book; a coverage check names what the book lacks and those gaps are filled offline. A state with no drawn border is drawn from its known sites, marked estimate. Claims are kept with their kind (dug and dated, written then, own record, later telling, tradition); a minority reading is told as a reading, or in a lore film.

## Added 26 Nov about 02:35 (Ambi)

4. It must be solid in code, as the time maps are: the regions taken and colonised at a given time are computed from data, "truth to indigenous stories and carbon dating as possible", whatever the age the dating gives ("40,000 years, 37,000 years, 37,643,000 years"). "That needs to be a part of Juju. I swear, I'm not joking."

Lead's design, *exploring*: every drawn shape is a function of sourced rows, never written by a model; dates are stored raw with method, error and lab and turned into ranges by code (radiocarbon calibrated, other methods for ages past radiocarbon's reach); control of land is computed from dated rows of who held which sites; disagreeing sources stand side by side and the choice between them is a rule in code.
