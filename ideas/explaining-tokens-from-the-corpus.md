---
title: Explaining tokens by disconnecting them from LLMs
status: raw
created: 2026-10-16
updated: 2026-10-16
related: [agent-gets-an-environment, ai-is-blurry-super-agency]
context: [demystifying-ai-deck]
---

# Explaining tokens by disconnecting them from LLMs

## Current understanding
The person has a better way to explain tokens, for their slide deck about
demystifying AI: **totally disconnect the concept from LLMs** and start from
the problem it solves.

The steps as they gave them:
1. The training set is the whole of human knowledge as text.
2. To treat it statistically, it has to be encoded in a single vocabulary.
3. Words are not very adapted or optimized for that.
4. "Tadam": tokens are slices of characters that are frequently found in the
   corpus.

Why words are not adapted (their answer, 2026-10-16, "first" so possibly
more reasons to come):
- A word vocabulary is scoped to a single language.
- Many languages have vocabulary that is not words.
- "Word" is itself hard to define.
- Some languages don't even have spaces.

So a token is presented as the answer to an engineering need (a vocabulary
for statistical treatment of a huge text), not as a piece of how a language
model works.

## Open threads
- What was the earlier explanation that did not work? Not said (they said
  "a better way", so there was a worse one).
- They said "first", so there may be more reasons why words don't fit. Ask
  if they come back to it.
- Same shape as `ai-is-blurry-super-agency`: "word" is hard to define, like
  "intelligence" and "agent". Real echo, theirs to make, not stated.
- The "Tadam" is theirs: the reveal comes after the need is built. Keep the
  order if written up.
- Does the same method (start from the need, drop the LLM) apply to other
  concepts in the deck? Not said.

## Raw drops
### 2026-10-16
> Also i have a better way to explain tokens: totally disconect it from llms. Like ok the training set is the whole human knowledge as text. We have to encode this in a single vocabulary for statistical treatment. Words are not very adapter and optimized. Tadam, tokens are slice of characters we frequently find in the corpus.

### 2026-10-16 (why not words)
> first, word vocabulary are scoped to a single language. And many languages have non word vocabulary. Word is hard to define. Some languages dont event have spaces.
