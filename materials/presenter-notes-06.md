# Presenter notes - Session 6 · How LLMs work

## Preflight (5 min before)
- Open courses/06-how-llms-work.html, Projector zoom 125%.
- Test the tokenpredictor widget: pick a stem, set temperature low (top token ~85%), then high (odds flatten). Rehearse that flip.
- Have a real hallucination example ready (the invented legal cases story, or generate a fresh one live).
- If the room did Sessions 2-3-5, name the callbacks (neural nets, embeddings, retrieval all converge here).

## Run of show
- 0-3 · Welcome. Ask: "who has caught ChatGPT confidently making something up?" Every hand. Promise: by the end you will know exactly why, and what to do about it.
- 3-8 · Part 1 next-token. The one-sentence truth: predict next token, repeat. Autocomplete-scaled-up analogy lands it. Not lookup, not understanding.
- 8-13 · Part 2 dials. Training vs inference (frozen weights - kill the "it learns from our chat" myth). Context window = memory budget. Temperature = boldness.
- 13-18 · Part 3 hallucination. The big one. Optimizes plausibility not truth, no fact-checker. Three mitigations: ground / human / eval. The invented-legal-cases story.
- 18-28 · Apply-along 1 tokenpredictor. Everyone builds a sentence. The temperature flip is the aha - low = bland, high = where nonsense enters. Connect high temp to hallucination.
- 28-34 · Apply-along 2 rank hallucination risk. The 4 tasks. Land: grounded + verifiable + low-stakes = safe; recall + hard-to-verify + high-stakes = dangerous.
- 34-40 · Apply-along 3 context budgeting. The 100-page contract. Realization: retrieval quality caps answer quality (RAG bridge to nowhere-it-is-S7).
- 40-45 · Q&A + quiz. Q1 (predict-not-lookup) is the keeper.

## Never cut
- The one-sentence mechanism (Part 1) - the whole session hangs off it.
- The hallucination-is-built-in point (Part 3) - the single most important trust lesson in the course.
- The temperature flip in Apply-along 1 - it makes hallucination visceral, not abstract.

## Cut if long
- Part 2 self-study training-cutoff card - point at it.
- The transformers/attention self-study card - explicitly practitioner-optional, say so.
- Apply-along 3 - compress to a 2-minute discussion if the room is with you.

## Expected questions
- "Does it actually think / understand?" - No. It predicts tokens. The coherence feels like understanding; that is exactly the trap.
- "Will a bigger context window fix hallucination?" - It helps (more room to ground it) but does not cure it. The mechanism still optimizes plausibility.
- "Why does it get recent events wrong?" - Training cutoff; the weights froze. Feed current facts at inference (paste or RAG).
- "Is a bigger/more expensive model always better?" - Fewer hallucinations, but slower and pricier, and never zero. Match model to task (Session 7).
- "It said something false so confidently - is it lying?" - No intent. Confident tone is constant whether right or wrong. Never read confidence as accuracy.
