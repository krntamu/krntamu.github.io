---
layout: page
title: Unsourced Random Access
description: Massive multiple access methods for 6G and machine-type communication
img: 
importance: 5
category: work
related_publications: true
---

Unsourced random access is motivated by massive machine-type communication, where a base station may need to recover a list of short messages from a large population of devices without first identifying which devices are active.

This project studies coding and signal-processing methods for the unsourced multiple access channel. The setting is especially relevant to future 6G systems, internet-of-things deployments, and sporadic traffic patterns where conventional scheduling and identity-centric access can be inefficient.

Very recent work shows how to achieve robustness to delay spread and Doppler by combining Orthogonal Time Frequency Signalling (OTFS) with irregular repetition slotted ALOHA {% cite mirri2026zak %}

Recent work examines the role of asynchrony in unsourced MACs {% cite fengler2023advantages %} and connects unsourced access ideas to the evolution of two-step random access procedures in 5G New Radio {% cite agostini2024evolution agostini2024enhancements chamberland2025density %}. These projects aim to clarify both the information-theoretic limits and the standardization-facing design choices. {% chamberland2025density %} received the 2025 best paper award at the IEEE SPAWC conference.

The research blends random access protocol design, coding theory, finite-blocklength analysis, and practical constraints from cellular systems.
