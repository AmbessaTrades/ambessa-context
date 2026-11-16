# How this pack is kept current

Generated and pushed by `~/AUH/AMBESSA/sync_context_repo.py`, on a schedule. Every run rebuilds
the generated files, rewrites `index.json`, and commits only when something actually changed.

## Generated on every sync (do not edit these by hand)

| Path | Comes from |
|---|---|
| `02-goals/mission.md` | Memoir topic `mission` |
| `01-who/north-star.md`, `founder-authority.md`, `calm-room.md` | Memoir topics of the same names |
| `01-who/mental-models-memoir.md` | Memoir topic `mental-models` |
| `01-who/systems-thinking.md` | Memoir topic `causal-thinking` |
| `04-market/evidence/confidence.md` | Memoir topic `evidence` |
| `04-market/thread-log.md` | Memoir topic `afribbean` — the running Africa-Caribbean log |
| `07-agents/agents-and-harnesses.md`, `bot-contract.md`, `context-as-a-packet.md` | Memoir topics |
| `03-the-brief/the-brief.md` | Ambi's founding brief, verbatim, contact details removed |
| `04-market/evidence/findings.csv` | the verified pain base, from `pains.db` |
| `04-market/evidence/README.md` | row count and the rules for using it |
| `08-journal/recent.md` | last 21 days of the day log |
| `08-journal/summaries.md` | last three generated summaries |
| `09-assets/manifest.json` | image slots in the brief, plus whatever was dropped in `incoming/` |
| `index.json` | machine index of every file |

## Written once, kept by hand

`README.md`, `00-READ-FIRST.md`, `01-who/identity.md`, `01-who/mental-models.md`,
`02-goals/money.md`, `03-the-brief/directives.md`, `04-market/pain-map.md`,
`04-market/market-answers.md`, `04-market/competitive-map.md`, `05-offers/offer-set.md`,
`05-offers/hypotheses.md`, `06-playbook/search.md`, `06-playbook/content.md`, this file.

The sync never overwrites these.

## Deliberately left out

- Every project that is not this business: the language app, the studio, the video tools, the
  maps, the old channels. They are history, not context.
- Credentials, keys, tokens, and any file containing them. A file that fails the secret check
  is skipped rather than redacted.
- Email addresses and phone numbers, which are stripped from every file on the way in.
- Private personal details and family connections, which stay on the machine.

## Run it by hand

```
python3 ~/AUH/AMBESSA/sync_context_repo.py            # rebuild, commit, push
python3 ~/AUH/AMBESSA/sync_context_repo.py --dry      # show what would change
python3 ~/AUH/AMBESSA/sync_context_repo.py --no-push  # commit locally only
```

## Read it from anywhere

Raw file, no account needed:

```
https://raw.githubusercontent.com/AmbessaTrades/ambessa-context/main/<path>
```
