# Literature curation with Claude Code

- [E] Project to replace manual curation of scientific literature with Claude Code. It has its own folder and git repo. (2026-10-05)
- [E] Their reading of it: they are teaching Claude to do the job like an intern. (2026-10-05)
- [E] Repo: `github.com/pmall/curation`. They describe it as a project that orchestrates a lot of agents in parallel, and a great example of all they think about AI. The point is the AI strategies, not the project. (2026-10-16)
- [O] What the repo shows (read 2026-10-16, not stated by the person): it is the harness in which Claude curates "Drakkar", a database of virus–human protein–protein interactions. Instructions (`AGENTS.md`, `docs/`), tools (Python commands that fetch, convert, check and write), and a `curate` skill that runs batches of up to 20 publications, one subagent per publication, with a dry run and a curator's "go" before any write. Strategies are listed in `ideas/orchestrating-agents-strategies.md`.
- [O] Dates in the repo: first full-text runs 2026-10-14 and 2026-10-15 (runs of 4 and 20 publications); a versioning pass onto UniProt 2026_03 closed 2026-10-08. The repo's own history dir records a move from manual curation to the agent's curation.
- [I] Likely the same line of work as [enyopharma](enyopharma.md) and [bpgraph](bpgraph.md) (virus–human PPI, facts backed by publications), but the person has not said so. Do not state it in content.
- [E] Status (2026-10-16): still benchmarking. They monitor the agent and compare its curation to manually curated data, to bring the number of unsettled cases as low as possible. Their key point is not the benchmark but that monitoring stays possible.
- [E] Real throughput (2026-10-16): still testing, in batches of 20 publications. About 100 publications per 5-hour usage limit, which they put at roughly 10 million tokens. The 1000-in-5-minutes / 100 million tokens figure is math, not something they have run.
- Not yet recorded: when it started, how far it works, how much of the curation is now done by the agent. Ask before using.
- It is an example of a principle, not a subject for writing (see substrate §13), unless they ask.
