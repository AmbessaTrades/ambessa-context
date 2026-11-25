<!-- copied from the Juju repo: runs/taste/PANEL.md, last changed 22:57 EAT, 24 Nov 2026. Private lines removed. Do not edit here. -->
# The taste panel

> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.
> 24 Nov 2026, 19:06 to 22:00 EAT. Every count is Measured, from `proof.json`, unless it says otherwise.

```
python3 scripts/taste.py <strip.mp4> <map|space|essay|archive> [--script the-films-own-words.txt] [--against N] [--writer google,deepseek]
```
One JSON verdict on stdout: `win`, `tie` or `lose` against a published strip of the same kind, with reasons, seconds, the seats that
voted and one `next_repair`. A strip is 55 to 95 s. Exit 3 and `short`: fewer than three seats could be read, which is not a verdict.
A packet already made of the same file and length is used again (`same_pack`). Full record of each run: `runs/taste/verdicts/`. No Claude in it. Always pass `--script`: it is free, and it is the only sure check of line order.

## How it judges
1. `pack.py` makes the same blind packet of both strips: 12 frames at equal spacing (480x270, two sheets, no label), the words with their
   times heard by one machine (faster-whisper small.en, from the sound itself), picture change and loudness for each second, and
   Earshot's hints. No title, path, logo or file tag goes in. Logos and captions inside the picture stay.
2. Each seat looks twice, order swapped, and answers A or B to four questions (a person chose it; keep watching at 10, 30, 60 s), then
   gives each strip one second and one reason. A seat that changes side with the order counts 0.
3. Votes are +1, 0, -1. Sum of 2 or more is `win`, -2 or less is `lose`, else `tie`.
4. **Cap.** "Held too long" or "sound missing", named by two seats within 6 s and confirmed by the packet's own numbers (picture still
   10 s or more, sound under -50 dB for 3 s or more), makes it `lose` whatever the votes. So does a line the script shows out of place.
   `judged` keeps what the votes said; `capped_by` says why.

Seats that vote: glm-flash (z-ai), jev (TypeSafe), qwen (Alibaba), deepseek. A seat of the writer's family sits out, so today
(Neon and DeepSeek write) **three seats of three families vote: glm-flash, jev, qwen.**
Removed by the key: gemini-3.5-flash-lite (chose slot A 74 percent of the time) and gpt-6-luna (27 percent).

## The four proofs
| Proof | Asked | Result |
|---|---|---|
| a published v published, 12 pairs | near even | four seats 4 win 5 tie 3 lose: **passes the key** (2 to 7 each way). **Today's three seats 4 win 6 tie 1 lose 1 short: fails it** (too few losses). Ties are half, so "win or tie" is a low bar for the 19 of 20 count: report wins and ties apart |
| b our film with no sound, 3 pairs | must lose | lost **3 of 3** |
| c planted faults, 12 | two seats, right reason | freeze 4 of 4, cut sound 4 of 4, **shuffle 0 of 4** in the pair look, 3 of 4 by the words check: **fails the key** (11 of 12). That 3 of 4 came after one rule change on the same plants (first and last line not counted, token ceilings); the 13 fresh shuffles below are the honest count |
| d same pair twice, 6 | agree | same verdict **5 of 6**; single answers the same 161 of 188 |

Held out, strips no seat or rule had seen (`key-held.json`, written first):
- words check on 13 fresh shuffles: two seats named the moved line 7 of 13, it fired on 10 of 13, and on 0 of 13 clean. **Fails its key.**
- pair look on one fresh host: freeze named by two (jev, deepseek), cut sound by four; but three seats also said "sound missing" of the clean
  host (a stretch with no narrator, quiet, not silent). **Fails its key**; this is why the cap needs the numbers to agree.
- with today's three seats that fresh freeze was named by jev alone.

What was built after those fails, both free:
- the film's own script against what is heard (`--script`, no model): **18 of 18** shuffles found (5 in real sound, 13 in words), 0 false on 10 strips heard
  again (there the script is the clean strip as heard). On two real scripts of ours read in order, which repeat "became an independent state":
  0 of 360 good strips flagged with 0, 1 or 2 words wrong in each line; swaps found 120, 118 and 91 of 120 (`script-garble.json`).
  The first version flagged 17 and 7 good strips of 120 and was replaced. Not tested on a real voice of ours: see the last table.
- the measured cap, today's three seats: freeze 4 of 5, cut sound 5 of 5, our no-sound film 3 of 3, clean published **0 of 44** showings
  (1 of 44 if deepseek sits too). The 10 s and 3 s numbers were set on these same strips.

## Good for
- Refusing a strip with dead sound, a frozen picture or moved lines, with the second and the repair.
- A like for like vote on a 60 s strip that is mostly the same when asked twice.

## Cannot see
- **Liking hardly moves with a fault.** A 15 s freeze lowered the score on 4 of 4 hosts but by 1 to 10 points of 32, and changed the voted verdict on 1 of 4;
  cut sound changed it on 2 of 4. Seats prefer a film, not its state. Without the cap a broken copy of a strong film still wins.
- **The seats read numbers more than pictures.** Freeze and cut sound are written in the packet as numbers. Naming them proves reading, not taste.
- **No proof covers a voiced strip that is smooth and robotic.** Flat voice, same move again, generic line, wrong scale and text on busy picture
  were never planted. They are printed with `proved: false` and how often clean published strips got the same reason (held too long 5 of 24,
  sound not from anything seen 5 of 24, number not shown 3 of 24). Treat them as a hint.
- It hears no voice: only words, loudness and tags. Acting, tone, accent and a bad read are outside it. Between the 12 frames it sees only how much changed.
- Published loses to published 3 of 12 (today's three seats: 1 of 12, one short), and "even" is the count over the list, not a coin: the panel
  has favourites. oRB beat pUZ 3 of 3, J0w beat MVI 2 of 2, sJi beat Zgp 4 seats to 0. So **which opponent is drawn decides a lot**; a count of
  strips should use `--against 3` (a third of the luck, three times the cost), and 19 of 20 says what happened 20 times.
- Same model families may share a taste. One person's watch (ADR 0019 point 4c) is not replaced.

## Cost and time
About **0.006 US** a verdict against one published strip (6 looks and 2 words checks; see the runs below), 0.0005 to 0.0012 a look. The packet of our strip is
about a minute of Earshot under `scripts/heavy`; then about 20 to 60 s of calls. Published packets are already on disk.
`--against 3` triples the calls. **On a busy Mac make the packets first**, all strips in one list, one wait in the queue: write `[{"id","src" (full path),"start":0,"dur" (whole seconds, at most 90; 60 to 66 becomes 63 or less),"kind"}]` to a file, run `scripts/heavy .toolchain/earshot/venv/bin/python runs/taste/pack.py <file>`, then `taste.py` uses them. A length that is not 60 to 66 s also needs the published strips cut again to that length. Anything that stops it (money, file, packet) prints `{"verdict":"refused","why"}` and exits 2. The tool refuses past `TASTE_LIMIT_USD` over all `taste` rows in the ledger (default 0.60, the limit of the job that built it,
of which almost all is spent): **a lane that judges 20 strips sets `TASTE_LIMIT_USD` to what is spent plus about 0.20, under its own paid limit.** The shared cap holds on top.

## One losing reason, one repair
| Reason | Repair | Trust |
|---|---|---|
| sound missing | mix: find why the track is empty at this second, mix again | proved when measured |
| held too long | shots: add one change inside this hold, at the word nearest the second | proved when measured |
| lines out of order | words: put this line where its own before and after ask for it, time again | proved with `--script`; two seats fired on 0 of 13 clean |
| picture late | shots: move this beat's picture change to 2.5 s before its naming noun (ADR 0014.11) | hint |
| no pause | timing: 1.3 s before the turn, 3.0 s at a chapter, at this second | hint |
| number not shown | shots: show the spoken token, equal to the word, at this second (0014.8) | hint |
| text on busy picture | layout: type to its own plain ground on the empty side (0014.5) | hint |
| same move again | shots: give this beat another layout or move than the one before | hint |
| flat voice | voice: say this one line again with another direction | hint |
| sound not from anything seen | mix: take out the cue nearest this second | hint |
| generic line | words: cut this line, or put one checked fact in its place | hint |
| wrong scale | camera: reframe this beat so the thing named fills the frame it needs | hint |

"Sound missing" and "lines out of order" were added to the kickoff's ten: its own plants (cut sound, shuffled lines) have no right answer among the ten.
Use: take `next_repair` only, make that one change, run again. If it says `proved: false`, look at that second yourself first.

## The published shelf (`shelf.json`, 19 strips of 63 s, 7 films; `runs/teardown/HmuQoak_IAg`, `runs/teardown/G4w-a8NgnnQ` have no film)
map: J0w x3 (`runs/scout/atticus`), MVI x1. space: oRB x3, pUZ x2. essay: Zgp x4, sJi x3. archive: sJi x3, IEW x3.
Missing: `runs/craft`, `runs/skeleton`, `runs/atlas` hold no moving picture at all; `runs/rip/donors/G4w-a8NgnnQ.f299.mp4` has no sound. `runs/scout/v/Vx5AbTUxvTQ` (picture and sound) is not on the shelf.
Two or three films a kind is thin: a channel's own look can win every time. sJi serves two kinds.

## Runs on our own strips
| Strip | Verdict | What it said |
|---|---|---|
| `runs/spine/20261124-171717-1e01/master.mp4`, map, against MVI | lose (glm-flash 0, jev -1, qwen -1) | two seats: a sound that belongs to nothing seen, 13 s (hint). It has a steady bed and no voice at all: 0 words heard. 24 s, 0.0048 US |
| `runs/spine/20261124-174132-02c4/film/film.mp4`, map, against MVI (proof b's film) | lose 3 seats to 0, capped | sound missing 0 to 63 s, proved. 49 s, 0.0054 US |
| `runs/taste/strips/ours-map-02c4-voiced.mp4`, map, fresh packet, against J0w-400 | **tie** (glm-flash -1, jev +1, qwen +1; ours was preferred by two) | two seats: a sound that belongs to nothing seen, 60 s (hint). Script check on the real voice: no line wrongly called moved. 26 s, 0.0062 US |

**A warning in that last row (Judged by the maker's eye).** Its script says "became independent" or "an independent state" eight times, holds the same slow drift on every
map, and prints the year over land. Two seats of three still preferred it. No seat said "generic line", one said "same move again". So a tie from this panel does not mean
the strip does not feel robotic: the panel refuses broken strips, and has not been shown to see dull ones. Next proof to run: plants for flat voice, same move and generic line.
The packet needs the heavy queue: it waited 41 minutes on 24 Nov (pool changed to 8 slots at 22:45, shorter since); the judging itself took 26 to 49 s.
