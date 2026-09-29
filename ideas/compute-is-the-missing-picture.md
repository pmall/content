---
title: AI is a matter of compute, and most people judge one inference
status: growing
created: 2026-09-29
updated: 2026-09-29
related: []
context: []
---

# AI is a matter of compute, and most people judge one inference

## Current understanding
Most people's experience of AI is one inference: ask for a document, judge
its quality. But one output is a single draw from a stochastic process, one
document out of an infinity the system could produce. Given computing power
("x unit of energy = y units of intelligence"), AI can produce thousands of
candidates, evaluate and rank them, and mix the good ideas: the "diamond
pattern" (fan out, then converge).

The same logic applies to exploration. A single agent run exploring a space
of hypotheses loses track of them, and which ones it picks is stochastic.
Fix: an orchestrator spawning X subagents, one per hypothesis. The larger X,
the more exhaustive the exploration, so exhaustiveness becomes a matter of
energy. The person's claim is that people miss this full picture.

The graph database exploration was where it came up. It is only an example.

## Open threads
- Evaluation: the person says agents rank the candidates ("the agent, obviously", esp. in biology) and doesn't see it as a problem. A reader may. Decide in the writing whether to address it.
- Cost and diversity: do X subagents actually explore different hypotheses, or the same ones?
- A concrete case, outside bioinformatics, that a reader can follow.
- Level: concepts, not implementation. No orchestration how-to.
- Their own words for the pattern: "the diamond pattern". Keep it.

## Raw drops
### 2026-09-29
> we dont care what graph it is. I dont want to center my content around my bioinformatics projects, they are only examples. What i think is what most people are missing is the ai can continuously work given computing power. x unit of energy = y units of intelligence. Current experience of most people is to ask to write a document and evaluate que quality of this one inference. But this is still a stochastic proccess. This is one document out of infinity of documents the system can produce. But they miss that given computing power, the ai could build a thousands documents and evaluate them and rank them and mix the good ideas. The diamond pattern. Thats what im facing with exploring my graph: one run of opus will inspect multiple hypotheses randomly. So 1 it might loose track through multiple hypotheses and 2 the choice of hypothesis to explore is stochastic. Solving this would be 1 orchestrator agent spawning X subagents, 1 agent per hypotheses. The greater the X the more exhaustive we are. And the point is this is only a matter of energy/computing power. People dont see this full picture

### 2026-09-29 (later)
> the agent, obviously. especially on biology. For a first try, one agent orchestrates, spawn a swarm and collect results. But still this is not the point. I care about concepts, not implementation
