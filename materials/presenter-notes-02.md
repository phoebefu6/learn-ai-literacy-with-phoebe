# Presenter notes - Session 2: Neural nets and deep learning

Runtime 45 min. Goal: they leave able to say what a neuron computes, what "deep" means, and own the black-box tradeoff. The neuron widget is the heart of the session - protect it.

## Run of show

- **0-3 · Welcome.** Callback to Session 1: "deep learning was the doll everyone means by AI. Today we open it." Promise: no math, no biology - just a tiny piece of arithmetic repeated at scale.
- **3-18 · Concepts (Parts 1-3).** Part 1 the neuron (weighted sum + threshold, one line). Part 2 why "deep" + the 2012 ImageNet story. Part 3 training as rolling downhill + the black-box tradeoff. Keep each ~5 min. Do NOT read the self-study cards aloud - point to them.
- **18-40 · Apply-along.** Demo 1 the neuron widget (10 min, the anchor). Demo 2 feature-ladder sketch (6 min). Demo 3 black-box vote (6 min).
- **40-45 · Q&A + close.** Land the cheat sheet, tee up Session 3 (embeddings).

## Preflight (do before they walk in)

- Open 02-neural-nets.html, hit "Expand all" once then collapse, toggle Projector zoom on for the room.
- Test the neuron widget once yourself. Pre-know a 100% weight combo so you can rescue anyone stuck: w1 = -1, w2 = 1, bias = 0 separates the default two groups. Drag each dial once so you have felt the line swing and slide.
- Zoom both SVGs once on the projector so you know the click-to-zoom works.

## Never-cut beats

- **Hitting 100% on the neuron = you just trained by hand.** This is the whole session in one moment. When someone clears the red rings, stop and name it: "you just did, with three dials, what a GPU does with millions. That is training." Do not let this pass as a game.
- The one-line loop: "show an example, measure the error, nudge the weights, repeat." Say it as a chant.
- The black-box line: "more layers buy more power and less explanation." Tie it to loan denials vs movie picks.

## Cuts if running long

- Drop Demo 2 (feature ladder) to a 2-min verbal walk-through of the receipt example only.
- Compress the 2012 story to one sentence: "old idea, new fuel - big data plus GPUs."
- Skip Demo 3's fourth vote; do movie rec + tumor flag only.

## Five expected questions

1. **"Is this how the human brain actually works?"** Loosely inspired, not a copy. Real neurons are electrochemical and far messier; the artificial "neuron" borrowed the word and the add-and-fire idea, nothing more. Do not oversell the brain metaphor.
2. **"If it works, why can't we explain it?"** Because the logic lives in millions of weights, not readable rules. No single weight "means" anything; the behavior is the whole soup. That is the black box.
3. **"So is deep learning always better?"** No - callback to Session 1's right-tool test. More power, more cost, less explainability. For structured data with a clear target, classic ML often wins.
4. **"What is a GPU doing that a normal chip can't?"** The same simple arithmetic, thousands of times in parallel. That parallelism is why 2012 happened when it did.
5. **"How much data does training need?"** Depends, but "a lot" - the 2012 leap was as much about ImageNet's millions of labeled images as the model. No clean data, no model (the hierarchy from S1).

## Close

"You opened the black box and found arithmetic. Next session: how machines turn words into meaning they can measure - embeddings."
