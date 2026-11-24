<!-- copied from the Juju repo: mockups/r2/PARTS.md, last changed 11:34 EAT, 24 Nov 2026. Private lines removed. Do not edit here. -->
# Juju parts, round 2

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

Every room is built from four files in this folder, linked in this order:
`<link rel="stylesheet" href="kit2.css"><script src="kit2.js"></script><script src="light.js"></script><script src="art.js"></script>`.
A room draws nothing of its own and sets no colour of its own. See every part in every state: `kit-sheet.html`
(`?skin=codex|atelier|daylight`, `?part=a|b|c|d`, `?state=sheet|toast|motion`, `?flat=1` for a full-length picture).
`light.js` is generated: change an object in `build/bake.py` or `build/tree.py`, run it, then `build/pack.py`.

## Shell

- **Room**: write `<body data-skin data-room data-title data-channel data-chan-state data-back data-back-label data-tank data-who>`, then `<main>`, optional `<div data-tools>`, `<footer class="deck">`; kit2.js builds the rail, head and deck in the same place in every room.
- **Rail / bottom bar**: built for you: Ambi's mark, three doors (Altar, Crossroads, Cauldron), the person; on the phone it becomes the bottom bar. Set `data-door` if the lit door is not the room.
- **Head**: back (`data-back`, `data-back-label`), room mark (`data-mark` emblem, defaults to the room), room name (`data-title`), channel with its state dot (`data-channel`, `data-chan-state="need|work|stop"`), your tools, then the Tank chip (`data-tank="asleep|ok|low"`), always last.
- **Deck**: `<footer class="deck"><div class="aside">…</div><button class="primary">…</button></footer>`: bottom right on the desk, above the bottom bar on the phone. Exactly one `.primary` per room.
- **Primary**: `.primary` (lit slab); `.need` gold, `.breach` ember (breaking a seal), `.busy` while it works, `disabled` when there is nothing to do. `Kit.finish(btn,'words')` rings it and toasts.
- **Buttons**: `.btn` secondary, `.btn.need`, `.btn.stop`, `.btn.bare` quiet, `.btn.icon` square with one `Art.glyph`; `.chip` for head tools.
- **Hall**: comes with `.room`; `--focus-x` / `--focus-y` on the body move the pool of light to the room's focus.

## Frames and surfaces

- **Panel**: `<div class="panel" data-frame>`; `.focus` for the one thing in view (`data-frame="crest"` adds the peak and brim), `.need`, `.stop`, `.sunk` (a well objects stand in), `.flat` (inside sheets).
- **Niche and ledge**: `<div class="niche need|work|pick">object</div><i class="ledge need"></i>`: the arched hollow a jar or object stands in, lit by what is inside.
- **Rule**: `<div class="rule"><i></i></div>` divides inside a panel.
- **Sheet and veil**: `<section class="sheet" id="x" hidden><h3>Plain name</h3>…</section>`; open with `data-open="x"` or `Kit.sheet('x').open()`; `data-close`, the veil or Escape closes it. Depth always goes here, never in an Advanced fold.
- **Toast**: `Kit.toast('The title is copied',{state:'need|stop',art:Art.seal({state:'live'})})`: one short sentence of what just happened.

## Lists and controls

- **Rows**: `<div class="rows" data-pick><button class="row" data-card><span class="tile">emblem</span><span><b class="name">…</b><span class="sub">…</span></span><span class="val">…</span></button>`; `.on` picked (lit from its edge), `.need`, `.stop`, `.off`.
- **Tabs**: `<div class="tabs" data-tabs data-scroll><button class="tab" aria-selected="true" data-panel="id">Name <span class="n">8</span></button>…`; `data-panel` shows the matching panel.
- **Pills**: `.pill` plus `.work` running, `.need` yours, `.stop` locked or refused, `.dim` asleep, `.sample` for anything that is not real yet.
- **Switch**: `<button class="switch" aria-checked="true">Words</button>`; the bolt slides and lights; `disabled` when it cannot be used.
- **Stepper**: `<div class="stepper" data-min="1" data-max="7" data-unit="per week"><output data-v="7">7</output></div>`.
- **Pick**: put `data-pick` on any group and `data-card` on its items; the picked one gets `.on` and a stamp.
- **Status**: `<span class="status">Art.pip + words</span>` for a few plain status words that move by themselves.

## Plates and film

- **Plates**: `<div class="plate empty|working|failed"><span data-art="plate" data-state="…"></span><span class="says"><b>Not drawn yet</b><span>why</span></span></div>`: the honest place where a picture or film will be.
- **Scene strip**: `<div class="strip" data-scroll><div class="act"><span class="lab">Act I · Name</span><div class="scenes"><button class="scene drawn|picked|changed|working|failed">…`; a film is scenes in acts, never a picture count.
- **Steps of a film**: `Art.path(['done','next','none'])` and `Art.pip({state})`: done, next (yours), now, failed, none.

## Cards

- **Card**: `<button class="card"><span class="pic"><img></span><span class="t">title</span><span class="proof"><span>channel</span><span class="num">8.00x</span></span></button>`; `.picked` (+ `<span class="stamp" data-art="seal" data-state="pressed">`), `.rejected` (+ `<i class="x-out">`), `.echo` (+ `<span class="link">follows a hit</span>`), `.down` (face down) with `Art.cardback()`.
- **Dealt hand**: `<div class="hand" data-pick data-scroll>` of `.card data-card`; fans on the desk, swipes on the phone; `Kit.deal(hand)` deals it in.

## Objects (art.js, all lit from the upper left)

- **Channel jar**: `Art.jar({state,label,near})` or `<span data-art="jar" data-state="needs" data-label="LT">`; asleep (hat lid, slate), needs (flame), working (jade vapour), done (jade seal), stopped (ember cord), new (glass ghost and plus); `near:'l'|'r'` when a lit neighbour stands beside it. Put it in a niche; `.jarbox` + `.objname` + `.objstate` for a pickable shelf item.
- **Wallets**: `Art.wallet({mind,state,level})`; mind is tongue (voice), pigment (pictures), elder (deep writer), griot (fleet writer), scribe (text checker), watcher (picture checker); state asleep (no key, say "Asleep" and "Wake it"), ok (jade), low (gold, under three days of films), locked (ember seal). Level is money left as a share of the plan, from the live service only. Use inside `.rack` as `.wal` with `Art.medal(mind)`, the dollars in `.left`, films in `.films`. `Kit.wake(el)` fills it from nothing.
- **Tree**: `Art.tree({boughs:[{state,flowers}],focus,zoom})`; bough state bare, bud, bloom (jade, the real multiple in `flowers`), gold (kept after five wins), prune; `zoom:true` with `focus` closes in on one bough for the phone. Today every bough is bare.
- **Seal**: `Art.seal({state,emblem})`; blank ring, pressed (bone), live (jade), void (ember). `Kit.seal(slot,state)` thuds one onto any slot.
- **Scroll receipt**: `<div class="scroll"><div class="rod"></div><div class="paper"><h4>…</h4><div class="ln"><span class="k">Voice</span><span class="fill"></span><span class="v num">$0.84</span></div>…<div class="total">…</div><span class="wax" data-art="seal" data-state="blank"></span></div><div class="rod"></div></div>`; `.void` when stopped; `Kit.seal(wax,'live',{emblem:'pact'})` seals it.
- **Copy seals**: `<button class="copy" data-name="The title" data-text="…"><span class="slot" data-art="seal" data-state="blank"></span><span class="what">…</span>glyph</button>`; a tap copies and presses the seal; `.live` once it is on YouTube.
- **Dial**: `<div class="dial" data-value=".8" data-min="10" data-max="60" data-unit="min" data-state="set|held|off"></div>`; drag up and down to turn.
- **Effort knob**: `<div class="effort" data-effort="1">` with three `<button class="step">` (Quick, Crafted, Masterwork), each with what changes, its cost and its minutes; mark costs as estimates and minutes "not timed yet" until measured.
- **Sound**: `Art.sound({state,seed,progress})` (gong and waveform) or `Art.wave({…})` alone; empty, made, playing, kept, rejected.
- **Voice**: `Art.voice({state})`; none, standin (silent timing voice, costs nothing), chosen, speaking. Never a face.
- **Offering chest**: `Art.chest({state})`; asleep, wanted (gold sparks), ready (tied and sealed), live (open, jade light).
- **Lock**: `Art.lock({locked})`; open bone, locked ember.
- **Marks**: `Art.emblem(name)` for rooms and the six minds (`Art.rooms`), `Art.medal(name,{state:'on|off|need|work|stop'})` struck in metal, `Art.glyph(name)` for small line icons.
- **Cat**: `<span class="cat"></span>` (add `scan` for the eyes); it is Ambi's logo as drawn, the only character.
- **Any object in place**: `<span data-art="name" data-…>` is replaced by its drawing, keeping classes and data; `Art.fill(el)` redraws it.

## Feel

- **Press**: every `.btn`, `.primary` and picked item gives a short stamp on tap; the primary sinks onto its lip.
- **Pick**: `data-pick` stamps the picked item; tabs, switches, steps and steppers each answer on tap.
- **Seal**: `Kit.seal` thuds wax down with a ring of light.
- **Finish**: `Kit.finish` rings the primary outward and toasts in plain words.
- **Deal / wake**: `Kit.deal` deals cards in order; `Kit.wake` raises a wallet's level. All motion stops under reduced motion.

## Words

- **Quiet law (Ambi, 24 Nov), in MAKER.md law 2: names and verbs only.** No `.sub`, no `.objstate`, no second line in
  `.says`, no sentence beside a heading, no caption for a drawing, no "sample" pill. 30 interface words at rest on the
  desk, 24 on the phone, nothing of 5 words or more. Outside text (film title, channel name, number) carries `data-d`.
  Every part above that shows a second line of words is used without it. `shot.py` prints each breach as `QUIET`.
