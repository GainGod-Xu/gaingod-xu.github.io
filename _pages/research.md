---
layout: page
permalink: /research/
title: Research
description: "Core mission: Micro-to-Macro Mechanistic AI. A few directions define most of my current work; each is anchored by representative papers, with the full list on the publications page."
nav: true
nav_order: 3
---

### AI for Science

Embedding atomic-level physical and chemical mechanisms&mdash;spectral properties, atom interactions, evolutionary sequence context&mdash;directly into deep networks, so models predict molecular properties and structures through physically grounded reasoning rather than superficial correlations.

<div class="publications">
{% bibliography --group_by none --query @*[research=ai4science]* %}
</div>

### AI4Health

Developing foundational models and explainable frameworks for multi-omics, medical imaging, and electronic health records (EHR)&mdash;individually and in multimodal combination&mdash;to advance clinical prediction and diagnosis.

<div class="publications">
{% bibliography --group_by none --query @*[research=ai4health]* %}
</div>

### AI Fundamentals

Parameter-efficient fine-tuning and multimodal alignment methods that preserve fine-grained gradient sensitivities, so adaptation stays reliable, interpretable, and cheap to train at scale.

<div class="publications">
{% bibliography --group_by none --query @*[research=aifundamentals]* %}
</div>

### Chemistry

Earlier work on cobalt-catalyzed asymmetric radical reactions and total synthesis&mdash;the physical-organic-chemistry foundation that now informs how I build mechanism-aware AI models.

<div class="publications">
{% bibliography --group_by none --query @*[research=chemistry]* %}
</div>

### Emerging Direction

**Quantum Computing for Scientific Discovery** &mdash; exploring where quantum algorithms can accelerate simulation and search in molecular and biological discovery pipelines. Publications forthcoming.
