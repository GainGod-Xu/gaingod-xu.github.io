---
layout: page
permalink: /research/
title: Research
description: "Trustworthy world models for life science: current directions, organized from molecular recognition to system-level biology, each anchored by representative papers."
nav: true
nav_order: 2
---

<style>
  .rcard {
    margin-top: 1.1rem; padding: 1.1rem 1.3rem;
    border: 1px solid var(--global-divider-color); border-left: 4px solid var(--global-theme-color); border-radius: 8px;
  }
  .rcard h3 { margin: 0 0 0.2rem; font-size: 1.15rem; font-weight: 700; scroll-margin-top: 5rem; }
  .rcard .scale { font-size: 0.74rem; font-weight: 700; letter-spacing: 0.08em; text-transform: uppercase; color: var(--global-theme-color); margin-bottom: 0.5rem; }
  .rcard p { font-size: 0.95rem; line-height: 1.55; }
  .rcard ul { margin: 0.5rem 0 0; padding-left: 1.1rem; font-size: 0.88rem; }
  .rcard li { margin-bottom: 0.3rem; }
  .rcard.future { border-left-style: dashed; }
  .rcard.past { border-left-color: var(--global-divider-color); }
  .rcard.past .scale { color: var(--global-text-color-light); }
  .r-intro { font-size: 1.02rem; line-height: 1.6; max-width: 46rem; }
  .r-nav { display: flex; flex-wrap: wrap; gap: 0.4rem; margin: 0.8rem 0 0.4rem; font-size: 0.85rem; }
  .r-nav a { padding: 0.15rem 0.7rem; border-radius: 999px; border: 1px solid var(--global-divider-color); text-decoration: none !important; }
</style>

<p class="r-intro">I build trustworthy AI systems to understand how biological interventions propagate across scales. The directions below move from molecules to interactions, networks, and cells; each asks a version of the same three questions&mdash;<strong>understand</strong>, <strong>predict</strong>, <strong>intervene</strong>&mdash;and each is held to the same standard of interpretability, uncertainty, robustness, generalization, and mechanistic consistency. The <a href="{{ '/#map' | relative_url }}">research map</a> on the home page shows how they fit together.</p>

<div class="r-nav">
  <a href="#molecular-recognition">Molecular recognition</a>
  <a href="#rna-biology">RNA biology</a>
  <a href="#molecular-representation">Molecular representation</a>
  <a href="#structure-elucidation">Structure elucidation</a>
  <a href="#network-medicine">Network medicine</a>
  <a href="#trustworthy-methods">Trustworthy methods</a>
  <a href="#toward-world-models">Toward world models</a>
  <a href="#foundations">Foundations</a>
</div>

<div class="rcard" markdown="1">
<div class="scale">Interaction &middot; Understand</div>

### Molecular recognition and biomolecular interactions {#molecular-recognition}

How do small molecules recognize proteins and RNA? ExplainBind predicts protein&ndash;ligand binding through explicit non-covalent interactions, so each prediction exposes its physicochemical determinants rather than a bare score. Ongoing work extends the same mechanistic framing to RNA&ndash;ligand recognition.

- **ExplainBind: Explainable Physicochemical Determinants of Protein-Ligand Binding via Non-Covalent Interactions.** Meng, Z.<sup>&dagger;</sup>, Bai, Z.<sup>&dagger;</sup>, et al., Oldham, W. M.\*, Meng, Z.\*, *Xu, H.*\*, Loscalzo, J. *bioRxiv*, 2026.
</div>

<div class="rcard" markdown="1">
<div class="scale">Interaction &middot; Predict</div>

### RNA biology and modification {#rna-biology}

RNA modifications sit between sequence and function. EvoRMD integrates biological context with evolutionary RNA language models to predict modification sites interpretably, a step toward modeling how interventions on RNA propagate to cellular state.

- **EvoRMD: Integrating Biological Context and Evolutionary RNA Language Models for Interpretable Prediction of RNA Modifications.** Wang, B., Zhang, H., Cui, T., Wang, X., Song, J.\*, *Xu, H.*\* *Genome Biology*, 2026.
</div>

<div class="rcard" markdown="1">
<div class="scale">Molecule &middot; Understand / Predict</div>

### Multimodal molecular representation {#molecular-representation}

Chemical structure is observed through complementary views: graphs, spectra, text, and 3D geometry. Aligning these modalities yields representations that transfer to property prediction and drug discovery while staying consistent with chemistry.

- **Advancing Drug Discovery with Enhanced Chemical Understanding via Asymmetric Contrastive Multimodal Learning.** Wang, Y.<sup>&dagger;</sup>, Li, Y.<sup>&dagger;</sup>, Liu, L., Hong, P., *Xu, H.*\* *J. Chem. Inf. Model.*, 2025.
- **Multimodal Fusion with Relational Learning for Molecular Property Prediction.** Zhou, Z.\*, Li, Y., Hong, P., *Xu, H.*\* *Communications Chemistry*, 2025.
- **Mat-Instructions: A Large-Scale Inorganic Material Instruction Dataset for Large Language Models.** Liu, K., et al., *Xu, H.* *IJCAI*, 2025.
</div>

<div class="rcard" markdown="1">
<div class="scale">Molecule &middot; Understand</div>

### Structure elucidation from spectra (NMRScape) {#structure-elucidation}

Determining a molecule's structure from its spectra is a problem where a model must be able to check its own answer. This line builds solvent-aware 2D NMR prediction, an annotated experimental benchmark, and reasoning-based elucidation toward self-verifying structure determination.

- **TransPeakNet for Solvent-Aware 2D NMR Prediction via Multi-Task Pre-Training and Unsupervised Learning.** Li, Y.<sup>&dagger;</sup>, *Xu, H.*<sup>&dagger;</sup>, et al., Hong, P.\* *Communications Chemistry*, 2025.
- **2DNMRGym: An Annotated Experimental Dataset for Atom-Level Molecular Representation Learning in 2D NMR via Surrogate Supervision.** Li, Y.<sup>&dagger;</sup>, *Xu, H.*<sup>&dagger;</sup>, Hong, P. *LoG*, 2025.
- **How Well Can Off-the-Shelf LLMs Elucidate Molecular Structures from Mass Spectra Using Chain-of-Thought Reasoning?** Wang, Y., Lu, W., Liu, L., *Xu, H.*\*, Ling, H.\* *J. Cheminform.*, 2026.
</div>

<div class="rcard" markdown="1">
<div class="scale">Network &middot; Understand / Intervene</div>

### Network medicine and systems pharmacology {#network-medicine}

Molecular interactions act through networks. Connecting binding and interactome structure to disease modules provides the route from a single intervention to a system-level response, and the basis for principled drug repurposing. Ongoing work builds affinity-weighted protein&ndash;protein interaction networks.

- **Systems Chemical Biology: Integrating Medicinal Chemistry and Systems Biology for Drug Discovery.** Wang, R., *Xu, H.*, Loscalzo, J. In *Comprehensive Medicinal Chemistry*, Elsevier, 2025.
- **Modern Computational Methods for Drug Repurposing.** *Xu, H.*, Loscalzo, J.\* *Drug Repurposing*, 2026.
- **Deep Learning-Based MRI Model for Predicting P53-Mutated Hepatocellular Carcinoma.** Jia, L., et al., *Xu, H.*\*, Lei, J.\* *BMC Medical Imaging*, 2025.
</div>

<div class="rcard" markdown="1">
<div class="scale">Methods &middot; Trustworthiness</div>

### Trustworthy foundation-model methods {#trustworthy-methods}

Scientific data are scarce and shift across experiments, so the foundation models behind these systems must adapt cheaply and remain reliable. This work studies which parameter directions matter during adaptation and how to keep multimodal models grounded in their inputs.

- **Not All Directions Matter: Toward Structured and Task-Aware Low-Rank Adaptation.** Xiao, X., et al., *Xu, H.* *ACL*, 2026.
- **Staying VIGILant: Mitigating Visual Laziness via Counterfactual Visual Alignment in MLLMs.** Xiao, X., et al., *Xu, H.* *ECCV*, 2026.
- **HyperAdaLoRA: Accelerating LoRA Rank Allocation During Training via Hypernetworks without Sacrificing Performance.** Zhang, H., et al., *Xu, H.* *Findings of ACL*, 2026.
- **Sensitivity-LoRA: Low-Load Sensitivity-Based Fine-Tuning for Large Language Models.** Zhang, H., et al., *Xu, H.* *Findings of EMNLP*, 2025.
</div>

<div class="rcard future" markdown="1">
<div class="scale">Cell &middot; Phenotype &middot; Planned</div>

### Toward world models of biological response {#toward-world-models}

The next step is to close the loop from molecule to phenotype: perturbation biology and single-cell response modeling, cross-scale state transitions, and inverting these models to design precision interventions. Each stage will carry explicit uncertainty and be tested for consistency with known mechanisms.
</div>

<div class="rcard past" markdown="1">
<div class="scale">Foundations</div>

### Chemistry {#foundations}

Earlier work in cobalt-catalyzed asymmetric radical reactions and total synthesis is the physical-organic foundation for building mechanism-aware models.

- **Enantioselective Radical *N*-Heterobicyclization by New Mode of Asymmetric Induction via Kinetically Stable Chiral Radical Center.** *Xu, H.*, Wang, D.-S., Zhu, Z.-Y., Deb, A., Zhang, X. P.\* *Chem*, 2024.
- **Metalloradical Activation of Carbonyl Azides for Enantioselective Radical Aziridination of Alkenes.** Riart-Ferrer, X., et al., *Xu, H.*, et al., Zhang, X. P.\* *Chem*, 2021.
</div>
