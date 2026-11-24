> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

# 0001. Earshot's listening models may live on the Mac

**Status:** accepted by Ambi, 24 Nov 2026, in conversation: "all aspects of earshot are important to use [...] Earshot can also create its own sound effects, and that's extremely crucial to not get those weird AI 2-bit sounding effects".

**Context.** The brief bans every local AI weight to protect 16 GB of memory. Earshot can make sounds with no model, but building new effects well and rejecting fake ones needs its two listening models (about 2.2 GB on disk, CPU).

**Decision.** One named exception to the ban. The models judge sound; they never generate it. Local LLMs and local speech stay banned.

**Considered.** Catalogue-only Earshot (no models): rejected, because nothing would hear the result before it reached a film.

**Consequences.** Superseded the same morning: an earlier version of this file said the phone only plays sounds the Mac made. That was the builder's inference and Ambi overruled it: "for the APK version, it needs to somehow use earshot as well, independent of my computer." So Earshot must run on the phone with the Mac off.

**How, on the phone: candidate, not decided** (spike of 24 Nov, `docs/earshot-phone-spike.md`; every number is from the Mac, nothing has run on a phone yet).

- Candidate: embed Python in the app with Chaquopy and run Earshot's own code, with its 28 speed loops (570 lines) rewritten as one small Rust library. Android arm64 builds of numpy, scipy, soundfile and soxr exist for Python 3.13.
- Measured: without the speed loops 879 of 922 sounds came out byte-identical; a short sound takes under 0.4 s, a 20 s rain loop 48.8 s (3.8 s with four loops in Rust).
- Measured: the listening models are 1.12 GB on disk, not the 2.2 GB the README says. A phone set of 420 MB matched the Mac models on 18 of 18 clips.
- Estimated: about 85 MB added to the APK, 420 MB of models as a side file, 11 to 16 working days.
- Unproven link, to test first: a throwaway APK that makes one sound through Chaquopy and plays it.

**Still open (inferred, not said).** Load the models per job and exit; never beside a render; the pass mark for a sound (the skill writer measured a clean learned page turn at z 2.8, under the brief's candidate 3.0).
