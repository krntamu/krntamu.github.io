---
layout: page
title: Over-the-Air Federated Learning
description: Communication-efficient scheduling and computation for distributed learning
img: 
importance: 
category: hidden
giscus_comments: true
related_publications: true
---

Federated learning pushes model training toward distributed devices, but wireless communication can become the bottleneck. Over-the-air computation offers a different design principle: use the superposition property of the wireless channel to aggregate updates directly during transmission.

This project studies how to select users and computations so that wireless aggregation supports reliable and timely learning. Computation selection asks which devices should transmit at a given time so the resulting over-the-air signal is useful for federated optimization {% cite nazer2024computation %}.

The work connects distributed learning, wireless scheduling, and analog computation. It is part of a broader effort to make communication systems serve AI workloads directly, rather than merely transporting bits for them.

Key goals include reducing communication overhead, improving robustness to channel variation, and developing scheduling policies that balance learning progress with wireless resource constraints.
