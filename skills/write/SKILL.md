---
name: write
description: Write a piece of content (blog post, thread, short post, talk outline…) for the person from the knowledge base (ideas, context, substrate), with or without a topic given. Use when the person asks for content, a draft, or a title.
---

# Write

The agent writes from the knowledge base. The person usually brings nothing:
no topic, no plan, sometimes just a title or "write something". They react
to the draft in conversation and never edit files. Everything the piece
needs should already be in `ideas/`, `context/` and `substrate.md`; ask only
when something essential and personal is truly missing.

## 0. Choose (when no topic is given)

Pick from `ideas/INDEX.md` by maturity: a clear claim, their own words, an
example they gave, few open gaps; a converging cluster; nothing already in
`published/` or `drafts/`. If they gave a title, use it and find the idea it
belongs to. Say in one line what you picked and why, name one or two
runner-ups, and go on. Don't wait for approval.

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

Then state a short brief (the person may skip reading it; don't hold the
draft for a go unless the angle is genuinely uncertain):
- the core claim or question, in one or two lines;
- the angle and why it's theirs;
- the structure (following their plan if they gave one);
- which personal material you'd use, and what's missing — ask for it, never
  invent it;
- the register: exploratory vs assertive, matching how settled the idea
  actually is.

Keep it short, then draft. The draft is what they react to.

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
- Where a personal detail is needed and unknown, prefer an angle that
  doesn't need it. If it is truly essential, leave `[ASK: …]` and ask once
  after showing the draft.

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

If the person gave a title, use it (in the language they chose). When asked,
or when none was given: offer 4–6 options of distinctly
different kinds (plain claim, question, tension, concrete image, dry/funny
if that fits the person) with a one-line recommendation. Note which one
they pick and why, if they say.

## 7. Close

- When the person says it's done: `status: final`.
- When published: move to `published/<slug>.md`, add `published:` date and
  URL if given. Set the idea(s) to `written`.
- Run the `learn` skill on the session before finishing. Reactions to the
  draft are the strongest signal about voice.
