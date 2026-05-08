---
layout: page
title: Sparse Regression LDPC Codes
description: Coding theory for reliable communication and storage
img:
importance: 4
category: work
related_publications: true
---

Sparse regression LDPC codes bring together ideas from sparse superposition coding, low-density parity-check codes, and iterative decoding. The project studies code constructions that preserve the algorithmic advantages of sparse graphical models while achieving strong performance in communication and storage settings.

The work develops code ensembles, decoding algorithms, and performance analysis for sparse regression LDPC codes {% cite ebert2024sparse %}. A key theme is designing codes whose structure supports efficient inference, making them attractive for large-scale systems where reliability and computational cost both matter.

This line of research also extends to multi-user settings. Coded demixing provides a way to separate simultaneously transmitted sparse codewords and is useful in cell-free and distributed wireless architectures where many devices may share the same communication resources {% cite ebert2024multi %}.

The broader goal is to build coding schemes that are mathematically analyzable, implementation-conscious, and well matched to the traffic patterns of modern networks.
