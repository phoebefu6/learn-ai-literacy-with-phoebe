# Presenter notes - Session 8 · AI strategy and risk

## Preflight (5 min before)
- Open courses/08-ai-strategy-and-risk.html, click Projector zoom to 125%.
- Test the checklist widget once with a real use case: score "AI drafts first-pass replies to tier-1 support tickets" - tick the genuinely-true rows and confirm the verdict banner updates and the data row moves the score hardest.
- Confirm both SVGs render clean at zoom: the decision strip (no / yes branches) and the five-cell risk grid (mitigations in red).
- Have the six-row adoption-memo template on a slide or handout for Apply-along 3, and ask everyone to bring their Session 1 right-tool list.

## Run of show
- 0-3 · Welcome. Frame the capstone: "Seven sessions taught you how AI works. Today you decide with it." One line each: which session changed how they think most.
- 3-8 · Part 1 build / buy / API. Walk the decision strip. Land the default out loud: API-first, buy for a workflow, build ONLY your true edge. Tell both mistakes - the custom model that should have been an API call, and the moat rented behind someone else's endpoint.
- 8-13 · Part 2 the risk grid. Five rows, one line each, then the punchline: nearly every mitigation ends in "a human checks it first". Tell the hiring-tool bias story - bias lived in the data, not the intent, and a review gate catches it in an afternoon.
- 13-18 · Part 3 ROI, governance, memo. Real ROI = augment expensive time / messy input at scale / measurable. Hype = AI for its own sake or replacing a working rule. Governance is four things, not a committee. Introduce the six-row memo and the honest boundary: this is where literacy ends.
- 18-28 · Apply-along 1 scorecard. Everyone scores one real idea. Force honesty on the ticks. Debrief the data row (worth triple) and that a red is a useful answer.
- 28-34 · Apply-along 2 risk grid. Fill all five rows on one use case. Let the room find how often the answer is "human reviews before send".
- 34-40 · Apply-along 3 memo. Quiet writing time - do not talk over it. One volunteer reads answer-first; grade the first sentence only.
- 40-45 · Q&A + quiz + course close. End on the homework and "where next": builder skills, vendor docs, and data literacy underneath it all.

## Never cut
- The data row scoring triple in Apply-along 1 - it is the whole "no data, no AI" lesson made physical.
- The risk grid filled live in Apply-along 2 - reading a grid is not the same as applying it to your own case.
- The adoption memo in Apply-along 3 - it is the course's take-home artifact; the answer-first first sentence is the point.

## Cut if long
- The self-study "hidden costs of build" card - one sentence: "a built model is a standing team, not a line item".
- Apply-along 2 step 4 (flag the scariest risk) - state it verbally.
- The three-path recap on the close - point at the index page instead.

## Expected questions
- "Should we build or buy?" - API-first for capability, buy for a solved workflow, build only the one thing customers pay you for. A built model is a standing team; reserve it for your true edge.
- "How do we govern this?" - Four things, not a committee: a named owner, an approval gate before ship, an eval with a bar, and a kill switch. Add a human-in-the-loop check before anything irreversible.
- "What is next after this course?" - This is the end of the literacy arc. Next is hands-on builder skills and your vendor's docs - and the data-literacy course sits underneath all of it. No clean data, no AI.
- "How do we know an AI project is worth funding?" - Run the scorecard. If there is no expensive-human-time answer and no eval bar, it is usually hype wearing an AI sticker - send it back to Session 1's right-tool test.
- "Is prompt injection covered?" - Named in the risk grid, not gone deep on by design. Security depth is a separate course; the mitigation here is isolate untrusted inputs, least privilege, never trust output.
