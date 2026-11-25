# How this repo stays true

`com.auh.juju-context`, a job on Ambi's Mac, runs every two hours: `sync_context_repo.py --haiku`.

1. **Code collects**: jobs and agents from the live workshop page, pull requests, commits, the paid-call ledger, crate and room counts, new
   decisions, changed design pages, Juju entries of the day log, new pictures, every film run, every logged attempt, the exit check.
2. **Haiku 5.5 (medium)** gets those facts and the lead agent's own messages, and writes the sheet in `10-now/`. It has no tools and reads nothing else.
   Ambi's messages are never read by this job.
3. **Code cleans and checks**: private lines are dropped, then every text file in the repo is read. One key, email, private detail or local path
   and the push is refused.
4. It commits and pushes. If the Mac sleeps, the next sheet is late: check the stamp. **It was down from 24 Nov 13:52 to 25 Nov 08:20** (a date format one Python could not read). Fixed; a crash now writes to the day log.

| Rebuilt by the job | Written by hand |
|---|---|
| `01-context.txt`, `10-now/*`, `08-journal/recent.md`, `11-juju/decisions/*`, `11-juju/skills.md`, the copied design pages (each says so in line 1), `09-assets/live/*`, `GALLERY.html`, `LIBRARY.md`, `index.json` | Everything else. Each hand-written page carries its own time. |
