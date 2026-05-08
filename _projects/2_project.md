---
layout: page
title: AI-Native Wireless Communications
description: Learning-driven models and algorithms for future wireless systems
img: assets/img/projects/ai-native/cover.png
importance: 2
category: work
giscus_comments: true
related_publications: true
---

Future wireless systems will need to adapt to rapidly changing channels, heterogeneous devices, and new traffic patterns created by distributed AI, sensing, robotics, and immersive media. This project studies wireless communication as an AI-native system rather than as a fixed pipeline with isolated learning components.

**Thrust 1: Transformers as adaptive in-context wireless estimators.** One thrust studies how Transformers and in-context learning can act as estimators for wireless channels and signals. The goal is to understand when sequence models can adapt from examples at inference time, how their behavior relates to classical estimators, and what guarantees can be proved for communication settings {% cite kunde2023transformers %}. 

This thrust focuses on receiver adaptation without gradients. In-context learning offers a way for receivers to adjust to new environments using only observed examples, which is especially attractive when explicit channel models are unavailable or hardware constraints make conventional adaptation difficult {% cite zecchin2025context %}.

**Thrust 2: Generative priors for semi-blind channel estimation.** A second direction uses diffusion models as learned priors for wireless channels, while retaining the physical structure of classical estimation problems. In GRAM-DIFF, the receiver combines a pretrained angular-domain diffusion prior with pilot likelihood information and a data-derived estimate of the channel Gram matrix. The Gram matrix supplies realization-level second-order structure from received data symbols, so the reverse diffusion process is guided by both known pilots and semi-blind information from the payload. On 3GPP and QuaDRiGa channel models, this approach improves normalized mean-squared error over deterministic diffusion baselines and remains robust when coherence-time constraints make the Gram estimate noisy {% cite wang2026gramdiff %}.

This idea also extends to unsourced random access, where many devices transmit short packets through non-orthogonal pilots and multi-user superposition. In that setting, Gram-guided diffusion provides a data-driven alternative to least-squares and sample-covariance LMMSE estimators. The method uses the detected pilot matrix together with received data symbols to guide channel generation, and simulations show substantial gains over classical baselines for multi-antenna random access receivers {% cite wang2026semiblindura %}.

This work connects machine learning, signal processing, and information theory. The central objective is to design communication systems that learn from context while still retaining the reliability and interpretability expected in engineered wireless infrastructure.
