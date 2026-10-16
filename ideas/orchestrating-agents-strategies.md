---
title: Strategies for orchestrating many agents, seen in the curation project
status: raw
created: 2026-10-16
updated: 2026-10-16
related: [compute-is-the-missing-picture, agent-gets-an-environment, less-between-data-and-result]
context: [literature-curation]
---

# Strategies for orchestrating many agents, seen in the curation project

## Current understanding
The person built a project that orchestrates many agents in parallel
(`github.com/pmall/curation`, see `context/literature-curation.md`) and
considers it "a great example of all I think about AI". The project itself is
not the point: the point is the AI strategies used in it. They had the agent
read the repo to catch the idea.

What follows is the agent's reading of the repo, not the person's words. It
is a list of strategies to confirm or correct, not yet a thesis:

1. **Fan out, one context per unit of work.** An orchestrator hands each
   publication to its own subagent (up to 20 per batch). The orchestrator
   never reads the publications itself. This is the "diamond pattern" and
   "1 agent per hypothesis" from `compute-is-the-missing-picture`, in
   production. Batches are independent and could run in parallel.
2. **The agent decides, deterministic tools check.** Agents write files;
   code checks them against the whole database; values that can be computed
   (coordinates, names, mappings) are computed by the tools, never given by
   the agent. Judgment goes to the model, verification goes to code.
3. **A dry run is the same code as the commit.** It runs the real write in
   a transaction and rolls back, so the human reviews what would happen, not
   a description of it.
4. **Human gate before anything is written.** The agent curates, the curator
   supervises: nothing reaches the database before a "go" on a report.
   Every version is kept, so no write is irreversible and a publication can
   always be curated again.
5. **Saying "unsettled" is a valid answer.** A case the agent cannot settle
   is reported with why, never guessed. "Unsettled is better than wrong."
   Those cases are routed to a manual pass.
6. **Independent second pass.** Re-curation is done from the full text
   without looking at the current curation, then diffed against it. The
   comparison, not the agent's memory, finds what changed.
7. **Instructions live in files, written once.** Rules in `docs/`, each
   process in a skill that points to the docs, a glossary with one meaning
   per term, and an `AGENTS.md` that also encodes how the person wants to
   work with the agent (agree the plan before any analysis, one decision at a
   time, counts only from fresh queries). This is "teaching an intern",
   made concrete.
8. **The environment learns from real use.** What the tools meet on real
   publications (failed fetches, bad conversions) goes into dated logs, to
   improve the tools. Every decision is traceable in a note without the
   conversation that took it.
9. **Prepare the inputs before the swarm.** Full texts are fetched and
   converted first, by tools, so subagents never download anything and
   spend their context on judgment only.

Clarification (2026-10-16): the key point is that **monitoring stays
possible**, not that it is a stage to get past. The design keeps the human
able to look at what the agent did and decide (reports, dry run, go, notes,
kept versions) however good the agent gets. Separately, the person is
benchmarking now: they reduce the "unsettled" cases by comparing Claude's
curation to manually curated data (the earlier manual curation is the
reference), which is why they are monitoring closely at the moment. That is
a tenth element, **measure the agent against a human ground truth**, but it
is secondary to the key point. My earlier reading of the supervision as a
temporary stage was wrong.

Fractal design, constrained by the tool (2026-10-16): the project's result
files are made to work like a fractal (the person's words). In the repo,
each publication directory holds the same kinds of files as the batch
directory, and the batch files are the concatenation of the publication
ones, so a level above could merge batches the same way. But Claude Code
allows only one level, per the person: the main agent spawns subagents, and
those subagents cannot spawn their own. So the swarm in this project is one
fractal level deep, by tool limit, not by design (links to the fractal
picture in `agent-gets-an-environment`). Their firsthand statement; not
checked against Claude Code's documentation.

## Open threads
- Which of these does the person see as the core? Ask them, or wait for a
  drop. The list is the agent's reading and may overweight the engineering.
- Tension to look at, not resolve: in `compute-is-the-missing-picture` the
  person says "the agent, obviously" ranks and evaluates candidates, and
  sees that as no problem. In this project a human go and deterministic
  checks stand between the agent and the database. Answered (2026-10-16):
  the point is not who evaluates but that monitoring stays possible. The
  agent can evaluate; the human can always look. Not yet said: what makes
  monitoring possible in concept terms (traceability, reversibility,
  reports a human can read?).
- What does the benchmark measure exactly (agreement with manual curation,
  per description? per publication?), and how low does "unsettled" need to
  go? Not said. Secondary to the monitoring point. The repo has no benchmark doc yet; its `todo.md` lists
  re-curation of test publications as the next step.
- Link to `less-between-data-and-result`: this project is a case of
  presenting data and rules so an agent can work, and formulating the
  result wanted.
- What would a deeper fractal buy them (batches of batches, a coordinator
  per run)? Not said.
- Level: the person cares about concepts, not implementation. Whatever is
  retained must be said as concepts a non-expert decision-maker can follow.
- Which strategy would make a reader "click"? Candidate from the list:
  "the agent decides, code verifies".
- Title candidate: none given.

## Raw drops
### 2026-10-16
> i made a project that orchestrate a lot of agent in parallel. I think it is a great example of all i think about ai. Do you want to read the git repo to catch the idea?

### 2026-10-16 (repo)
> https://github.com/pmall/curation - the point is not the exact project but the ai strategies i used

### 2026-10-16 (benchmark)
> im still monitoring because im still benchmarking it. I want to reduce the unsettled ones to the lowest possible by comparing claude curation to manually curated data.

### 2026-10-16 (fractal limit)
> yes the result files are made to work like a fractal, but claude code allows only one lever, the main agent spawning subagents

### 2026-10-16 (correction)
> This is not the key point. They key point is monitoring stays possible
