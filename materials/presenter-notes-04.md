# Presenter notes - Session 4: Recommendations

45 min. 3 welcome / ~14 concepts / ~22 apply-along / ~6 Q&A. Audience: mixed leaders + practitioners. Warm, fun, not dry.

## Run of show
- 0-3 · Welcome. Callback to S2 (neural nets) and S3 (embeddings): "today the machinery earns its keep every day." One-line hook: your feed runs on people who are secretly you.
- 3-8 · Part 1, two ways to recommend. Collaborative (people like you) vs content-based (items like this). Land "real systems blend both."
- 8-12 · Part 2, the daily engines + cold start. Netflix/Amazon/Spotify/TikTok are recommender-first. Then the empty day-one feed.
- 12-17 · Part 3, when it goes wrong. Filter bubbles, engagement gone bad, feedback loops, the objective question.
- 17-27 · Apply-along 1, recsandbox. Everyone rates and watches recs move.
- 27-33 · Apply-along 2, cold-start design.
- 33-39 · Apply-along 3, spot the objective (4 feeds).
- 39-45 · Quiz + Q&A.

## Preflight
- Open 04-recommendations.html once before the room arrives. Click into recsandbox and rate 2+ items so you have seen the recommendations appear (it shows nothing until 2 ratings - do not debug this live).
- Test one rating flip so you can reproduce the "recs shift" moment on demand.
- Projector zoom: on. Click each SVG once to confirm zoom works.
- Expand-all off to start; open cards as you narrate.

## Never cut these beats
- The live moment where you change a rating in recsandbox and the recommendations visibly shift. This is the whole session in one gesture - "the engine has no opinions, it mirrors the crowd."
- The objective / failure-mode discussion in Apply-along 3. The takeaway that the same tech is helpful or harmful depending on the human-chosen metric is the leadership payload.

## Cut if running long
- Apply-along 2 (cold-start design) can drop to a 60-second think-pair rather than full share-out.
- Matrix-factorization self-study card: point to it, do not teach it live.
- Trim the engines list in Part 2 to Netflix + TikTok if time is tight.

## Five expected questions
1. "Is it spying on me / reading my mind?" - No. It watches behavior (clicks, plays, ratings), not thoughts. The "how did it know?" feeling is just other people whose behavior rhymes with yours.
2. "Why do I get stuck in a bubble?" - You click one kind of thing, the model shows more of it, the feed narrows. It is a feedback loop, not a conspiracy - fixable with a better objective and deliberate diversity.
3. "Is collaborative or content-based better?" - Neither alone. Collaborative can't help brand-new items; content-based only echoes what you already like. Blend + popularity + rules.
4. "How does it work with no data on me?" - It doesn't, at first - that's cold start. Onboarding questions, content features, and a popularity fallback bridge day one.
5. "A click means I liked it, right?" - No - a click is not a like. Implicit signals are noisy; systems that treat every click as endorsement spiral into clickbait.

## Tone reminders
- Real-world story per concept is already in the callouts (Spotify Discover Weekly, Netflix Prize / 35% of Amazon sales, engagement re-tuning). Tell them as stories, not stats.
- Hyphens only, never em/en dashes, if you edit the deck live.
