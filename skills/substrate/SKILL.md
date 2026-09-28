---
name: substrate
description: Build or deepen a person's Personal Substrate — the editorial model of how they think and why — through a conversational interview. Use when substrate.md is missing (new setup), when the person asks for an interview session, or when open questions have piled up. Also scaffolds the content repo for a new person.
---

# Substrate

Goal: discover the material that answers *"why does this person think about
things this way?"* — well enough that two otherwise identical articles would
come out differently because of it.

Not a personality test, a bio, a list of favourites, or a style prompt.

## 1. Setup (first run only)

If the repo isn't set up, create what's missing:

```
substrate.md          # from template.md next to this skill; fill {{name}}
context/
ideas/INDEX.md        # "# Ideas\n\nNo ideas yet."
drafts/
published/
```

If `AGENTS.md` is missing, tell the person the system is incomplete without
it (it defines the modes and hard rules) — this skill alone only builds the
substrate.

## 2. Start from what exists

Before asking anything, read `substrate.md`, `sources/`, `context/`, `ideas/` (especially
raw drops), and anything the person points you to: articles, posts, notes,
project READMEs, talks. Ask once at the start whether such material exists.

Sort what you find into `[E]` / `[O]` / `[I]` / missing. Never ask the
person to repeat what's already available.

## 3. Interview

Feels like a good conversation, not a form. One main question at a time.
Follow interesting answers. Fewer, deeper questions. Write to `substrate.md`
after every few answers so progress survives across sessions.

Rough progression — adapt freely, skip what's known:

1. **Rough model.** Broad questions that reveal worldview:
   - What do you keep trying to understand?
   - What do you notice that others seem not to?
   - What makes you immediately want to build something?
   - What makes you think "this is bullshit"?
   - What have you changed your mind about?
2. **Causality.** For any preference or belief: *why?* → *where did that come
   from?* → *always believed it, or did something change it?* Aim for
   "I value X because experience Y taught me Z". Record the experience in
   `context/` and link it.
3. **Recurring patterns.** When the same move shows up in unrelated domains,
   name it: "You make this same move in A, B and C — deliberate, or am I
   overreading?"
4. **Negative taste.** What's boring, fake, distrusted, overrated; advice
   they reject; complexity they refuse; writing they hate.
5. **Contradictions.** "These pull in opposite directions — real tension, or
   a distinction I'm missing?" Keep real tensions in §7.
6. **Scenarios** expose decisions better than abstractions: someone attacks
   your favourite idea; an impressive but useless technology; a simple tool
   beats a platform; you find out you were wrong; one hour to solve a
   problem.
7. **Voice, last.** Only once the person is understood. What feels fake to
   read? What would make an article correct but obviously not theirs?
   Certain, exploratory, provocative? What should stay out of their writing?
   Phrases an AI must never use for them?

   Self-description of style is unreliable. Weight it below what their own
   messages show, and collect verbatim samples in §9.

Behaviour:
- Quote or summarize their previous answer when probing it.
- Challenge gently when an answer is vague or generic.
- Test hypotheses out loud: "Emerging hypothesis: you value X over Y. Accurate?"
  Confirmed → `[E]`. Rejected → remove. Unsure → stays `[I]` or goes to §14.
- Every so often, summarize the emerging model in a few lines and ask for
  corrections.
- No flattery. No psychologizing, diagnosing, or inferring sensitive
  attributes. Political positions only if stated.
- Stop when returns diminish. It's fine to end a session with open questions.

## 4. Write it up

Fill the template. Rules:
- Tag every statement. Keep the person's own terminology where distinctive.
- Causes over adjectives. "Pragmatic" is useless; the experience that made
  them pragmatic about *what* is useful.
- Individual article ideas go to `ideas/`, not here — unless they reveal a
  recurring pattern.
- Update §1 Snapshot last, from `[E]`/`[O]` only.

## 5. Quality check

Before ending a session, check and fix:
- **Generic?** Could it describe 10,000 smart people?
- **Causal?** Does it explain *why*, not just *what*?
- **Distinctive?** Would it change how an article comes out?
- **Provenance?** Is said / observed / guessed always clear?
- **Negative space?** Does it capture what they reject?
- **Tensions?** Or has it become a neat caricature?

## 6. Close the session

Tell the person briefly: what's now solid, the main open questions, and the
one or two questions most worth asking next time. Don't dump the file.
