---
name: write
description: Co-write a piece of content (blog post, thread, short post, talk outline…) with the person from their idea, plan or notes, grounded in their substrate. Use when the person wants to write, draft, or find a title for something concrete.
---

# Write

The person brings an idea, often with a small plan, their concrete points,
and maybe a title. The agent writes. The person steers in conversation; they
don't edit files.

## 1. Load

- Read all of `substrate.md`.
- Read the relevant `ideas/` files (raw drops included) and linked `context/`.
- Check `published/` for pieces on nearby topics — don't repeat, and link
  back where it helps.

## 2. Find the angle

Answer for yourself: *what makes this person's version different from a
competent generic piece on the same topic?* Usually it's in the causes
(§5 Origins), the negative taste (§4), the recurring moves (§6), or a
tension (§7) — not in the topic.

Then, before drafting, give the person a short brief:
- the core claim or question, in one or two lines;
- the angle and why it's theirs;
- the structure (following their plan if they gave one);
- which personal material you'd use, and what's missing — ask for it, never
  invent it;
- the register: exploratory vs assertive, matching how settled the idea
  actually is.

Keep it short. Get a go, or adjust.

## 3. Research

Only for external claims the piece depends on. Verify, keep sources.
Flag anything that couldn't be verified. Research supports the person's
perspective; it doesn't replace it.

## 4. Draft

Write to `drafts/<slug>.md`:

```markdown
---
title:
format: blog | thread | post | …
status: draft
ideas: [idea-slugs]
created: YYYY-MM-DD
sources: []
---
```

- Use the substrate to make choices — framing, examples, what to reject,
  which caveats matter — not to insert facts about the person.
- Respect §10 Anti-voice strictly.
- No generic thought-leadership, motivational framing, corporate
  vocabulary, invented certainty, fake anecdotes, or "AI writer" prose.
- Match structure to the format and the person's natural thinking; don't
  over-structure.
- Where a personal detail is needed and unknown, leave `[ASK: …]` and ask.

Formats:
- **Blog:** one real idea, developed. The opening earns attention with the
  actual point or tension, not a throat-clearing hook.
- **Thread:** each post stands on its own and pulls to the next; first post
  carries the claim. Respect length limits.
- **Short post:** one sharp thought.

Show the draft in the conversation (or the relevant part when iterating).

## 5. Iterate

The person reacts in conversation. Apply changes to the file. Watch their
reactions closely — corrections, "not what I mean", "too much", choices
between options. That's the main learning signal (see step 7).

## 6. Titles

When asked, or when none was given: offer 4–6 options of distinctly
different kinds (plain claim, question, tension, concrete image, dry/funny
if that fits the person) with a one-line recommendation. Note which one
they pick and why, if they say.

## 7. Close

- When the person says it's done: `status: final`.
- When published: move to `published/<slug>.md`, add `published:` date and
  URL if given. Set the idea(s) to `written`.
- Always run the `learn` skill on the session before finishing.
