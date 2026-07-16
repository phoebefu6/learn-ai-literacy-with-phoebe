# learn-ai-literacy-with-phoebe - course map

The sequel to learn-data-literacy-with-phoebe. It picks up exactly where that course's "not covered by design" boundary stops: deep learning, embeddings, recommendations, search, and GenAI/LLMs.
Audience: **mixed - business leaders + practitioners**. Core voice is decision-maker literacy (what AI is, when to trust it, when NOT to use it); a light practitioner lane in S6-S7 (prompt patterns, RAG shapes). No code required; practitioners get slightly deeper cards tagged Self-study.
Format: 8 sessions x 45 min (3 welcome / ~15 concepts / ~22 apply-along / 5 Q&A).
Design: electric violet + cyan. Ramp deep #4C1D95 / primary #6D28D9 / mid #7C3AED / soft #C4B5FD / tint #EDE9FE; flagship cyan #06B6D4; ink #1E1B2E; code-bg #14082E.
Interactivity: no code. 8 in-page widgets (assets/widgets.js), 6 built new for this course.

## Session map

| # | Title | Diff | Core content | Widget |
|---|-------|------|--------------|--------|
| 1 | What AI actually is | 🟢 | AI vs ML vs deep learning vs GenAI (nested dolls); narrow vs general (AGI myth-check); the 3 eras (rules -> ML -> foundation models); the right-tool test (when a spreadsheet/rule beats a model); AI Hierarchy of Needs (Rogati, callback to data-literacy) | sorter: AI or not-AI / right-tool |
| 2 | Neural nets and deep learning | 🟢 | neuron = weighted sum + threshold; layers -> network; "deep" = many layers; training = adjust weights from labeled examples (gradient descent at intuition); what changed ~2012 (ImageNet + GPUs + data); CNNs for vision, the black-box/explainability tradeoff | neuron: tune weights to separate 2 classes |
| 3 | Embeddings: how machines read meaning | 🟡 | turning words/images into vectors; similarity = distance in meaning-space; king-man+woman=queen; why one embedding space powers search + recs + LLMs; vector databases at intuition | embedding: click a word, see nearest neighbors |
| 4 | Recommendations | 🟡 | collaborative filtering (people like you) vs content-based (items like this); matrix factorization intuition; the Netflix/Amazon/Spotify/TikTok engines; cold start; filter bubbles + engagement-optimization failure modes | recsandbox: rate items, watch it predict |
| 5 | Search and ranking | 🟡 | keyword -> semantic search (embeddings again); ranking = weighted signal sum (relevance/freshness/popularity/personalization); there is no objective #1; RAG preview (retrieval feeding an LLM); search quality = data quality | rankingtuner: weight signals, reorder results |
| 6 | How LLMs work | 🟠 | next-token prediction; training vs inference; tokens; context window; temperature; why they hallucinate (fluent != factual); transformers/attention at intuition; prompt = steering not programming | tokenpredictor: pick next token, feel temperature |
| 7 | Using GenAI well | 🟠 | prompt patterns (role, constraints, examples, format); RAG for grounding in your data; the prompt vs RAG vs fine-tune decision; agents + tools at intuition; evals (how you know it works); cost + latency literacy | promptlab: weak vs strong prompt, same task |
| 8 | AI strategy and risk | 🔴 | build/buy/API decision; where AI ROI is real vs hype; the risk grid (hallucination/bias/privacy/IP/security); human-in-the-loop governance; capstone: an AI use-case scorecard + adoption memo; honest boundary: this is literacy, not an ML engineering course | checklist: AI-readiness + use-case scorecard |

## Models / concepts to recognize (all intuition tier, no math)

Neural network · CNN (vision) · RNN/LSTM (sequence, historical) · **Transformer** (the architecture behind modern GenAI) · embeddings / word2vec · collaborative filtering · matrix factorization · semantic search / vector DB · RAG (retrieval-augmented generation) · foundation models (GPT, Claude, Gemini, Llama) · diffusion (image generation) · fine-tuning / LoRA · agents + tool use · attention

## Frameworks

AI-vs-ML-vs-GenAI nesting · the right-tool test · AI Hierarchy of Needs (Rogati) · train/inference split · prompt-vs-RAG-vs-finetune decision tree · build/buy/API · human-in-the-loop governance · hallucination/bias/privacy/IP/security risk grid · AI use-case ROI matrix · eval-before-trust

## Widgets (assets/widgets.js)

NEW (6): neuron, embedding, recsandbox, rankingtuner, tokenpredictor, promptlab. REUSED from the shared engine: sorter (S1), checklist (S8). Terminal-style boxes via .termbox where showing prompts.

## Not covered by design

The math (backprop, loss functions, linear algebra) · training your own models / MLOps · coding with the APIs (that is a builder course) · agent framework specifics · prompt-injection security depth (named in the risk grid only) · which vendor to buy (framework given, not a recommendation). This is literacy: understand, evaluate, decide, govern - not build.
