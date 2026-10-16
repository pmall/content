---
title: Human work is compressed, time becomes a parameter
status: raw
created: 2026-10-16
updated: 2026-10-16
related: [compute-is-the-missing-picture, less-between-data-and-result, orchestrating-agents-strategies]
context: [literature-curation]
---

# Human work is compressed, time becomes a parameter

## Current understanding
What the person is realizing concretely from the curation project (their
numbers, firsthand, not checked against the repo): if one publication is
curated in 5 minutes for 100k tokens, nothing prevents running 1000 agents
in parallel to curate 1000 publications in 5 minutes, for 100 million
tokens. It does not matter whether those 100 million tokens are spent over
6 months or in 5 minutes: the cost is the same, the time is not. Infrastructure
costs and limits for running 1000 agents at once exist, but they see them as
secondary to the big idea.

Their conclusion: **human work is compressed.** The duration of a body of
work stops being fixed by how long it takes one worker. It becomes
something you choose, within infrastructure limits, by how much you
parallelize.

This is the compute thesis (`compute-is-the-missing-picture`) shown on a
real, ordinary task: tokens are the unit, and parallelism trades time for
nothing but infrastructure. It also echoes the "training room where 1000
years pass in 1 second" image they gave there (their link to confirm, not
stated here).

## Open threads
- Per-publication figures (5 min, 100k tokens) are the person's own, not
  recorded in the repo. Confirm they stand before using them as numbers in
  content.
- What stops compression in practice? They name infrastructure costs and
  limits; not detailed.
- Tension to look at, not resolve: compression makes the work arrive faster
  than a human can look at it. This touches their key point that monitoring
  stays possible (`orchestrating-agents-strategies`). How does monitoring
  work for 1000 publications in 5 minutes? Their words needed.
- Which kinds of work compress this way? The example is work that splits
  into independent units (one publication each). Not said whether they see
  limits for work that doesn't split.
- Title candidate from the person (2026-10-16): "The day I spent 100 million
  tokens" (as typed: "tha day i spent 100 millions tokens"). Their phrasing
  for the idea: "Human work is compressed". The title is first-person and
  matches the 100 million figure above. Clarified 2026-10-16: they have
  NOT run the 1000-publication batch, it's math they worked out. The
  title can't be a firsthand story as is: either a projection framing
  ("the day I could spend…"), a hypothetical, or wait until they actually
  do it.
  Real numbers so far (2026-10-16): batches of 20, ~100 publications per
  5h usage limit, so "the day I used 10 million tokens" would be true. They
  find it less impactful ("lol"). Possible angle, not theirs: the true 10M
  day as the opening, the 100M math as where it goes.
  Their next step (2026-10-16): with 10 such subscriptions, 1000
  publications in one 5h window. So the limit is bought, not technical:
  compression scales with what you pay for. Math, not done.

## Raw drops
### 2026-10-16
> what im realizing concretely is that, if i can curate 1 publication in 5min and it cost 100k tokens. Then, nothing prevents me to run 1000 agents in parallel to curate 1000 publications in 5min, for 100 millions tokens. It does not matter if the 100 millions tokens are used over the course of 6 months or in 5min. There are some infrastructure costs and limits to run 1000 agents in parallel of course but this is the big idea. Human work is compressed

### 2026-10-16 (title)
> I also like the title "tha day i spent 100 millions tokens"

### 2026-10-16 (clarification)
> its just the math i worked out

### 2026-10-16 (real numbers)
> Curently im still testing, im going to batches of 20 publciations. I can reasonably curate 100 publications per 5h usage limit. So its more like the day i used 10 millions tokens but this is less impactfull lol

### 2026-10-16 (subscriptions)
> had i 10 subscriptions like this i could do my 1000 publications in a 5h laps
