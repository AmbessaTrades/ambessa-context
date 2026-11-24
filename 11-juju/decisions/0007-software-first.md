> Working document. Subject to change through continued conversation. Nothing here is a requirement until Ambi says so.

# 0007. The software first: no channel is the goal of the build

**Status:** decided by Ambi, 24 Nov 2026: "Stop trying to figure out how to make an LOT video and start trying to figure out how to make the software good." "It is highly unacceptable for our software to only be good at those particular styles. We need to be good at a lot of other things, especially the things that you said is hardest." "If I put any video in there, a faceless video, it will know exactly how to strip it down, wire it up, and make our own version of it in every way [...] everything that VidRush has." The aim he named: 52 minute TV-style films a sixty year old watches on the couch, then the offering. His channels: "assume there is going to be something that you do not expect."

**Decision.** Build order follows measured capability, not a channel or a date. The job that wrote a first LOT film was stopped; its files stay only as test material. The lead no longer recommends channels.

**How capability is measured (the lead's method, under test):** real faceless films are dissected shot by shot (`crates/juju-absorb`, `runs/absorb`); `docs/CAPABILITY-MAP.md` states what share of their screen time Juju can make; the next thing built is whatever raises that share fastest for inner-life films and couch documentaries. Target line: 90 percent.

**Supersedes.** The brief's Wednesday 25 November launch line as a driver of the build, and the lead's "what we will make well" list of 24 Nov (charts, chats, maps first).

**60 day running cost, estimated 24 Nov from live prices, nothing metered:** about $290 US for 150 films (4,800 finished minutes): voice 98, pictures 69, DeepSeek 61, GLM 28, Neon 27, Jev 7. The largest unknown is how many reasoning tokens DeepSeek on max uses per call (assumed 16,000).
