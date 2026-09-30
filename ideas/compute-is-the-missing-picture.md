---
title: AI is a matter of compute, and most people judge one inference
status: growing
created: 2026-09-29
updated: 2026-09-30
related: [less-between-data-and-result]
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

Two themes, in the person's framing (2026-09-30):
1. What is misleading: judging one inference of a stochastic process.
2. Energy as the source of intelligence. Results are a byproduct of
   intelligence, so production can go on indefinitely, and working
   indefinitely means being more exhaustive when exploring the stochastic
   space. The diamond pattern is one example of being exhaustive, not the
   idea itself. The energy point is not well defined yet, and it is the
   part people don't see.

Intended reader (2026-09-30): people whose only AI experience is something
like Copilot writing work emails, who could get a glimpse of the bigger
picture. No fixed takeaway; the hope is a glimpse, not a lesson.

Grounding in current events, per the person: the diamond pattern is not
hypothetical, they say OpenAI solved Navier-Stokes this way, with 10k agents
working on the maths problem. Checked 2026-09-30, see "Research" below. The person
doesn't care whether the proof holds. What matters to them is how the agents
were used: many agents on one job.

Development of theme 2 (2026-09-30): what made it click recently is a model
producing something, reading its own result, evaluating it and correcting
it (their evidence: the "I'm Upping My P(doom)" music video, animated in
JavaScript and made with Opus 5.5, which they read as the model
understanding 2D spatial geometry). Given unlimited energy, a model that can
produce, evaluate and correct in a loop can in principle work on any
problem. They see this loop as closer to intelligence than getting it right
the first time. The model can trial-and-error indefinitely, and train
indefinitely, which fits "it's all a matter of compute". Image they
associate with it: a manga training room where 1000 years pass inside while
1 second passes outside (manga not identified by the person).
Second variable, speed: an unbounded loop is useless if it never finishes.
The faster the model, the more self-correction loops fit in a given time,
so what matters alongside energy is speed. (The training room image fits:
time compressed, 1000 years inside for 1 second outside.)
This also moves the evaluation question: for them, evaluate-and-correct is
the core capability, not a weak point.

The graph database exploration was where it came up. It is only an example.

## Open threads
- Title candidate from the person: "Leveraging infinity". French: "Exploiter l'infini" (their pick, 2026-09-30: "sounds very cool").
- Energy and speed together: loops per unit of time. How to say it plainly for a non-expert.
- Re-check the Navier-Stokes details against the primary source (openai.com blocked our fetch, 403) before publishing. Numbers differ between outlets.
- Define the energy point: energy -> intelligence -> results as a byproduct, working indefinitely. Not well defined yet, in the person's own words.
- One post or two? Theme 1 (misleading) is the proposed opening; theme 2 (energy) may be separate.
- Evaluation: the person says agents rank the candidates ("the agent, obviously", esp. in biology) and doesn't see it as a problem. A reader may. Decide in the writing whether to address it.
- Cost and diversity: do X subagents actually explore different hypotheses, or the same ones?
- A concrete case, outside bioinformatics, that a reader can follow.
- Level: concepts, not implementation. No orchestration how-to.
- Their own words for the pattern: "the diamond pattern". Keep it.

## Research (external, not personal perspective)
Checked 2026-09-30 via web search, plus a fetch of the Quanta article. The
OpenAI primary page returned 403 and was not read.
- Claim confirmed as reported: OpenAI announced (early Sept 2026) that a swarm of ~10,000 concurrent agents found a proof in ~88 hours of a finite-time singularity for 3D Navier-Stokes. Formalized in Lean by another model in ~17 more hours. Sources: [Quanta](https://www.quantamagazine.org/ai-has-solved-one-of-maths-1-million-millennium-prize-problems-20260908/), [CNBC](https://www.cnbc.com/2026/09/09/openai-navier-stokes-math-problem-solved.html).
- Shape matches the diamond pattern: different groups of agents got different versions of the problem, and Codex consolidated useful ideas between groups (search summaries). Quanta describes a hierarchy: ~100 agents on Euler variants for ~50 h, then ~10,000 on Navier-Stokes.
- Caveats (background only, the post is not a scientific review and should not litigate them): it is the *forced* version (smooth forcing), not the unforced problem the Millennium prize is about (per Quanta and an arXiv title). OpenAI is not claiming the $1M prize. Mathematicians still need to check the Lean statement matches the intended problem. Not independently verified. Human groundwork (Córdoba, Martínez-Zoroa, credited by Fefferman) was essential. VentureBeat raised that it can't rule out benefiting from a researcher's private Codex data.
- Numbers disagree: ~2.7M messages (search summary) vs "almost 5 million" (Quanta). Cost: several million dollars (Quanta).
- The person uses this only as an example of the *method* (many agents, one job), not of the result. Still say "reported", never "solved". "OpenAI solved Navier-Stokes" is too strong as written. Safe wording: "reported a proof of a forced version, formally checked in Lean, using ~10,000 agents".

- Video: [P(doom) music video source](https://github.com/neoneye/PDoomVideo). Exists as a Claude Opus 5.5 music video, painted animation rendered from code (p5.brush). That the model reads its rendered result and corrects it is the person's own firsthand observation, stated as such; no source needed. Parallel subagents in the project are irrelevant to their point.

## Raw drops
### 2026-09-29
> we dont care what graph it is. I dont want to center my content around my bioinformatics projects, they are only examples. What i think is what most people are missing is the ai can continuously work given computing power. x unit of energy = y units of intelligence. Current experience of most people is to ask to write a document and evaluate que quality of this one inference. But this is still a stochastic proccess. This is one document out of infinity of documents the system can produce. But they miss that given computing power, the ai could build a thousands documents and evaluate them and rank them and mix the good ideas. The diamond pattern. Thats what im facing with exploring my graph: one run of opus will inspect multiple hypotheses randomly. So 1 it might loose track through multiple hypotheses and 2 the choice of hypothesis to explore is stochastic. Solving this would be 1 orchestrator agent spawning X subagents, 1 agent per hypotheses. The greater the X the more exhaustive we are. And the point is this is only a matter of energy/computing power. People dont see this full picture

### 2026-09-29 (later)
> the agent, obviously. especially on biology. For a first try, one agent orchestrates, spawn a swarm and collect results. But still this is not the point. I care about concepts, not implementation

### 2026-09-30
> i would start by what is misleading. And there is two different things following the diamond pattern, which is an example of how to be exhaustive on this stochastic process. The energy point is not well defined. This is what people dont see yet. As intelligence, and then result production is only a byproduct of energy, its possible to produce infinitely. Working infinitely means we can be more exhaustive while exploring stochasticity. There are two themes i guess

### 2026-09-30 (later)
> I dont know what a reader must keep. I just hope like people who just experienced copilot to write emails at work finally get a glipse of the bigger picture. Also diamond pattern is rooted in the actuality because openai solved navier stoke this way. 10k agents working on this match problem.

### 2026-09-30 (later still)
> oh i dont care if they actually solved it or not, the point is how they use agents. Many agents on one job

### 2026-09-30 (last)
> We are not doing scientific reviews

### 2026-09-30 (P(doom) video)
> another rhink that  made me click recently is the upping my p(doom) video and all other made with opus 5.5. Thats javascript animated videos. It shows the model is understanding the spacial geometry at least in 2d, and its very impressive. It show the model can read its result and evaluate it and correct it. This, given infinite energy, opens the door to any problem solving. If a model can infinitely produce something and evaluate the result and correct it then they will become super cappable. In a strange way this ability to evaluate and correct seems more aligned with intelligence that getting it right the first time. Model can trial and error infinitely, and train infinitely. This match my all matter is compute lol. I dont remember what manga it is but there is a training room where they can spend 1000 years to train while 1s elapse in the real world lol.

### 2026-09-30 (speed)
> i tell you lol. I tell real things lol. Swarm of agents is not what matters for the video but the spacial understanding + self correction. Also what matters alongside energy is speed. If we have infinite long loop it is useless. The quicker the model is, the more self correction loops it makes

### 2026-09-30 (title)
> Stop thinking in term of articles. We are chatting, you record my thoughs this is good. About articles i think a good catchy title for the first one would be "leveraging infinity" - i dont know how it would translate in french.
