# Presenter notes - Session 3: Embeddings

Runtime 45 min. Goal: they leave able to say what an embedding is (a vector capturing meaning), why near = related, and why one embedding space powers search, recs, and LLMs. The meaning-map widget is the anchor - protect it.

## Run of show

- **0-3 · Welcome.** One-line hook: "a computer has no dictionary. Here is the trick it uses to read meaning anyway - turn everything into a position on a map." Callback to S2: those positions are numbers a neural net produces.
- **3-18 · Concepts (Parts 1-3).** Part 1 things into numbers, meaning as location, 2D is a shadow. Part 2 distance = similarity + king - man + woman ≈ queen. Part 3 vector databases + the RAG preview. ~5 / ~4 / ~4 min. Do NOT read the self-study card aloud - point to it.
- **18-40 · Apply-along.** Demo 1 the embedding widget (10 min, the anchor). Demo 2 keyword vs semantic (6 min). Demo 3 what would you embed (6 min).
- **40-45 · Q&A + close.** Land the cheat sheet, tee up Session 4 (recommendations).

## Preflight (do before they walk in)

- Open 03-embeddings.html, hit "Expand all" once then collapse, toggle Projector zoom on for the room.
- Test the embedding widget once: click a word in each cluster and confirm neighbors light up. Have one satisfying pairing ready to show (e.g. cat -> kitten) so the reveal lands on the first click.
- Zoom both SVGs on the projector - especially the king-man+woman parallelogram, check the labels are readable at the back.

## Never-cut beats

- **The click-a-word neighbors reveal.** The moment a word is clicked and related words light up with no human labeling - stop and name it: "no one filed these together. The machine placed them purely from usage." This is the aha.
- **Keyword vs semantic.** Make someone say a customer phrase in their own words ("won't turn on") and show it lands next to the official term ("power failure"). This is where a leader feels the business value.
- The one-line spine: "meaning becomes a position, so relatedness becomes distance."

## Cuts if running long

- Drop Demo 3 (what would you embed) to a 2-min verbal prompt; assign it as homework instead.
- Compress the vector-arithmetic explanation to just showing the SVG and saying "meaning has directions."
- Skip the RAG preview detail; say only "this retrieval step comes back in Sessions 6 and 7."

## Five expected questions

1. **"Does the machine really understand the words?"** No - it captures statistical meaning (which words keep similar company), not human understanding. It has geography, not comprehension. Powerful, and not the same thing. Keep this honest.
2. **"Where do embeddings come from?"** Learned from huge amounts of text (or images): the model sees billions of examples of how things are used and places them so similar usage lands nearby. Nobody hand-assigns the numbers.
3. **"Why hundreds of dimensions? The map only had two."** The 2D map is squashed so we can see it. Meaning has many independent directions (topic, tense, sentiment, and more), so real spaces need hundreds - the self-study card covers this.
4. **"Is this the same as a normal database?"** No - a normal DB matches exact values; a vector DB finds nearest neighbors by meaning. "Find similar" instead of "find equal."
5. **"How does this connect to ChatGPT?"** LLMs run on embeddings internally, and RAG uses a vector DB to fetch your documents for the model to answer from. Session 6 opens the LLM; Session 7 builds the RAG.

## Close

"Meaning is a location, and relatedness is distance - that one idea runs search, recs, and LLMs. Next session: recommendations, the first place this quietly makes money."
