# ADR 0020: one unit, one pull request, one round

Decided 24 Nov 2026, 22:00. Ambi: "Why do we keep shoving everything in pull request 11? Instead of starting new PRs, new PRs, new PRs,
for different things ... check merge, go check merge, go check merge go or just whatever architecture you think is best ... do what you
see fit for the best for Juju." What went wrong: PR 11 took five rounds because each round's findings, some of them wordings, were
pushed into the same pull request, and every push cleared both reviews and started 13 minutes of checks again.

1. A pull request holds one unit, from `main`, opened the moment the unit's own check passes. Nothing is added to it after that.
2. Two reviewers start at the same time on that head, once, and record a verdict with `scripts/pr_state.py review`. Each finding is
   **block** (wrong result, hang, lost work or money, a leaked secret, a loosened gate), **fix** or **note**. Only a block is FINDINGS.
   A fix or a note is CLEAN with the list kept in `runs/pr/NEXT.md`, and the next pull request carries it.
3. A block gets one repair in the same pull request and one recheck of the changed lines by the same two names. A second block closes
   the pull request and the unit starts again smaller.
4. Clean and green merges at once, in the order they turn green, never by number. A pull request waits for another only when it needs
   its code.
5. Integration branches end when pull request 10 lands. After that every lane's maker opens its own pull request at the end of its
   lane; a lane is not done while its work is only on this Mac.
6. Unchanged: two reviewers who did not write it, green checks at that head, the lead's word on a gate change, no loosened threshold.
