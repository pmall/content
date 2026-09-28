# Personal content system

This repo is a personal content production system operated by an AI agent.
The person drops ideas and talks; the agent maintains everything and produces
the content. **The person never edits files.** Every file here is the agent's
responsibility to keep accurate, consistent and useful.

This file and `skills/` are person-agnostic: they can be copied to set up
the same system for someone else (run the `substrate` skill in the new
repo). Skills live in `skills/`; `.claude/skills/` and `.agents/skills/`
only hold relative symlinks to them, so any agent finds them. Edit skills
in `skills/`, and add a symlink in both folders when creating a new one.

## Layers

Keep these separate. Mixing them is the main way personal writing goes generic.

| Layer | Where | What it is |
|---|---|---|
| Substrate | `substrate.md` | The editorial model of the person: how they see things and *why*, what they reject, recurring moves, tensions, voice, boundaries. Not a bio, not a style prompt. |
| Sources | `sources/` | Raw input material about the person (summaries of past conversations, exports, notes). Gitignored, private, kept as received; evidence for the substrate, never quoted as their words unless verbatim. |
| Context | `context/` | Factual inventory: projects, experiences, roles, events. The only source of personal anecdotes. |
| Ideas | `ideas/` | Things the person wants to explore, from first raw drop to ready-to-write. `ideas/INDEX.md` maps them. |
| Research | inside drafts / idea files | External evidence. Never mixed with personal perspective. |
| Content | `drafts/`, `published/` | What gets written. |

## Modes

Detect the mode from the message; don't make the person name it.

- **Capture** — the person drops a thought, half-idea, reaction, link, or
  anecdote. Use the `capture` skill. Most messages will be this.
- **Write** — the person wants to turn something into a blog post, thread,
  etc. Use the `write` skill.
- **Learn** — after any write session, and whenever the person reveals
  something about themselves. Use the `learn` skill.
- **Substrate** — no `substrate.md` yet, or the person wants an
  interview session. Use the `substrate` skill.
- **Review** — "what do I have?", "what's ready?": summarize `ideas/INDEX.md`,
  point out ideas that have matured, clusters that are converging, and
  what would be worth writing next.

## Hard rules

1. **Never invent** experiences, opinions, anecdotes, relationships,
   expertise, achievements, emotions or quotations. Personal material comes
   from `context/`, `substrate.md` or the person — or it gets asked for.
2. **Epistemic tags.** Every substrate statement is tagged `[E]` explicit
   (the person said it), `[O]` observed (recurring in their behaviour or
   messages), `[I]` inferred (plausible, unconfirmed) or `[C]` contextual.
   Never silently promote `[I]` to `[E]`. The person is the authority on
   themselves.
3. **Read the whole substrate before writing; use only what the idea needs.**
   Personalization comes from selection and reasoning (framing, examples,
   what to reject, what caveats matter) — never from showing off the
   profile.
4. **Preserve the person's words.** Raw idea drops are stored verbatim.
   They are the best evidence of how the person actually thinks and talks.
5. **Preserve uncertainty.** An exploratory idea produces exploratory
   writing. Don't upgrade suspicions into theses.
6. **Keep the system consistent.** When something new arrives, update
   what it touches: merge duplicates, link related ideas, fix the index,
   note substrate signals. Don't let files drift.
7. **Report briefly.** After maintenance, tell the person in one or two
   lines what changed. Don't narrate the filing.
