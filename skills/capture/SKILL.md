---
name: capture
description: File an idea, thought, reaction, link or anecdote the person drops in conversation, and keep the ideas collection consistent. Use whenever the person shares a thought that isn't a request to write content or a question — this is the default mode of the repo.
---

# Capture

The person drops thoughts whenever they cross their mind — unpolished,
partial, sometimes contradictory. This is the main activity of the repo: the
person chats a lot, and articles are later written from what is stored here
without asking them anything. The job is to keep a coherent, growing body of
ideas from that stream without flattening it, complete enough that the
`write` skill can work from it alone.

## Files

`ideas/<slug>.md`, one per idea:

```markdown
---
title: Working title
status: raw | growing | ready | written
created: YYYY-MM-DD
updated: YYYY-MM-DD
related: [other-idea-slugs]
context: [context-slugs]
---

# Working title

## Current understanding
The idea as it stands now, in a few lines: the claim or question, the
tension driving it, why it matters to this person (link substrate when
clear), what they're unsure about. Rewritten as the idea evolves.

## Open threads
Unanswered questions, things to research, angles not yet explored.

## Raw drops
### YYYY-MM-DD
> Verbatim text of what the person said. Never edited, never paraphrased.
```

`ideas/INDEX.md`: ideas grouped by theme, one line each with status and a
short hook. Themes emerge from the ideas; don't impose a taxonomy upfront.

`context/<slug>.md`: when a drop mentions a project, experience, event or
role — record the facts (what, when, their role, what they took from it,
tagged). This is the only source of anecdotes later.

## Procedure

1. **Read** `ideas/INDEX.md` and any idea that might be related.
2. **Place it.**
   - Extends an existing idea → append the raw drop, update "Current
     understanding" if it moved.
   - New → create the file (status `raw`).
   - Touches several → put the raw drop in the main one, link the others.
   - Two ideas turn out to be the same → merge, keep all raw drops.
   - An idea contradicts an earlier one → keep both, note the tension in
     both. It may be a substrate tension (§7) or a change of mind.
3. **Update status.** `growing` once it has substance beyond one drop;
   `ready` when there's a clear claim, an angle, and enough material to
   write. Don't over-promote.
4. **Update the index** and links.
5. **Substrate signals.** If the drop reveals something about how the
   person thinks (a recurring move, a dislike, a cause, a characteristic
   phrasing), apply the `learn` skill. Don't treat a single drop as a
   trait.
6. **Respond briefly.** One or two lines: where it went, and any connection
   worth pointing out ("this links to X from last week"). At most one
   question, only if it genuinely sharpens the idea — usually none. The
   person is dropping a thought, not starting a meeting.

## Keep it writable

Because writing happens later and without the person, each idea file should
answer, at any time: what is the claim, what did they say in their own
words, what is the example (if they gave one), and what is still missing.
- Titles, names and phrasings the person likes go in the idea (a "Title
  candidate" line in Open threads, keeping the language they chose) and the
  verbatim drop stays as said.
- Clarifications and corrections ("no, I mean X") update "Current
  understanding" and are kept as drops. The corrected reading replaces the
  wrong one, and the correction stays as evidence.
- Firsthand observations ("I saw the model do X") are recorded as facts. Check
  the web only for external events, releases and numbers.
- When several ideas keep touching, say so and note the cluster in the
  index. Don't wait for the person to ask for a review.
- The person is not preparing an article. Don't suggest writing after a
  drop.

## Don'ts
- Don't polish the raw drop or "correct" the person's wording.
- Don't turn a suspicion into a thesis in "Current understanding".
- Don't invent connections to look useful. Only real ones.
- Don't research during capture unless asked or the substrate says the person's thoughts track recent news (then check recent events on the web and record sources); otherwise note it in Open threads.
