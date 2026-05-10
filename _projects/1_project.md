---
layout: page
title: LLMZip
description: Lossless text compression using large language models
img: 
importance: 1
category: work
related_publications: true
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/llmzip/figure-3-arithmetic-coding.png" title="Arithmetic coding turns predictive probabilities into bits" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Arithmetic coding turns predictive probabilities into bits by successively refining an interval on [0, 1) as symbols arrive.
</div>

LLMZip explores a simple question with broad implications: if a large language model is a strong predictor of the next token in natural language, how much can that predictive distribution help with lossless compression?

The project combines the probability estimates produced by modern language models with classical entropy coding. In this view, the language model supplies a highly adaptive model of English text, while the compression layer turns those probabilities into an exact, reversible code. This creates a bridge between generative AI, information theory, and practical compression systems.

The initial work used LLaMA-7B to estimate an asymptotic upper bound on the entropy of English and to build a compressor that outperformed several strong text-compression baselines in limited experiments {% cite valmeekam2023llmzip %}. The broader research direction asks how far learned predictors can push compression, what computational tradeoffs they introduce, and how these methods can be made robust enough for real systems.

Key themes include:

- Lossless compression with neural predictors.
- Entropy estimation for natural language.
- Connections between language modeling and source coding.
- Practical tradeoffs among compression ratio, latency, and model size.

## Presentations

- Krishna Narayanan, [Plenary talk at ITA 2026](https://ita.ucsd.edu/workshop/), "Compression and Estimation: Transformers and Classical Problems in Information Theory."
- Krishna Narayanan, [Revisiting Compression and Communication through the Lens of Generative AI](https://2025.ieeespawc.org/keynotes/).
