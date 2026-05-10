---
layout: page
title: LLM Watermarking
description: Information-theoretic methods for watermarking and steganography in LLM-generated text
img: assets/img/projects/llm-watermarking/cover.png
importance: 4
category: work
related_publications: true
---

Large language models make it easy to generate fluent text at scale, which raises two closely related information-theoretic questions: how can hidden information be embedded in generated text without changing its apparent naturalness, and how can generated text carry a reliable watermark that can later be detected or decoded?

This project studies LLM watermarking and linguistic steganography through the lens of probability distributions, entropy, divergence constraints, and sequential decision-making. The goal is to design methods that are mathematically analyzable while remaining compatible with practical text generation.

One direction is coverless steganography, where an LLM and arithmetic coding are used together to generate stego-text that carries secret message bits. OD-Stega formulates the token-level embedding problem as the optimization of a replacement next-token distribution: maximize embedding efficiency while constraining the divergence from the original LLM distribution. The resulting optimized distribution admits closed-form solutions under KL-divergence and total-variation constraints, and the work also addresses practical issues such as tokenization mismatch, vocabulary truncation, and compatibility with sequence-level selection methods {% cite huang2026od %}.

Another direction treats steganographic text generation as a sequential control problem. Rather than optimizing each token in isolation, relatively secure LLM-based steganography via constrained Markov decision processes models the long-term effect of distribution changes across a generated sequence. This leads to a finite-dimensional convex optimization problem with a closed-form optimal policy, showing when the encoder should spend its divergence budget and why decisions should account for future transition structure rather than only the current token distribution {% cite huang2025relatively %}.

A third direction studies multi-bit generative watermarking for LLMs under worst-case false-alarm constraints. Recent work shows that a previously proposed finite-token construction is suboptimal, then gives two encoding-decoding schemes that attain the lower bound on misdetection probability. This characterizes the optimal multi-bit watermarking performance under the model, formulates the design as a linear program, and identifies the structural conditions under which optimality is achieved {% cite huang2026optimal %}.

Together, these results connect generative AI safety with classical information-theoretic ideas: entropy coding, hypothesis testing, constrained optimization, and finite-blocklength tradeoffs.
