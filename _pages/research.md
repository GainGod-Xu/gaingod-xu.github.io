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

  /* Micro-to-Macro flow (compact) */
  .m2m {
    margin: 1.5rem 0 0.5rem;
  }
  .m2m-flow {
    display: grid;
    grid-template-columns: 1fr auto 1fr auto 1fr;
    align-items: stretch;
    gap: 0.5rem;
  }
  .m2m-step {
    padding: 0.7rem 0.9rem;
    border: 1px solid var(--global-divider-color);
    border-top: 3px solid var(--global-theme-color);
    border-radius: 8px;
    background: var(--global-card-bg-color);
    text-align: center;
  }
  .m2m-step strong {
    display: block;
    font-weight: 700;
  }
  .m2m-step span {
    font-size: 0.82rem;
    color: var(--global-text-color-light);
  }
  .m2m-arrow {
    display: flex;
    align-items: center;
    color: var(--global-theme-color);
    font-size: 1.3rem;
    font-weight: 700;
  }
  .m2m-dirs {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 0.4rem;
    margin-top: 0.9rem;
    font-size: 0.85rem;
    color: var(--global-text-color-light);
  }
  .m2m-dirs a {
    padding: 0.15rem 0.7rem;
    border-radius: 999px;
    border: 1.5px solid var(--accent);
    color: var(--accent) !important;
    font-weight: 600;
    text-decoration: none !important;
  }
  .m2m-dirs a:hover {
    background: color-mix(in srgb, var(--accent) 12%, transparent);
  }
  @media (max-width: 640px) {
    .m2m-flow {
      grid-template-columns: 1fr;
    }
    .m2m-arrow {
      justify-content: center;
      transform: rotate(90deg);
    }
  }
</style>

<figure class="m2m" aria-label="Micro-to-Macro Mechanistic AI: micro-scale mechanisms, mechanistic AI models, macro-scale behavior">
  <div class="m2m-flow">
    <div class="m2m-step"><strong>Micro-scale mechanisms</strong><span>atoms &middot; interactions &middot; parameters</span></div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step"><strong>Mechanistic AI models</strong><span>physically and structurally grounded</span></div>
    <div class="m2m-arrow" aria-hidden="true">&rarr;</div>
    <div class="m2m-step"><strong>Macro-scale behavior</strong><span>function &middot; health &middot; reliability</span></div>
  </div>
  <div class="m2m-dirs">
    <a href="#ai-for-science" style="--accent: #3a7bd5;">AI for Science</a>
    <a href="#ai4health" style="--accent: #d9534f;">AI4Health</a>
    <a href="#ai-fundamentals" style="--accent: #7b52c7;">AI Fundamentals</a>
    <a href="#chemistry" style="--accent: #3fa65b;">Chemistry</a>
    <a href="#emerging-direction" style="--accent: #d9a441;">Quantum (emerging)</a>
  </div>
  <div class="m2m-dirs">Foundation: AI + Chemistry + Medicine</div>
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
