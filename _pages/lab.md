---
layout: page
permalink: /lab/
title: XLab
description: News and selected publications from XLab.
nav: true
nav_order: 2
---

**XLab's core mission: Micro-to-Macro Mechanistic AI** &mdash; building AI systems that connect micro-scale mechanisms to macro-scale behaviors and outcomes, from parameter dynamics in foundation models to physicochemical mechanisms in molecular and biological systems. In fundamental AI, the lab develops parameter-efficient fine-tuning (PEFT) and multimodal foundation models that connect micro-scale parameter dynamics with emergent model behaviors. In AI4Science, the lab combines physicochemical mechanisms with 3D geometric deep learning to reveal molecular-level principles governing biological function, enabling more interpretable molecular discovery and precision medicine.

## News

{% include news.liquid limit=true %}

## Selected Publications

<div class="publications">
{% bibliography --group_by none --query @*[selected=true]* %}
</div>
