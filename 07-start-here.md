# The build — read this first

You are picking up one project. It is not TubeLoop 2.0 and it has no name yet: **a private AI editing
software that turns a channel pack into finished YouTube videos**, so that opening a channel costs almost
nothing and running it costs almost nothing. It is built by Ambi and one builder. Rust is at least 80% of
the code — that is his instruction, not a preference.

Read this, then the brief, then the repo. Do not read the brief cover to cover first; read sections 1–6,
then 21–24, and come back for the rest when a task needs it.

## Where everything is

| Thing | Path | What it is |
|---|---|---|
| **The brief** | `~/AUH/AMBESSA/intel/THE-SOFTWARE-BRIEF.html` | 25 sections, ~91,000 words. The long form. |
| **The library** | `~/AUH/AMBESSA/context-repo/09-assets/library/GALLERY.html` | 104 images, one library, numbered once. |
| **The glossary** | `~/AUH/AMBESSA/GLOSSARY.md` | Canonical. Appended to the brief automatically. |
| **The repo** | `github.com/AmbessaTrades/ambessa-context` | The short form: `00-READ-FIRST.md` → `01-context.txt` → `02-the-software.md`. |
| **The old app** | `~/AUH/Loop` | Read it; do not trust it. `data/loop/lot/wisdom.json` is the lesson store behind brief §16. |
| **The study** | `~/AUH/STUDY/loop-rebuild-2026-11-19/` | Frames, contact sheets, `outliers/channels.jsonl`. |

Ambi will paste two links into the chat: the brief and the gallery. If a link is dead, read the local file
above — it is the same artefact.

## The laws of this project

1. **Nothing is decided unless Ambi says it in conversation.** The brief records what was said and when;
   it does not extend that authority to what it inferred. Write *exploring*, *candidate*, *open question*.
2. **A channel pack is the unit of work, of scale and of billing.** A video is an instance of a pack.
   Three channels are three packs, not three hundred projects. Opening channel eleven is clone-and-swap.
3. **Design systems are onions** — pacing, motion, layout, transitions, data grammar, type, colour,
   emotion — each mapped and versioned separately. A bump needs a hypothesis and a 90-second proof.
4. **The thumbnail is a frame the video contains**, and the title is the sentence that frame cannot say.
5. **Simplify the vibe, never the count.** Never a budget of objects. Every film is art: the test is where
   the viewer's mind goes.
6. **A green metric is not a correct film.** Look at the pixels. A critic that counts and never looks
   passes an empty page.
7. **A public URL is the definition of done.** A plan, a board and a passing suite are not done.
8. **One record, one copy.** One gallery, one glossary, one brief. Never fork them.

## How to work here

- **Before a plan:** `grill-with-docs` (it loads `grilling` and `domain-modeling`). Rounds of at most five
  questions, each with a recommendation, then wait. Write the glossary as terms resolve.
- **Before a document for an agent:** `writing-for-agents`.
- **Before engine code:** `tdd`. Before a multi-session chunk: `wayfinder`.
- **Estimate and verify separately.** Scripts compute; models judge. Every child writes a file, and you
  verify it against the source rather than believing the summary.
- **Report in four beats:** what changed · why it matters · what is open · one next action. No preamble,
  no closers, five visible items maximum.

## The first three tasks, in the order the brief gives them

1. **Freeze and prove one render** from the tree as it stands, before any refactor.
2. **Write the pack schema** (`pack.json`) with versioned onions, three title templates, six moment rules
   and one grade table; two packs must validate, and a pack missing a template must fail to load.
3. **Build the six-moment extractor** — six frames at 1920×1080 from a finished MP4, each hash-matching a
   re-extraction at its stated timecode.

The build order in brief §6 (B0–B8) is the fuller version. It is a recommendation, not a decision; where
it disagrees with §1's "publish first, build only what the publish was blocked on", say so and ask.

## What is closed

Everything that sold intelligence, verification or deal files to governments or to companies doing
$10M–$5B. It is archived at `~/AUH/AMBESSA/_archive-govcon-2026-11-19/` and must not come back. AAY has
nothing to do with this project and appears nowhere in it. LOT is the only channel that exists.
