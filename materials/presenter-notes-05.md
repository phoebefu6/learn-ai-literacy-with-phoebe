# Presenter notes - Session 5: Search and ranking

45 min. 3 welcome / ~14 concepts / ~22 apply-along / ~6 Q&A. Audience: mixed leaders + practitioners. Warm, fun, not dry.

## Run of show
- 0-3 · Welcome. Callback to S3 embeddings: "closeness = similar meaning - today it pays off in public." Hook: the moment two results match, someone decides the order.
- 3-8 · Part 1, keyword to semantic. Letters vs meaning. "Won't turn on" finds "power failure." Keyword still wins for codes and names.
- 8-13 · Part 2, ranking = weighted signals. There is no objective #1; "the algorithm changed" = the weights changed.
- 13-17 · Part 3, RAG. Search your docs, feed top passages to the LLM, grounded answer. The dominant enterprise pattern.
- 17-27 · Apply-along 1, rankingtuner. Everyone reweights and watches #1 change.
- 27-33 · Apply-along 2, design your search.
- 33-39 · Apply-along 3, RAG readiness audit.
- 39-45 · Quiz + Q&A.

## Preflight
- Open 05-search-and-ranking.html once. Click into rankingtuner and move each of the three signal weights so you have seen the order reorder live (do not discover the controls in front of the room).
- Confirm you can push the exact-match doc down the list by leaning on freshness/popularity - that is the money moment in Apply-along 1.
- Projector zoom: on. Click both SVGs once (keyword-vs-semantic lanes, and the RAG pipeline) to confirm zoom.
- Expand-all off to start.

## Never cut these beats
- Burying the exact-match, high-relevance doc by reweighting, live in rankingtuner. It makes "there is no objective #1" undeniable - the room feels it, doesn't just hear it.
- The RAG pipeline walkthrough (question -> embed -> retrieve -> LLM reads -> grounded answer) and the line "search quality caps answer quality." This is the bridge to S6-S7 and the enterprise payoff of the whole course.

## Cut if running long
- Apply-along 2 (design your search) can shrink to a 60-second pair discussion.
- Personalization and chunking self-study cards: signpost, don't teach live.
- Trim the SEO story in Part 2 to one sentence if needed.

## Five expected questions
1. "Does RAG stop all hallucination?" - No - it reduces it, doesn't eliminate it. If retrieval misses the right passage, the model confidently answers from the wrong context. Answer quality is capped by retrieval quality.
2. "Is keyword search dead?" - No. Hybrid is the norm. Keyword nails exact codes, names, and part numbers that semantic can fumble; semantic rescues natural-language queries. Real systems run both.
3. "Who decides the ranking weights?" - A team at the company. That's the point: "best result" is a product/business choice encoded as numbers, not a fact of nature.
4. "Do we need to fine-tune the model for our data?" - Usually start with RAG, not fine-tuning: cheaper, fresher (update docs, not the model), and it cites sources. S7 covers the decision.
5. "Why is my search assistant giving bad answers?" - Almost always retrieval, not the model: stale PDFs, duplicate policies, bad chunking. The AI project is a data project.

## Tone reminders
- Real-world stories are in the callouts (support-centre deflection, the SEO industry, the "ask our docs" cleanup month). Tell them as stories.
- Hyphens only, never em/en dashes, if you edit live.
