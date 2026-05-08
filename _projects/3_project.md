---
layout: page
title: Neural Joint Source-Channel Coding
description: End-to-end learned representations for compression and communication
img: assets/img/7.jpg
importance: 3
category: work
related_publications: true
---

Joint source-channel coding revisits a foundational communication problem: instead of compressing data and then separately protecting it against channel noise, can the representation be designed end to end for the source, the channel, and the final task?

This project develops neural and information-theoretic approaches to communication under distortion, perception, and reliability constraints. Neural architectures can learn representations that degrade gracefully, exploit structure in the source, and adapt to operating regimes where classical separation-based designs are not ideal.

The research is closely tied to emerging questions in semantic communication and generative compression, where the receiver may care not only about bitwise recovery but also about the perceptual or task-level quality of the reconstruction. Recent work on source-channel separation for distortion-perception coding provides a theoretical lens for understanding when separation remains optimal and when new designs are needed {% cite tian2025source %}.

The long-term goal is a principled toolkit for learned communication systems that combines the flexibility of neural representations with the guarantees and design discipline of information theory.
