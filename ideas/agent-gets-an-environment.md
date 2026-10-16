---
title: The difference between a chatbot and an agent is the environment
status: raw
created: 2026-10-05
updated: 2026-10-16
related: [less-between-data-and-result, shared-memory-mcp, compute-is-the-missing-picture, orchestrating-agents-strategies, ai-is-blurry-super-agency]
context: [literature-curation, demystifying-ai-deck]
---

# The difference between a chatbot and an agent is the environment

## Current understanding
The main difference between chatbot usage and agentic usage is that the
agent gets an environment: a filesystem and tools. With it, the agent can
organize its own documentation and its own memory of a project, and each
session it gets back to where the work was left. The person thinks most
people have not conceptualized this: they see the agent as a chatbot that
does more, not as something that lives in a place and keeps state there.

Consequence the person drew from their own practice: working with an agent
on a project, with its folder and git repo, is teaching it the job the way
you would teach an intern. The knowledge ends up in files the agent
maintains, instead of in your head or in a one-off conversation.

Their example (firsthand, see `context/literature-curation.md`): replacing
manual curation of scientific literature with Claude Code. Only an example
of the principle, not the subject.

This repo is the same pattern applied to the person themselves (see the
"this repo" drops in `less-between-data-and-result`). Confirmed by them: the
agent here is literally their note-taking intern and content producer.

Their picture of an agent (2026-10-16, for a slide deck that goes from zero
to swarms of agents; see `context/demystifying-ai-deck.md`): a
**three-party conversation**. The user talks to the chatbot, the chatbot
talks to the environment. The chatbot is the middleman between the user and
the environment. The **environment is anything to act on**: the filesystem,
databases, connectors, code execution, instruction files, etc. The chatbot
holds the whole conversation: the one with the user, and the
instruction-response loop it has with the environment. "Agent" is hard to
define because, for them, it is the **chatbot + the environment**. Treating
it as three entities (user, chatbot, environment) always makes it simple to
understand. This is their model, used as the explanation of "agent".

Confirmed and extended (2026-10-16, later): the skills (instructions) are
literally something the chatbot **reads from the environment**. The model
lives **only in the chatbot**; everything else, instructions included, is
environment. And a **swarm is a fractal**: a chatbot instructs the spawning
of another chatbot and its own environment, and instructs it. So the same
three-party picture repeats inside itself, each spawned unit being a
(chatbot, environment) pair under the one that created it. This is their
model, used for the deck.

Link to `ai-is-blurry-super-agency`: their definition of agency (using
available tools efficiently to reach a goal) is what the chatbot does on
the environment side of this picture.

## Open threads
- Fractal swarm: the user of a spawned chatbot is the chatbot that spawned
  it. Does the person say it that way? Not said. In the fractal, is the new
  environment shared with the parent or separate? "Spawn another chatbot and
  environment" suggests separate; not confirmed.
- Link to `compute-is-the-missing-picture` and `orchestrating-agents-strategies`:
  the orchestrator spawning one subagent per hypothesis or publication is this
  fractal in practice (each subagent has its own context and files). Confirmed
  by them (2026-10-16): the curation project's result files are built to work
  like a fractal, but Claude Code allows only one level (the main agent
  spawns subagents), so in practice it is one level deep.
- What exactly does the environment add? Candidates from the drop: persistent
  memory across sessions, self-organized docs, tools. Which one is the core?
  (They said "filesystem and tools"; the rest follows.)
- The intern comparison: what does "teaching" consist of in practice, at the
  concept level (instructions, examples, corrections that stay in files)?
- Link to `shared-memory-mcp`: that idea is memory shared across agents and
  people; this one is memory the agent keeps inside its own environment.
- Title candidate: none given. The person's phrasing: "the agent gets an
  environment".

## Raw drops
### 2026-10-05
> also a think i didnt word precisely is i think the main difference between chatbot usage and agentic usage, is the agent gets an environment. Filesystem and tools. So the agents can organize its own doc and memory of a project. And the agent gets back to where we were each session. Most people have not conceptialized this. Like, im making a project here, about replacing manual curation of scientific litterature by claude code, and it has its folder and git repo. I realized that im basically teaching claude how to do the job like an intern.

### 2026-10-05 (later)
> Yes this repo is the same idea, you are litteraly my note taking intern and content producer haha

### 2026-10-16
> Then for my slide deck that goes from zero to swarmsof agents, here is how i picture agent. Agent is a hard term to define too. I picture this like a three person conversation. The user talk to the chatbot, the chatbot talks to the environment. So the chatbot is the middleman between the user and the environment. By environment i mean anything to act on. The filesystem, the databases, the connectors, the code execution, the instruction files etc. The chatbot hold the whole conversation, with the user and the instruction response loop he has with the environment. Agent is hard to define because for me it is the chatbot + the environment. But treating this as 3 entities always make it simple to understand.

### 2026-10-16 (swarm)
> yeah litteraly, the skills (instruction) are something read from the environment. A swarm is a fractal, the chatbot instruct to spawn another chabot and enviroment and instruct it. The model is only contained in the chatbot.
