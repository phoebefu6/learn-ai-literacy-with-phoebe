# Presenter notes - Session 7 · Using GenAI well

## Preflight (5 min before)
- Open courses/07-using-genai-well.html, Projector zoom 125%.
- Test the promptlab widget: flip one task weak -&gt; strong, confirm the output card and note change.
- Have your own weak-vs-strong prompt example ready from real work.
- Have the prompt-vs-RAG-vs-fine-tune tree from Part 2 clear in your head - it is the session's decision spine.

## Run of show
- 0-3 · Welcome. Frame: most people use GenAI at 10% of its value by treating it like a search box. Today is the craft.
- 3-8 · Part 1 prompt as spec. The five parts. "A brief for a brilliant, literal new hire." Examples beat adjectives (few-shot).
- 8-13 · Part 2 prompt/RAG/fine-tune. The money decision. Drill: facts that change -&gt; RAG; style at scale -&gt; fine-tune; else -&gt; prompt. The fine-tuning trap.
- 13-18 · Part 3 agents + evals. Agents = LLM + tools + steps (power + new failure modes). Evals = the discipline that makes it shippable. "Cannot ship what you cannot measure."
- 18-28 · Apply-along 1 promptlab. Everyone flips weak/strong on both tasks, extracts the five-part pattern, rewrites one of their own prompts. The rewrite is the takeaway.
- 28-34 · Apply-along 2 pick the approach. The 4 scenarios. Debate the close calls (brand voice = fine-tune candidate; numbers = prompt+grounding).
- 34-40 · Apply-along 3 design an eval. The "we ship when X% of Y pass Z" sentence. Do not rush the writing minute.
- 40-45 · Q&A + quiz. Q2 (RAG not fine-tune for facts) is the one they will use most.

## Never cut
- The prompt-as-spec pattern (Part 1) - the free 2x that everyone can use Monday.
- The prompt/RAG/fine-tune rule (Part 2) - saves teams a wasted quarter.
- The eval sentence in Apply-along 3 - the line between demo and product.

## Cut if long
- Part 1 self-study system/user prompt card - point at it.
- Cost/latency self-study card - practitioner-optional, name it.
- Apply-along 2 - compress to 2 scenarios if time is tight.

## Expected questions
- "Should we fine-tune our own model?" - Usually no. Try a strong prompt, then RAG. Fine-tune only for consistent style/format at scale, and expect it to go stale on facts.
- "Are agents ready for production?" - Powerful but risky - they loop, misuse tools, compound errors. Limit tools, cap steps, human-approve anything irreversible, and eval hard.
- "How big should our eval set be?" - Start with 20-50 real cases; grow it as you find failures. Any eval beats "seemed fine".
- "Which model should we use?" - A cost/latency/quality tradeoff, not "biggest". Small fast model for easy steps, large only for the hard one.
- "Isn't prompting going to be automated away?" - The spec-writing skill (say exactly what you want, with constraints and examples) is durable whatever the interface.
