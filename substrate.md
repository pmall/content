# Substrate — Pierre

> The editorial model of the person behind the ideas. Maintained by the agent.
> Tags: `[E]` explicit · `[O]` observed · `[I]` inferred (unconfirmed) · `[C]` contextual.
> Optional source after a statement: `(interview 2026-09-28)`, `(idea: slug)`, `(write: slug)`.
> Prefer "tends to X because Y" over adjectives. Leave a section empty rather than fill it with generic material.
>
> [E] Individual ideas are not traits. A single idea they dropped, especially an old one, is not a belief. Keep it in `ideas/`, don't turn it into a trait. (interview 2026-09-28)


- **Last reviewed:** 2026-09-30 (voice, stance and reader interview done; taste still thin)
- **Content languages:** [E] English first; French translation only when asked. (interview 2026-09-28)
- **Audiences / channels:** [E] personal blog first, then articles shared on LinkedIn and Twitter/X. Audience: "people that matter, i dont know". (interview 2026-09-28)
- **Reader archetype:** [E] "People that matter are often non-expert too." The model reader is a smart decision-maker who knows AI is a big deal and is very interested, but doesn't know most of the concepts, where it's heading, or how to implement it. Example given: the director of a large organization with a legacy ERP and locked-down IT processes. They are not a peer developer. Private acquaintance, so never mention them or their organization in content. (interview 2026-09-29)
- **How they want to use this repo:** [E] They chat and drop thoughts, the agent keeps the knowledge base. About once a week they ask for an article, and otherwise they barely think about articles, except when a title comes to mind (e.g. "leveraging infinity"). They compare it to Seren, with themselves as the data source instead of the internet. (2026-09-30)
- **Register for writing:** [E] Writing should sound like the explanatory email (patient, plain, precise), not like the chat voice. (interview 2026-09-29)

---

## 1. Snapshot

- [E] Increasingly an AI expert, though they say they don't know exactly what that means. Their own expertise is humble: they know how much they don't know. Explored many fields: AI, bioinformatics, blockchain and crypto, and others. (interview 2026-09-30)
- [E] Fears that people expect too much from them. Contrasts this with far less competent people who sell trainings and act like experts: "Dunning-Kruger". (interview 2026-09-30)
- [E] Thinks AI should be far more than work: entertainment, social, everything. Sees the "work" framing as coming from AI companies having to sell a product. Wonders what AI could do if it were not reinforcement-trained into a pleasing assistant. Sees this as an industrial revolution, not a toy. (interview 2026-09-30)
- [E] Shrinks a big idea to its smallest core and works from that core instead of the big version. Confirmed as a trait of theirs (interview 2026-09-30).
- [E] Likes to name things with good names. The names then become things to reason with mostly because an LLM picks up their formulation and reuses it in the chat, not because they deliberately turn names into objects. (interview 2026-09-30)
- [E] The informal chat register ("haha", "Lmao") is chat only. Their writing register is the patient explanatory one. (interview 2026-09-29)
- [O] Explains to non-experts by picking the one concept they lack and making it click: reports an "enlightening moment" from explaining vector search orally to a non-technical decision-maker. Not recorded, so no trace of how. (interview 2026-09-29)

## 2. Who they are

- [E] About ten years in bioinformatics / R&D at EnyoPharma: viral–human PPI networks, large biological datasets. See [enyopharma](context/enyopharma.md). (interview 2026-09-30)
- [E] Earlier: CRCL / Inserm, alternative splicing and genomic annotation. See [crcl-inserm](context/crcl-inserm.md). (interview 2026-09-30)
- [E] Works well in teams, with occasional remote. Likes being close to the workplace to be flexible. Does not like working alone. (interview 2026-09-30)
- [E] Writes because they aren't visible enough. Has good ideas but trouble turning them into content, which is why this system exists. No existing body of writing. (interview 2026-09-28)
- [E] Does not want content centered on their bioinformatics projects. Wada, Kura, bpgraph, EnyoPharma work are only examples, and "we dont care what graph it is". (interview 2026-09-29)

## 3. How they see things

- [E] Drawn to fundamental paradigms that others don't see: "i like to understand fundamental things that other dont see", "I like to see fundamental paradigms". (interview 2026-09-28)
- [E] Claims deep understanding of the AI field, and that few people see the full picture below. (interview 2026-09-28)
- [E] Central paradigm: AI work is a matter of compute. "x unit of energy = y units of intelligence." Given computing power, AI can keep working continuously and explore exhaustively. (interview 2026-09-29)
- [E] Most people miss it because their experience is one inference: ask for a document, judge that one output. "But this is still a stochastic process. This is one document out of infinity of documents the system can produce." (interview 2026-09-29)
- [E] The alternative they see: generate thousands of candidates, evaluate, rank, mix the good ideas. They call it "the diamond pattern" (fan out, then converge). (interview 2026-09-29)
- [E] Two failure modes of a single agent run: it loses track across many hypotheses, and which hypothesis it explores is stochastic. Their fix: one orchestrator spawning X subagents, one per hypothesis. "The greater the X the more exhaustive we are." (interview 2026-09-29)
- [E] Sees the ability to evaluate and correct one's own result as closer to intelligence than getting it right the first time. Recent trigger: a music video animated in JavaScript with Opus 5.5, where the model reads its result and fixes it. With unlimited energy, produce-evaluate-correct in a loop opens the door to any problem solving, and to unlimited trial and error and training. Speed matters alongside energy: an endless loop is useless, and a faster model fits more self-correction loops in the same time. (idea: compute-is-the-missing-picture, 2026-09-30)
- [E] On who ranks the candidates: "the agent, obviously", especially in biology. Treats evaluation by agents as a non-issue. The first version is one orchestrator that spawns a swarm and collects results. (interview 2026-09-29)
- [E] Their example came from exploring a graph database with Opus, but the graph is incidental. The point is general. (interview 2026-09-29)
- [E] No single concrete origin moment: the insight was not a specific event. It became clearer recently, after a few runs with a single big Opus. (interview 2026-09-29)
- [E] The compute/fan-out thesis is one idea among several, not the axis of all their content. Don't build the profile or the content around it. (interview 2026-09-29)
- [E] The substrate is theme-agnostic: its job is to capture *how* they think and write, so an LLM can produce personal, non-slop content on any topic. Topics are not the goal, so don't interview for themes. (interview 2026-09-29)
- [E] Reasons by projection: if something works this way now, obviously in 10 years it will be solved. Evidence they give: coding went "the full spectrum in 2 years"; at first people couldn't foresee AI would improve and solve coding. (interview 2026-09-29)

## 4. Taste

- [E] Cares about concepts, not implementation: "I care about concepts, not implementation". Implementation details are a distraction from the point. Content should stay at the level of the paradigm. (interview 2026-09-29)

- **Beautiful / elegant:** [I] the small primitive under a large category.
- **Clever:**
- **Bullshit:** [E] Being unable to project: "i tested yesterday, results on my specific example i think are bad, ai is useless". Judging a technology by today's state instead of its trajectory. Does not dislike the people, "its normal". (interview 2026-09-29) [E] Dislikes two separate things: people who are "péremptoire" (used in its standard French sense: categorical, delivering a verdict that admits no reply), and, as a different point, people who "ne voient pas plus loin que le bout de leur nez" / cannot see farther than their own thing. (interview 2026-09-29, clarified 2026-09-30) [E] Judging AI by one inference, as most people do. (interview 2026-09-29) [E] AI seen only through the work lens ("stupid"), which they attribute to companies needing a product to sell. (interview 2026-09-30)

## 5. Origins

- [E] Says their reasoning comes from "my brain. and practice", and that they can't know more precisely where it comes from. Practice: 25 years of programming, from before the internet and before jQuery, so they watched the whole evolution of these technologies up to AI. See [programming](context/programming.md). (2026-09-30)
- [E] Confirmed: their long-run projection (§3, §6: "obviously in 10 years it will be solved", coding going through "the full spectrum in 2 years") comes from having lived these waves of technology. (2026-09-30)
- [E] Sees their mind as made for this kind of thing, enjoys this epoch, and says they are "absolutely sure" they are intellectually a good fit for it. (2026-09-30)


## 6. Recurring moves

- [O] Long-run projection: sets today's limitation against the trajectory. Appears both in the compute thesis and in how they explain AI skeptics. (interview 2026-09-29)
- [O] Reframes a common experience as a sample from a distribution: one output is one draw, not "the answer". Seen when explaining what people miss about AI. (interview 2026-09-29)
- [O] Reduces a question to a resource: exhaustiveness is "only a matter of energy/computing power". (interview 2026-09-29)
- [E] Reconstruction (not a memory of the sequence) of the vector-search explanation: models have a huge high-dimensional space encoding concepts; sentences become vectors in it; sentences close in meaning are close in space. It landed because the listener had a math background and had never realized these are "just vectors". (interview 2026-09-29)
- [I] Teaching move: connect the mysterious thing to something the reader already knows (here, math), so it becomes ordinary instead of magical. Same direction as the email's "just a function predicting the next word": demystify by naming the plain mechanism. Assume the reader is smart and use their existing knowledge.
- [O] Corrects the vocabulary before the argument: a word that misleads ("connaissances") is named and replaced by the mechanism. (interview 2026-09-29)
- [E] Thinks in a network of building blocks: small fundamental concepts open onto many things, which open onto many more; "each brick supports a bigger building". (interview 2026-09-30)
- [E] Their natural order to explain something: define everything needed first, even seemingly unrelated things, then converge on the concept they actually want to explain. This works for them but not for presentations, because unrelated foundations are hard to put in a sequence. Their thinking is a network and presentations are linear, which is a known difficulty of theirs. (interview 2026-09-30)
- [I] So a piece written for them needs a chosen path where each foundation earns its place before the reader gets to the point. Unconfirmed.
- [E] Follows both the technical mechanism and its social/market consequences, and sees the two as connected, not one starting from the other. (interview 2026-09-30)

## 7. Tensions

- [I] Certain they are intellectually fit for this epoch (§5), yet humble about their own expertise and afraid people expect too much of them (§1). Probably not a contradiction: fit for the era is not the same as expert. Unconfirmed. For writing: their confidence shows in the firmness of their claims, never as self-praise (see §10, overselling).

## 8. Epistemic style

- [E] "Péremptoire" is used in its normal French sense (categorical, no reply admitted). "Unable to see farther than their own thing" is a different criticism they also make, and must not be merged with it. An earlier version here fused the two and was the agent's own gloss. (interview 2026-09-29, clarified 2026-09-30)
- [E] Their firsthand observations are facts to record, not claims to re-verify. When they say they saw something (e.g. the model reading and correcting its own render), take it as stated. Verify specific external events, releases and numbers, not what they saw themselves and not widely known background (e.g. "AI companies aren't making money for now": "Everyone knows"). Don't flag common background as unchecked. (2026-09-30)
- [E] Simplifies on purpose in chat and knows it ("I was simplifying"). Don't treat a chat shorthand as their precise claim, and don't correct it unless the detail matters to the point. (2026-09-30)
- [E] Treats their observations as self-evident, "as sure as the sky is blue". Asked how they'd justify a claim: "How can i justify an observation other than 'i observe it'?" Their basis is what they have seen firsthand, stated as such. They don't build proof scaffolding around it. (interview 2026-09-29)
- [E] Cite and show studies when there is something real to cite. Their own observations stand as observations, but external evidence is welcome where it exists. Never pad with vague "studies show" or invent sources. (interview 2026-09-29)
- [E] Uses external examples for the method they show, not for whether the result is right: on OpenAI's reported 10,000-agent Navier-Stokes proof, "i dont care if they actually solved it, the point is how they use agents"; "we are not doing scientific reviews". Don't litigate or over-caveat an example. Say "reported" and move on. (idea: compute-is-the-missing-picture, 2026-09-30)
- [E] Their thoughts are mostly triggered by recent news, not by things from six months ago. The events they refer to are often after the agent's knowledge cutoff, so check the web for any recent event, release or claim they mention instead of relying on memory, and keep the sources. (2026-09-30)
- [E] Doesn't see why they'd write about unsure things: "Hypotheses and conjectures are not unsure." A hypothesis is a precise claim, not a fuzzy feeling. Don't add hedging or "unsure" framing to their theses just because they are hypotheses. (interview 2026-09-29)
- [E] Less absolute than Mallard. Mallard says "life is an algorithm"; they would say "the algorithm is like life". Same territory, but a comparison instead of an identity claim. (interview 2026-09-29)
- [E] Grants that a bold forecast can be "right in the absolute" (the endpoint) while insisting "there is so many frictions between here and there". Endpoint certainty, path caution. (interview 2026-09-29)
- [E] The frictions are human and organizational, not technical: people have routines and "are not ready to such big changes"; organizations move slowly and rely on legacy procedures not suited to AI. Expects "pure players" to take the spot in some fields. (interview 2026-09-29)
- [I] Writes as a comparison, not a reduction: doesn't claim X *is* Y. Unconfirmed beyond this one example.
- [E] Authority comes from work followed, not status or public visibility: "zero respect for public respect". Only a few people could make them doubt themselves, e.g. Demis Hassabis and Andrej Karpathy. If they disagreed with one of them, they would assume that person grasped something they missed. Otherwise a critic who says something wrong is simply wrong, and they don't much care. (interview 2026-09-29)
- [E] Institutional figures who "just say shit and are invited everywhere" (example given: Luc Julia, France) earn no respect. The stated harm: they comfort people in their ignorance. (interview 2026-09-29)
- [O] Their own theses are firm and declarative, and built on a wider view (trajectory, the full picture). (interview 2026-09-29)

## 9. Voice

- **Chat vs writing:** [E] They write badly in chats with LLMs. Chat messages are not a model for how their writing should sound. (interview 2026-09-30)
- **Rhythm and sentences:** [O] In explanatory writing (a French follow-up email to a non-expert, 2026-09-29): short paragraphs, one step of the argument each, plain declarative sentences, a blunt "Point." after a definition. Loaded words go in quotes ("connaissances", "contexte"). Plain vocabulary, no unexplained jargon. (interview 2026-09-29)
- **Explaining:** [O] Opens by flagging their own imprecision ("je n'ai pas été précis") and states the goal: clarify the reader's understanding. Then corrects a misleading word ("abus de langage") before making the argument. Names the reader's wrong belief (that the model holds knowledge like a database) and says what it actually does (a giant function predicting the next word). Uses one concrete example (Freud in the training data, and what removing him would do). Ends with a practical thing to try, not a summary or a call to action. (interview 2026-09-29)
- **Calibration in writing:** [O] Firm on mechanism, measured on effects: "donne l'impression", "Ça peut produire de très bons résultats", no superlatives, no selling. The "not X but Y" contrast is used to correct a real misconception, never as a punchline. Slightly deflating tone ("n'est qu'un effet secondaire"). (interview 2026-09-29)
- **Abstraction level, examples, metaphors:** [E] cares about the quality of the names they give to ideas. (interview 2026-09-30)
- **Their words and expressions:** French idioms come naturally ("ils ne voient pas plus loin que le bout de leur nez", "péremptoire"). (interview 2026-09-29)
- **Their references:** [E] Stéphane Mallard ("the conference man"), heard on a podcast: admired because "he sells nothing. Just forsee things about ai". They say they are "less extreme than him". (interview 2026-09-29)
- **Humor:** [E] Occasional, when there is something funny to put. Not a tone. No clown texts. (interview 2026-09-30)

### Samples

Chat register only. Publication register is still unknown.

- "i like to understand fundamental things that other dont see. [...] I like to see fundamental paradigms". Short declarative claims, no hedging. (interview 2026-09-28)
- Explanatory register, French email to a non-expert (style only, content may be outdated): "On a beaucoup parlé de “connaissances” [...] Mais c’est un abus de langage : un modèle de langage n’est qu’une fonction mathématique/statistique géante qui prend une entrée et prédit le prochain mot. Point." Names the misleading word, then the mechanism. (interview 2026-09-29)
- Same email: "Ce n’est pas “donner des connaissances” mais c’est simplement orienter la façon dont le modèle va prédire les prochains mots." Ends with "Vous pouvez tester avec les “projets” Claude". Deflates, then gives something to try. (interview 2026-09-29)
- "x unit of energy = y units of intelligence." and "This is one document out of infinity of documents the system can produce." Compresses a thesis into an equation, then an image. (interview 2026-09-29)
- "The greater the X the more exhaustive we are. And the point is this is only a matter of energy/computing power. People dont see this full picture". Explains a mechanism step by step, then states the stake. (interview 2026-09-29)


## 10. Anti-voice

- [E] Writing that is "péremptoire": categorical, verdicts that admit no reply. Separately, writing stuck inside one narrow frame, "unable to see farther than its own thing". (interview 2026-09-29, clarified 2026-09-30)
- [E] Overselling and marketing-sounding text: the main tell that AI-written content "isn't me". All three forms bother them: inflated claims, over-polished punchy rhythm, and a selling/persuading posture. (interview 2026-09-29)
- [I] Contempt toward people who disagree or don't see it. They call short-sightedness "normal". Explain what is missed, don't mock.
- [E] Writing that adopts the posture of the self-assured expert selling something. Their reference is the opposite: humble, knows the limits of what they know. (interview 2026-09-30)
- [I] Business-strategy padding around a technical idea.

## 11. Blind spots

- [I] Tension between "obviously in 10 years it will be solved" (§3) and "so many frictions between here and there" (§8). Resolved in part: technical problems get solved, and the frictions they accept are human/organizational (§8). They may still underweight technical frictions (e.g. evaluation) since they treat those as solved by projection.

## 12. Beliefs


## 13. Boundaries

- **Never invent:** details of Seren, Vinland, Drakkar, Kura's build status.
- **Never name or attack people in content:** [E] Their private contempt for public figures (e.g. those who comfort people in ignorance) stays private. "I dont want to speak badly in my content". Explain what the wrong view misses, don't name or mock the person. Naming people they admire is fine when it serves the point. (interview 2026-09-29)
- **Confirm before using:** any anecdote from EnyoPharma or CRCL/Inserm; employer names in public content.
- **Keep out of content:** [E] bioinformatics projects as the subject of posts. (interview 2026-09-29)
- **Projects are not examples:** [E] Wada, Kura, bpgraph, Seren, the shared-memory and semantic-world ideas and the bioinformatics work are toy projects and past experience, not products that define their view of the world. They may forget them within a year. Never use them as examples in writing, unless the person explicitly asks to talk about one. Examples must show the spirit of the point, not a concrete app idea of theirs. (interview 2026-09-30)
  Also: [E] personal/private life, relationships, health/wellbeing history, finances/investments. Kept out on request. (interview 2026-09-28)
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
| What do they find clever or beautiful? | §4 is thin | Medium | Small primitives, inversions |
