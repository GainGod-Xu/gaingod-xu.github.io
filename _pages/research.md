---
layout: page
permalink: /research/
title: Research
description: "Core mission: Micro-to-Macro Mechanistic AI. A few directions define most of my current work; each is anchored by representative papers, with the full list on the publications page."
nav: true
nav_order: 3
---

<style>
  .research-card {
    border-left: 4px solid var(--accent, var(--global-theme-color));
  }
  .research-card > h3 {
    color: var(--accent, var(--global-theme-color));
    scroll-margin-top: 5rem;
  }

  /* Micro-to-Macro flow diagram */
  .m2m {
    margin: 1.5rem 0 0.5rem;
  }
  .m2m-head,
  .m2m-row {
    display: grid;
    grid-template-columns: 8.5rem 1fr 1.5rem 1fr 1.5rem 1fr;
    align-items: stretch;
    gap: 0.4rem;
  }
  .m2m-head {
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--global-text-color-light);
    margin-bottom: 0.35rem;
  }
  .m2m-row {
    margin-bottom: 0.6rem;
  }
  .m2m-label {
    display: flex;
    align-items: center;
    padding: 0.5rem 0.7rem;
    border-radius: 6px;
    background: var(--accent);
    color: #fff !important;
    font-weight: 700;
    font-size: 0.92rem;
    line-height: 1.2;
    text-decoration: none !important;
  }
  .m2m-label:hover {
    filter: brightness(1.1);
  }
  .m2m-step {
    padding: 0.5rem 0.7rem;
    border: 1px solid var(--global-divider-color);
    border-left: 3px solid var(--accent);
    border-radius: 6px;
    background: var(--global-card-bg-color);
    font-size: 0.85rem;
    line-height: 1.35;
  }
  .m2m-step:last-child {
    background: color-mix(in srgb, var(--accent) 10%, var(--global-card-bg-color));
  }
  .m2m-arrow {
    display: flex;
    align-items: center;
    justify-content: center;
    color: var(--accent);
    font-weight: 700;
  }
  .m2m-base {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem 1.5rem;
    justify-content: center;
    margin-top: 0.3rem;
    padding: 0.5rem 0.7rem;
    border-top: 1px dashed var(--global-divider-color);
    font-size: 0.85rem;
    color: var(--global-text-color-light);
  }
  .m2m-base a {
    font-weight: 600;
  }
  @media (max-width: 640px) {
    .m2m-head {
      display: none;
    }
    .m2m-row {
      grid-template-columns: 1fr;
      margin-bottom: 1.2rem;
    }
    .m2m-step::before {
      content: attr(data-stage);
      display: block;
      font-size: 0.68rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--global-text-color-light);
    }
    .m2m-arrow {
      transform: rotate(90deg);
      line-height: 1;
    }
  }
</style>

<figure class="m2m" aria-label="Micro-to-Macro Mechanistic AI: how each research direction links micro-scale mechanisms to macro-scale behavior">
  <div class="m2m-head" aria-hidden="true">
    <span></span><span>Micro-scale mechanism</span><span></span><span>Mechanistic model</span><span></span><span>Macro-scale behavior</span>
  </div>
  <div class="m2m-row" style="--accent: #3a7bd5;">
    <a class="m2m-label" href="#ai-for-science">AI for Science</a>
    <div class="m2m-step" data-stage="Micro-scale mechanism">Atoms, non-covalent interactions, spectra, evolutionary sequence context</div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step" data-stage="Mechanistic model">Physics-grounded geometric deep learning and biological language models</div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step" data-stage="Macro-scale behavior">Binding, RNA modification, and molecular structure&mdash;explained, not just predicted</div>
  </div>
  <div class="m2m-row" style="--accent: #d9534f;">
    <a class="m2m-label" href="#ai4health">AI4Health</a>
    <div class="m2m-step" data-stage="Micro-scale mechanism">Multi-omics, medical imaging, and EHR signals</div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step" data-stage="Mechanistic model">Explainable, multimodal foundation models</div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step" data-stage="Macro-scale behavior">Clinical prediction and diagnosis</div>
  </div>
  <div class="m2m-row" style="--accent: #7b52c7;">
    <a class="m2m-label" href="#ai-fundamentals">AI Fundamentals</a>
    <div class="m2m-step" data-stage="Micro-scale mechanism">Parameter directions and gradient sensitivities</div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step" data-stage="Mechanistic model">Structured, task-aware low-rank adaptation and counterfactual alignment</div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step" data-stage="Macro-scale behavior">Reliable, efficient, visually grounded model behavior</div>
  </div>
  <div class="m2m-base">
    <span>Foundation: <a href="#ai-fundamentals">AI</a> + <a href="#chemistry">Chemistry</a> + <a href="#ai4health">Medicine</a></span>
    <span>Next: <a href="#emerging-direction">quantum computing for discovery</a></span>
  </div>
</figure>

<div class="card research-card mt-3 p-4" markdown="1" style="--accent: #3a7bd5;">

### AI for Science

Embedding atomic-level physical and chemical mechanisms&mdash;spectral properties, atom interactions, evolutionary sequence context&mdash;directly into deep networks, so models predict molecular properties and structures through physically grounded reasoning rather than superficial correlations.

- **ExplainBind: Explainable Physicochemical Determinants of Protein-Ligand Binding via Non-Covalent Interactions.** Meng, Z.<sup>&dagger;</sup>, Bai, Z.<sup>&dagger;</sup>, et al., Oldham, W. M.\*, Meng, Z.\*, *Xu, H.*\*, Loscalzo, J. *bioRxiv*, 2026.
- **EvoRMD: Integrating Biological Context and Evolutionary RNA Language Models for Interpretable Prediction of RNA Modifications.** Wang, B., Zhang, H., Cui, T., Wang, X., Song, J.\*, *Xu, H.*\* *Genome Biology*, 2026.
- **How Well Can Off-the-Shelf LLMs Elucidate Molecular Structures from Mass Spectra Using Chain-of-Thought Reasoning?** Wang, Y., Lu, W., Liu, L., *Xu, H.*\*, Ling, H.\* *J. Cheminform.*, 2026.
- **TransPeakNet for Solvent-Aware 2D NMR Prediction via Multi-Task Pre-Training and Unsupervised Learning.** Li, Y.<sup>&dagger;</sup>, *Xu, H.*<sup>&dagger;</sup>, Kumar, A., Wang, D., Heiss, C., Azadi, P., Hong, P.\* *Communications Chemistry*, 2025.

</div>

<div class="card research-card mt-3 p-4" markdown="1" style="--accent: #d9534f;">

### AI4Health

Developing foundational models and explainable frameworks for multi-omics, medical imaging, and electronic health records (EHR)&mdash;individually and in multimodal combination&mdash;to advance clinical prediction and diagnosis.

- **Deep Learning-Based MRI Model for Predicting P53-Mutated Hepatocellular Carcinoma.** Jia, L., Yang, Q., Jiang, H., Huang, G., Wang, Z., Guo, X., Li, J., *Xu, H.*\*, Lei, J.\* *BMC Medical Imaging*, 2025.

</div>

<div class="card research-card mt-3 p-4" markdown="1" style="--accent: #7b52c7;">

### AI Fundamentals

Parameter-efficient fine-tuning and multimodal alignment methods that preserve fine-grained gradient sensitivities, so adaptation stays reliable, interpretable, and cheap to train at scale.

- **Not All Directions Matter: Toward Structured and Task-Aware Low-Rank Adaptation.** Xiao, X., et al., *Xu, H.* *ACL*, 2026.
- **Staying VIGILant: Mitigating Visual Laziness via Counterfactual Visual Alignment in MLLMs.** Xiao, X., et al., *Xu, H.* *ECCV*, 2026.

</div>

<div class="card research-card mt-3 p-4" markdown="1" style="--accent: #3fa65b;">

### Chemistry

Earlier work on cobalt-catalyzed asymmetric radical reactions and total synthesis&mdash;the physical-organic-chemistry foundation that now informs how I build mechanism-aware AI models.

- **Enantioselective Radical *N*-Heterobicyclization by New Mode of Asymmetric Induction via Kinetically Stable Chiral Radical Center.** *Xu, H.*, Wang, D.-S., Zhu, Z.-Y., Deb, A., Zhang, X. P.\* *Chem*, 2024.

</div>

<div class="card research-card mt-3 p-4" markdown="1" style="--accent: #d9a441;">

### Emerging Direction

**Quantum Computing for Scientific Discovery** &mdash; exploring where quantum algorithms can accelerate simulation and search in molecular and biological discovery pipelines. Publications forthcoming.

</div>
