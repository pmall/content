---
title: One answer is one draw (working title)
format: blog
status: draft
ideas: [compute-is-the-missing-picture]
created: 2026-09-30
sources:
  - https://www.quantamagazine.org/ai-has-solved-one-of-maths-1-million-millennium-prize-problems-20260908/
---

# One answer is one draw

Most people form their opinion of AI from a single answer. They ask it to write an email, read the result, and decide how good the AI is.

The word "answer" is misleading. A language model does not look something up. It predicts the next word, then the next one, and each choice has some randomness in it. Ask the same question twice and you get two different texts. The one you received is one draw from a very large set of texts the model could have written.

So when you judge that text, you are judging one sample. It may be a lucky one or an unlucky one, and you can't tell which from the inside.

The model is the same either way. What changes is how many times you let it work. Nothing forces you to ask for one text. You can ask for a thousand, read them (or have the model read them), rank them, and keep the best ideas from each. Fan out, then converge. I call it the diamond pattern: narrow at the start, wide in the middle, narrow again at the end.

It also applies to exploring a problem, not only to producing a document. A single agent working through many hypotheses picks which ones to follow at random, and it loses track of the others along the way. The alternative is one agent per hypothesis. The more agents, the more exhaustive the exploration, so how far you explore becomes a question of how much computing power you can spend.

This is not only a thought experiment. OpenAI reported that around 10,000 agents worked on a famous maths problem, Navier–Stokes, at the same time, passing what they found between them. I am not judging the result here. The method is what interests me: many agents, one job.

That is the part most people don't see yet. What they have seen is one draw.

To see the gap yourself, ask the same request five times and read the five answers side by side. They will agree on less than you expect, and that difference is what you never see when you read only one.
