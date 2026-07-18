<!-- learn-with-phoebe hub banner -->
> ### 📚 Part of [**Learn with Phoebe**](https://phoebefu6.github.io/learn-with-phoebe/)
> The shelf of 20 free, hands-on courses on AI, data, and the craft around them. **[Browse every course ↗](https://phoebefu6.github.io/learn-with-phoebe/)**
<!-- /learn-with-phoebe hub banner -->

# learn-ai-literacy-with-phoebe

Understand AI and decide with confidence. Eight 45-minute sessions - the sequel to learn-data-literacy - that take leaders and practitioners from neural nets to LLMs to AI strategy. Not how to build models, but what these systems actually do, why they work, where they fail, and when the answer is "do not use AI for this". Every session has one interactive AI toy and no code anywhere.

## Sessions

| # | Title | What you learn | Toy |
|---|-------|----------------|-----|
| 1 | What AI actually is | AI vs ML vs deep learning vs GenAI (nested dolls), the three eras, the right-tool test | Which-doll sorter |
| 2 | Neural nets and deep learning | Neuron = weighted sum + threshold, layers to network, "deep", how training adjusts weights | Be the neuron |
| 3 | Embeddings | Words and images as vectors, similarity as distance, one space powering search + recs + LLMs | Nearest-neighbour explorer |
| 4 | Recommendations | Collaborative vs content-based filtering, cold start, filter bubbles and failure modes | Rate-and-predict sandbox |
| 5 | Search and ranking | Keyword to semantic search, ranking as a weighted signal sum, a first look at RAG | Weight-the-signals tuner |
| 6 | How LLMs work | Next-token prediction, tokens, context window, temperature, why fluent is not factual | Next-token predictor |
| 7 | Using GenAI well | Prompt patterns, RAG, the prompt vs RAG vs fine-tune decision, agents, evals before trust | Weak vs strong prompt lab |
| 8 | AI strategy and risk | Build / buy / API, the five-risk grid, ROI vs hype, governance, the use-case scorecard + memo | Use-case scorecard |

## What it covers (intuition level, no math)

Neural network, CNN, transformer and attention, embeddings and word2vec, collaborative filtering and matrix factorization, semantic search and vector databases, RAG (retrieval-augmented generation), foundation models (GPT, Claude, Gemini, Llama), diffusion, fine-tuning, and agents with tool use. Plus the frameworks a decision-maker needs: the AI-vs-ML nesting, the right-tool test, prompt vs RAG vs fine-tune, build / buy / API, the hallucination / bias / privacy / IP / security risk grid, and human-in-the-loop governance.

## Run locally

```
cd learn-ai-literacy-with-phoebe
python3 -m http.server 8000
```

Then open http://localhost:8000 in a browser.

## Structure

```
learn-ai-literacy-with-phoebe/
  index.html            landing page with paths and difficulty legend
  assets/               style.css, app.js, widgets.js (all 8 AI toys)
  courses/              01-what-ai-is.html ... 08-ai-strategy-and-risk.html
  materials/            course-map.md, presenter notes
```

by Phoebe Fu

This is the sequel to [learn data literacy](https://phoebefu6.github.io/learn-data-literacy-with-phoebe/) - it picks up exactly where that course's "coming next" boundary stopped. New to data itself? Start there first; it sits underneath everything here.

Sibling courses: [learn data literacy](https://phoebefu6.github.io/learn-data-literacy-with-phoebe/) · [learn github](https://phoebefu6.github.io/learn-github-with-phoebe/) · [learn github for builders](https://phoebefu6.github.io/learn-github-for-builders-with-phoebe/) · [learn strategic thinking](https://phoebefu6.github.io/learn-strategic-thinking-with-phoebe/) · [learn claude](https://phoebefu6.github.io/learn-claude-with-phoebe/) · [learn codex](https://phoebefu6.github.io/learn-codex-with-phoebe/) · [learn markdown](https://phoebefu6.github.io/learn-markdown-with-phoebe/) · [learn mermaid](https://phoebefu6.github.io/learn-mermaid-with-phoebe/) · [learn html](https://phoebefu6.github.io/learn-html-with-phoebe/)
