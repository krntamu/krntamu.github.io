---
layout: page
title: Over-the-Air Neural Group Testing
description: Learning-based sparse activity detection over wireless channels
img: assets/img/4.jpg
importance: 7
category: work
related_publications: true
---

Many wireless and sensing problems involve detecting a small active subset from a much larger population. Group testing provides a natural abstraction for this sparse recovery problem, while wireless channels add noise, interference, and physical-layer constraints.

This project develops neural group-testing methods that operate over the air. Rather than treating communication and detection as separate stages, the approach learns testing and decoding strategies that are shaped by the channel itself {% cite valmeekam2024over %}.

The setting is relevant to activity detection, random access, distributed sensing, and low-latency inference at the wireless edge. It also creates a useful testbed for understanding when neural designs can improve on handcrafted schemes in sparse inference problems.

The broader research question is how to co-design measurement, transmission, and inference so that the physical channel becomes part of the computation rather than only an obstacle to be overcome.
