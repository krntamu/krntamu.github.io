---
layout: page
title: AI-Native Wireless Communications
description: Learning-driven models and algorithms for future wireless systems
img: assets/img/3.jpg
importance: 2
category: work
giscus_comments: true
related_publications: true
---

Future wireless systems will need to adapt to rapidly changing channels, heterogeneous devices, and new traffic patterns created by distributed AI, sensing, robotics, and immersive media. This project studies wireless communication as an AI-native system rather than as a fixed pipeline with isolated learning components.

One thrust studies how Transformers and in-context learning can act as estimators for wireless channels and signals. The goal is to understand when sequence models can adapt from examples at inference time, how their behavior relates to classical estimators, and what guarantees can be proved for communication settings {% cite kunde2023transformers %}.

Another thrust focuses on receiver adaptation without gradients. In-context learning offers a way for receivers to adjust to new environments using only observed examples, which is especially attractive when explicit channel models are unavailable or hardware constraints make conventional adaptation difficult {% cite zecchin2025context %}.

This work connects machine learning, signal processing, and information theory. The central objective is to design communication systems that learn from context while still retaining the reliability and interpretability expected in engineered wireless infrastructure.
