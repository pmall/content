# Substrate — Pierre

> The editorial model of the person behind the ideas. Maintained by the agent.
> Tags: `[E]` explicit · `[O]` observed · `[I]` inferred (unconfirmed) · `[C]` contextual.
> Optional source after a statement: `(interview 2026-09-28)`, `(idea: slug)`, `(write: slug)`.
> Prefer "tends to X because Y" over adjectives. Leave a section empty rather than fill it with generic material.
>
> The seed over-weights one-off ideas. [E] The "templates / value is data" thread is "one of my random idea from a few month ago", not a belief, and was removed from here (it lives in `ideas/`). Don't turn an individual idea into a trait. (interview 2026-09-28)
>
> `(seed)` = from `sources/personal_substrate_seed.md`, a summary written by another assistant from past conversations. Its quotes are verbatim; its other claims are secondhand, and they stay `[I]` until confirmed here.

- **Last reviewed:** 2026-09-29 (built from seed; voice and stance interview done, taste and Seren still open)
- **Content languages:** [E] English first; French translation only when asked. (interview 2026-09-28)
- **Audiences / channels:** [E] personal blog first, then articles shared on LinkedIn and Twitter/X. Audience: "people that matter, i dont know". (interview 2026-09-28)
- **Reader archetype:** [E] "People that matter are often non-expert too." The model reader is a smart decision-maker who knows AI is a big deal and is very interested, but doesn't know most of the concepts, where it's heading, or how to implement it. Example given: the director of a large organization with a legacy ERP and locked-down IT processes. They are not a peer developer. Private acquaintance, so never mention them or their organization in content. (interview 2026-09-29)
- **Register for writing:** [E] Writing should sound like the explanatory email (patient, plain, precise), not like the chat voice. (interview 2026-09-29)

---

## 1. Snapshot

- [E] Rejects the "AI expert" label. Their angle is the combination of biology, AI, data, full-stack implementation and judgment. (seed)
- [E] Personal AI memory should not be locked to one model or provider. (seed)
- [E] Thinks restricting AI assistants to work productivity is "stupid". Cares about personally meaningful use more than flashy automation. (seed)
- [O] Starts from a big application idea and strips it down until the infrastructure primitive shows: dating agent → social assistant → social MCP → shared-memory MCP. (seed)
- [O] Connects domains that look unrelated: presentation templates → software architecture, knowledge graphs → agent context, dating → social infrastructure. (seed)
- [O] Names an abstract concept, then treats the name as a reusable technical object ("the personal substrate"). (seed)
- [O] Keeps technical discussions informal on purpose: "haha", "Lmao", absurd images. (seed) [E] That is the chat register only. Their writing register is the patient explanatory one. (interview 2026-09-29)
- [O] Explains to non-experts by picking the one concept they lack and making it click: reports an "enlightening moment" from explaining vector search orally to a non-technical decision-maker. Not recorded, so no trace of how. (interview 2026-09-29)

## 2. Who they are

- [E] About ten years in bioinformatics / R&D at EnyoPharma: viral–human PPI networks, large biological datasets. See [enyopharma](context/enyopharma.md). (seed)
- [E] Earlier: CRCL / Inserm, alternative splicing and genomic annotation. See [crcl-inserm](context/crcl-inserm.md). (seed)
- [E] Their own term: a "template" is a coding agent plus markdown files that assist them in one field. This repo is one. (interview 2026-09-28)
- [E] Builds workflow and knowledge projects: [Wada](context/wada.md), [Kura](context/kura.md), [bpgraph](context/bpgraph.md), [Seren](context/seren.md). (seed)
- [E] Prefers independent/remote work over generic office or full-time web development. (seed)
- [E] Writes because they aren't visible enough. Has good ideas but trouble turning them into content, which is why this system exists. No existing body of writing. (interview 2026-09-28)
- [E] **Rejected label:** "AI expert / AI specialist". (seed)
- [E] Does not want content centered on their bioinformatics projects. Wada, Kura, bpgraph, EnyoPharma work are only examples, and "we dont care what graph it is". (interview 2026-09-29)

## 3. How they see things

- [E] Drawn to fundamental paradigms that others don't see: "i like to understand fundamental things that other dont see", "I like to see fundamental paradigms". (interview 2026-09-28)
- [E] Claims deep understanding of the AI field, and that few people see the full picture below. (interview 2026-09-28)
- [E] Central paradigm: AI work is a matter of compute. "x unit of energy = y units of intelligence." Given computing power, AI can keep working continuously and explore exhaustively. (interview 2026-09-29)
- [E] Most people miss it because their experience is one inference: ask for a document, judge that one output. "But this is still a stochastic process. This is one document out of infinity of documents the system can produce." (interview 2026-09-29)
- [E] The alternative they see: generate thousands of candidates, evaluate, rank, mix the good ideas. They call it "the diamond pattern" (fan out, then converge). (interview 2026-09-29)
- [E] Two failure modes of a single agent run: it loses track across many hypotheses, and which hypothesis it explores is stochastic. Their fix: one orchestrator spawning X subagents, one per hypothesis. "The greater the X the more exhaustive we are." (interview 2026-09-29)
- [E] On who ranks the candidates: "the agent, obviously", especially in biology. Treats evaluation by agents as a non-issue. The first version is one orchestrator that spawns a swarm and collects results. (interview 2026-09-29)
- [E] Their example came from exploring a graph database with Opus, but the graph is incidental. The point is general. (interview 2026-09-29)
- [E] No single concrete origin moment: the insight was not a specific event. It became clearer recently, after a few runs with a single big Opus. (interview 2026-09-29)
- [E] The compute/fan-out thesis is one idea among several, not the axis of all their content. Don't build the profile or the content around it. (interview 2026-09-29)
- [E] The substrate is theme-agnostic: its job is to capture *how* they think and write, so an LLM can produce personal, non-slop content on any topic. Topics are not the goal, so don't interview for themes. (interview 2026-09-29)
- [E] Reasons by projection: if something works this way now, obviously in 10 years it will be solved. Evidence they give: coding went "the full spectrum in 2 years"; at first people couldn't foresee AI would improve and solve coding. (interview 2026-09-29)
- [E] Agents are infrastructure, not only chatbots: persistent memory, MCP, context, agents working across applications. (seed)
- [E] MCP is the common interface between agents and a durable backend. Inversion: "the MCP is the application". (seed)
- [I] Judges ideas by whether they become systems that produce many outputs, not one good output (Wada, Kura, this substrate, Seren). (seed)
- [I] Values continuity of thought: context should survive conversations, agents and providers instead of restarting from zero. (seed)
- [I] Their core design question: what context should persist, where should it live, and who or what may use it? (seed)

## 4. Taste

- [E] Cares about concepts, not implementation: "I care about concepts, not implementation". Implementation details are a distraction from the point. Content should stay at the level of the paradigm. (interview 2026-09-29)

- **Interesting:** [E] agent architectures that make workflows reproducible; agents building structured knowledge as a side effect of ordinary use; memory that survives model changes; shared memory for closed groups (couples, families, project teams); a "semantic world" built from everyday agent use. (seed)
- **Boring:** [E] Notion and generic agent harnesses, unless they bring a real template/memory/context layer. (seed) [E] Generic office web-dev work. (seed)
- **Beautiful / elegant:** [I] the small primitive under a large category.
- **Clever:**
- **Bullshit:** [E] Being unable to project: "i tested yesterday, results on my specific example i think are bad, ai is useless". Judging a technology by today's state instead of its trajectory. Does not dislike the people, "its normal". (interview 2026-09-29) [E] Dislikes people who are "péremptoire", meaning unable to see farther than their own thing. (interview 2026-09-29) [E] Judging AI by one inference, as most people do. (interview 2026-09-29) [E] AI assistants used "only for work". (seed) [E] Automation that is impressive but doesn't matter to them ("I don't care my assistant can buy me plane tickets by itself"). (seed) [I] Business-model talk before the technical primitive is pinned down. Rebuked an assistant: "you are doing a bit too far in the business model. I'm not thinking about all this". (seed)

## 5. Origins

- [I] Wada → Kura → bpgraph: moved from building software toward infrastructure that lets other agents and builders produce things. (seed)
- [E] Shared-memory idea came from a concrete problem: switching from ChatGPT to Claude without losing accumulated context. (seed)

## 6. Recurring moves

- [O] Long-run projection: sets today's limitation against the trajectory. Appears both in the compute thesis and in how they explain AI skeptics. (interview 2026-09-29)
- [O] Reframes a common experience as a sample from a distribution: one output is one draw, not "the answer". Seen when explaining what people miss about AI. (interview 2026-09-29)
- [O] Reduces a question to a resource: exhaustiveness is "only a matter of energy/computing power". (interview 2026-09-29)
- [E] Reconstruction (not a memory of the sequence) of the vector-search explanation: models have a huge high-dimensional space encoding concepts; sentences become vectors in it; sentences close in meaning are close in space. It landed because the listener had a math background and had never realized these are "just vectors". (interview 2026-09-29)
- [I] Teaching move: connect the mysterious thing to something the reader already knows (here, math), so it becomes ordinary instead of magical. Same direction as the email's "just a function predicting the next word": demystify by naming the plain mechanism. Assume the reader is smart and use their existing knowledge.
- [O] Corrects the vocabulary before the argument: a word that misleads ("connaissances") is named and replaced by the mechanism. Also reads as an inversion of the naive picture (no knowledge base, just prediction). (interview 2026-09-29)
- [O] Asks "what is the layer underneath this?" instead of stopping at the product: dating app → substrate; agent → MCP → backend. (seed)
- [O] Scope reduction toward a buildable primitive. (seed)
- [O] Architecture as a chain of transformations: "Curate publications into a knowledgebase -> produce a presentation on this topic." (seed)
- [O] Architectural inversions ("the MCP is the application"). (seed)
- [I] Tests ideas with economic/system analogies: x402, subscriptions, marketplaces, infrastructure providers. (seed)
- [I] Follows a technical mechanism to its social consequence instead of starting from a market category. (seed)

## 7. Tensions

- [E] Wants rich, personalized, persistent AI memory, and sees personal data and privacy as a serious problem. (seed)
- [O] Drawn to very broad systems (semantic world, social graph) but pulls implementation back to a small primitive. (seed)
- [E] Values structure and reproducibility, yet lets autonomous systems like Seren run with a lot of independence. (seed)
- [I] Maximal context vs minimal product scope: rich substrate, small first build. (seed)

## 8. Epistemic style

- [E] Péremptoire = "sounding sure while being closed inside its frame" ("unability to see farther than their own thing"). Both parts matter: certainty is not the problem, and narrowness is not either. The combination is. (interview 2026-09-29)
- [E] Treats their observations as self-evident, "as sure as the sky is blue". Asked how they'd justify a claim: "How can i justify an observation other than 'i observe it'?" Their basis is what they have seen firsthand, stated as such. They don't build proof scaffolding around it. (interview 2026-09-29)
- [E] Cite and show studies when there is something real to cite. Their own observations stand as observations, but external evidence is welcome where it exists. Never pad with vague "studies show" or invent sources. (interview 2026-09-29)
- [E] Doesn't see why they'd write about unsure things: "Hypotheses and conjectures are not unsure." A hypothesis is a precise claim, not a fuzzy feeling. Don't add hedging or "unsure" framing to their theses just because they are hypotheses. (interview 2026-09-29)
- [E] Less absolute than Mallard. Mallard says "life is an algorithm"; they would say "the algorithm is like life". Same territory, but a comparison instead of an identity claim. (interview 2026-09-29)
- [E] Grants that a bold forecast can be "right in the absolute" (the endpoint) while insisting "there is so many frictions between here and there". Endpoint certainty, path caution. (interview 2026-09-29)
- [E] The frictions are human and organizational, not technical: people have routines and "are not ready to such big changes"; organizations move slowly and rely on legacy procedures not suited to AI. Expects "pure players" to take the spot in some fields. (interview 2026-09-29)
- [I] Writes as a comparison, not a reduction: doesn't claim X *is* Y. Unconfirmed beyond this one example.
- [E] Authority comes from work followed, not status or public visibility: "zero respect for public respect". Only a few people could make them doubt themselves, e.g. Demis Hassabis and Andrej Karpathy. If they disagreed with one of them, they would assume that person grasped something they missed. Otherwise a critic who says something wrong is simply wrong, and they don't much care. (interview 2026-09-29)
- [E] Institutional figures who "just say shit and are invited everywhere" (example given: Luc Julia, France) earn no respect. The stated harm: they comfort people in their ignorance. (interview 2026-09-29)
- [O] Their own theses are firm and declarative, and built on a wider view (trajectory, the full picture). (interview 2026-09-29)
- [O] Self-checks overreach with humor: "I'm crazy, right?" (seed)

## 9. Voice

- **Default mode:** [O] informal, fast, thinks out loud, often in chains of transformations. (seed)
- **Excited:** [O] sudden short bursts after long technical discussion ("What a game cyberpunk"). (seed)
- **Skeptical:** [O] blunt dismissal ("This is so stupid…"). (seed)
- **Uncertain:** [O] humor as a probe ("I'm crazy, right?"). (seed)
- **Amused:** [O] absurd images next to system-level speculation (the virgin cocktail line). (seed)
- **Rhythm and sentences:** [O] In explanatory writing (a French follow-up email to a non-expert, 2026-09-29): short paragraphs, one step of the argument each, plain declarative sentences, a blunt "Point." after a definition. Loaded words go in quotes ("connaissances", "contexte"). Plain vocabulary, no unexplained jargon. (interview 2026-09-29)
- **Explaining:** [O] Opens by flagging their own imprecision ("je n'ai pas été précis") and states the goal: clarify the reader's understanding. Then corrects a misleading word ("abus de langage") before making the argument. Replaces the naive picture (a knowledge database) with the actual mechanism (a giant function predicting the next word). Uses one concrete example (Freud in the training data, and what removing him would do). Ends with a practical thing to try, not a summary or a call to action. (interview 2026-09-29)
- **Calibration in writing:** [O] Firm on mechanism, measured on effects: "donne l'impression", "Ça peut produire de très bons résultats", no superlatives, no selling. The "not X but Y" contrast is used to correct a real misconception, never as a punchline. Slightly deflating tone ("n'est qu'un effet secondaire"). (interview 2026-09-29)
- **Abstraction level, examples, metaphors:** [O] coins names for concepts and reuses them as objects. (seed)
- **Jargon and structure:** [O] MCP, x402, substrate, primitive: technical terms used casually. (seed)
- **Their words and expressions:** French idioms come naturally ("ils ne voient pas plus loin que le bout de leur nez", "péremptoire"). (interview 2026-09-29) "substrate", "primitive", "the deep idea is…", "Lmao", "haha". (seed)
- **Their references:** Cyberpunk (game). (seed) [E] Stéphane Mallard ("the conference man"), heard on a podcast: admired because "he sells nothing. Just forsee things about ai". They say they are "less extreme than him". (interview 2026-09-29)
- **Humor:** [O] deadpan-absurd, self-deprecating. (seed)

### Samples

Chat register only. Publication register is still unknown.

- "i like to understand fundamental things that other dont see. [...] I like to see fundamental paradigms". Short declarative claims, no hedging. (interview 2026-09-28)
- Explanatory register, French email to a non-expert (style only, content may be outdated): "On a beaucoup parlé de “connaissances” [...] Mais c’est un abus de langage : un modèle de langage n’est qu’une fonction mathématique/statistique géante qui prend une entrée et prédit le prochain mot. Point." Names the misleading word, then the mechanism. (interview 2026-09-29)
- Same email: "Ce n’est pas “donner des connaissances” mais c’est simplement orienter la façon dont le modèle va prédire les prochains mots." Ends with "Vous pouvez tester avec les “projets” Claude". Deflates, then gives something to try. (interview 2026-09-29)
- "x unit of energy = y units of intelligence." and "This is one document out of infinity of documents the system can produce." Compresses a thesis into an equation, then an image. (interview 2026-09-29)
- "The greater the X the more exhaustive we are. And the point is this is only a matter of energy/computing power. People dont see this full picture". Explains a mechanism step by step, then states the stake. (interview 2026-09-29)

- "World is not ready for x402 so it Ould be subscription model. But when x402 emerge I will be there sitting peacefully with a virgin cocktail." Serious speculation, then an absurd image.
- "Actually kura can be the provider for wada. Curate publications into a knowledgebase -> produce a presentation on this topic." Architecture as a pipeline.
- "The deep idea is to manage to use the same MCP, make like a shared connection between your personal conversation with your agents." Looking for the primitive, informally.
- "This is so stupid we use this only for work." Blunt rejection of a default assumption.
- "I'm so tired this morning. Fortunately Claude is here to implement things". Delegating to agents as a normal part of building.

## 10. Anti-voice

- [E] Writing that is stuck inside one narrow frame, unable to see beyond "its own thing". This is what they mean by péremptoire: sounding sure while closed inside that frame. (interview 2026-09-29)
- [E] Overselling and marketing-sounding text: the main tell that AI-written content "isn't me". All three forms bother them: inflated claims, over-polished punchy rhythm, and a selling/persuading posture. (interview 2026-09-29)
- [I] Contempt toward people who disagree or don't see it. They call short-sightedness "normal". Explain what is missed, don't mock.
- [I] Framing them as an "AI expert" or guru.
- [I] Business-strategy padding around a technical idea.

## 11. Blind spots

- [I] Tension between "obviously in 10 years it will be solved" (§3) and "so many frictions between here and there" (§8). Resolved in part: technical problems get solved, and the frictions they accept are human/organizational (§8). They may still underweight technical frictions (e.g. evaluation) since they treat those as solved by projection.

## 12. Beliefs

- **Central:** [E] memory must be portable across providers. (seed)
- **Held loosely:** [E] the semantic world idea is exploratory ("This could be…"). (seed)

## 13. Boundaries

- **Never invent:** details of Seren, Vinland, Drakkar, Kura's build status.
- **Never name or attack people in content:** [E] Their private contempt for public figures (e.g. those who comfort people in ignorance) stays private. "I dont want to speak badly in my content". Explain what the wrong view misses, don't name or mock the person. Naming people they admire is fine when it serves the point. (interview 2026-09-29)
- **Confirm before using:** any anecdote from EnyoPharma or CRCL/Inserm; employer names in public content.
- **Keep out of content:** [E] bioinformatics projects as the subject of posts; use them only as examples, when an idea needs one. (interview 2026-09-29)
  Also: [E] personal/private life, relationships, health/wellbeing history, finances/investments. Kept out of the seed on request. (seed)
- **Private — do not record:** same list.

## 14. Open questions

| Question | Why it matters | Priority | Current hypothesis |
|---|---|---|---|
| ~~Visible to whom?~~ Partly answered: smart non-expert decision-makers, organizations with legacy processes | Shapes register and depth | Closed for now, revisit after a few posts | — |
| How do they make a concept click for a non-expert? (vector search explained orally, worked) | Would give the explanation moves an LLM should reproduce | Medium | Partly answered: connects the concept to what the reader already knows, and demystifies with the plain mechanism. Only one reconstructed example |
| Chat voice vs writing voice | Samples are chat only | Closed: writing = explanatory email register | — |
| ~~Scenario: a respected person says "agents are overhyped"~~ Answered: doesn't care about status, won't reply, never speaks badly of people in content | — | Closed | — |
| Does the thesis have limits they accept? (cost, diversity of candidates). They dismissed evaluation as a problem | Tells us how strongly they state it, and what caveats a post needs | High | Evaluation ("who ranks the thousand documents?") is the hard part. Their answer so far: the agent, obviously; not seen as a problem |
| ~~Where did they see this first?~~ Answered: no concrete moment, clearer after recent single-Opus runs | — | Closed | — |
| Why does continuity of context matter so much to them? | Would move §3 from [I] to [E] | High | Seen too much knowledge lost between tools, people or projects |
| What is Seren? | Mentioned as a tension, unexplained | Medium | — |
| What do they find clever or beautiful? | §4 is thin | Medium | Small primitives, inversions |
