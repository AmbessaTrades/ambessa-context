> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

# 0003. Juju has its own private repo, for good

**Status:** decided by Ambi, 24 Nov 2026: "Yes, it needs its own private repo in perpetuity." And: "This is Juju, something completely different" (said when the lead ran the TubeLoop save for it).

**Decision.** `github.com/AmbessaTrades/juju`, private. Juju work is never saved through the TubeLoop backup. The skills live in this repo (`crates/juju-skills/packs`) and are linked into the agent harnesses by `scripts/link-skills.sh`.

**Merging (Ambi left the rule to the lead: "nothing auto merges, but review it so it becomes capable of auto merging; make your own call; I do not want to be bothered").** Every change lands as a pull request. The lead merges after the gate is open and fresh reviewers find nothing that matters. Each merge records whether it later needed a fix. Auto-merge is switched on only after 20 merges in a row needed none. *(The number 20 is the lead's choice.)*
