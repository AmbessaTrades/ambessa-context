# Images

`ambessa-saul-profile.png` is the brand portrait, and it is live — a web agent with browsing can
open and see it here:

`https://raw.githubusercontent.com/AmbessaTrades/ambessa-context/main/09-assets/ambessa-saul-profile.png`

Any other image works the same way: put the file in the repo and hand the agent the raw URL. The
agent reads the picture from the link; it cannot read a picture off Ambi's disk.

`manifest.json` lists every image slot in the brief, in order, with the words that precede it so you can tell which is which. To publish a missing image, drop it into `incoming/` named `01.png`, `02.png` and so on, matching the slot number. The next sync publishes it and the raw link becomes:

`https://raw.githubusercontent.com/AmbessaTrades/ambessa-context/main/09-assets/incoming/01.png`
