<!-- copied from the Juju repo: docs/poteto/hillclimb.md, last changed 19:38 EAT, 24 Nov 2026. Private lines removed. Do not edit here. -->
# Hillclimb: one change, one measurement, keep or revert

For improving one number over many attempts: render seconds per film second, a blind judge's catch rate, a fault count,
a script's defect count. A single bug with a repro is a bug fix, not a hillclimb.
Source: pstack Hillclimb playbook, read 24 Nov 2026.

1. **Ground it.** Name the real workload that shows the complaint (which film, which room, which Mac load). If no case
   reproduces the complaint, fix the repro first. Done when one command shows the bad number.
2. **Fix the metric and the stop rule.** One number, which direction is better, a target, and a floor on attempts so a
   lucky first try cannot end the run. Example: "at most 1.0 s of work per film second, and at least 5 attempts".
3. **Build the harness, prove it can tell good from bad, then freeze it.** Run it on a known easy case and a known hard
   case. If it cannot separate them, change the harness. It prints its error count and a count of work done. Take the
   median of three runs. From here the harness is read-only.
4. **Record the baseline** and a gate run before any change: `scripts/decide <lane> baseline none <n> <n> kept <evidence>`.
5. **Loop.** Before each attempt run `scripts/decide --tail <lane>` and read it.
   - State one hypothesis that names a mechanism: "scene prep waits on one thread, so split it across four".
     "Try caching" is not a hypothesis.
   - Make that one change. Touch as few files as it needs.
   - Measure with the frozen harness. Run `scripts/gate.sh` if code changed.
   - Keep it only if the number moved past noise and the gate is open. Then one commit with only your files.
   - Otherwise restore every file you touched and delete what you added. A change that "might help" is reverted.
   - Log the row either way.
6. **On a stall,** three reverts in a row: change category, combine two near misses, reread the source, or try the
   radical version. Two fixes on one premise failed: write the premise down and test it directly.
7. **Correctness beats the number.** Revert a win that breaks behaviour. Keep a simplification that holds the number.
8. **Stop** when the stop rule is met, or when the ideas left cost more than they could gain. Say which.

Report: metric and target, baseline to final with the percent, attempts kept and reverted, each kept change in one
line, the best untried idea.
