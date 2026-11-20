---
layout: plain
permalink: /research/
title: Research
description: "Research program: trustworthy world models for life science, built one biological scale at a time."
nav: true
nav_order: 2
---

<style>
  .plain h1, .plain h2, .plain h3 { letter-spacing: -0.01em; }
  .rs-hero { display: grid; grid-template-columns: minmax(0, 0.95fr) minmax(300px, 1.05fr); gap: 2.6rem; align-items: center; padding: 2.4rem 0 3.2rem; }
  .rs-hero h1 { font-size: clamp(2rem, 4.4vw, 2.8rem); font-weight: 650; line-height: 1.1; margin: 0 0 1rem; max-width: 18ch; }
  .rs-hero .lead { font-size: 1.05rem; line-height: 1.6; max-width: 34rem; margin: 0; }
  .rs-hero figure { margin: 0; }
  .rs-hero svg { display: block; width: 100%; height: auto; background: var(--global-card-bg-color); border: 1px solid var(--global-divider-color); border-radius: 8px; }
  .rs-hero .lad-node { fill: var(--global-text-color); font-size: 11px; font-weight: 700; }
  .rs-hero .lad-sub { fill: var(--global-text-color-light); font-size: 8px; }
  .rs-hero .lad-ic { fill: none; stroke: var(--global-theme-color); stroke-width: 1.5; stroke-linejoin: round; stroke-linecap: round; }
  .rs-hero .lad-arr { stroke: var(--global-text-color-light); stroke-width: 1.2; fill: none; }
  .rs-hero .lad-q { fill: var(--global-theme-color); font-size: 8.5px; font-weight: 650; letter-spacing: 0.12em; }
  .rs-hero .lad-band { fill: color-mix(in srgb, var(--global-theme-color) 6%, transparent); }
  @media (max-width: 820px) { .rs-hero { grid-template-columns: 1fr; gap: 1.6rem; } }

  .rs-sec { padding: 3.4rem 0; border-top: 1px solid var(--global-divider-color); }
  .rs-core { display: grid; grid-template-columns: minmax(0, 0.95fr) minmax(280px, 0.8fr); gap: 3rem; align-items: start; }
  .rs-core h2 { font-size: clamp(1.6rem, 3.4vw, 2.3rem); font-weight: 650; line-height: 1.15; margin: 0; }
  .rs-core p { margin: 0 0 1rem; color: var(--global-text-color-light); line-height: 1.6; font-size: 0.97rem; }
  .method-line { display: grid; grid-template-columns: 1fr 1fr; border-top: 1px solid var(--global-divider-color); }
  .method-line span { padding: 0.7rem 0.6rem 0.7rem 0; border-bottom: 1px solid var(--global-divider-color); color: var(--global-theme-color); font-size: 0.86rem; font-weight: 700; }
  @media (max-width: 820px) { .rs-core { grid-template-columns: 1fr; gap: 1.4rem; } }

  .stories { padding-top: 0.5rem; }
  .story { display: grid; grid-template-columns: minmax(0, 1fr) minmax(280px, 0.85fr); gap: 2.8rem; align-items: center; padding: 3rem 0; border-top: 1px solid var(--global-divider-color); scroll-margin-top: 4.5rem; }
  .story:nth-child(even) .story-copy { order: 2; }
  .story:nth-child(even) .research-plate { order: 1; }
  .story h2 { font-size: clamp(1.45rem, 3vw, 2rem); font-weight: 650; line-height: 1.15; margin: 0 0 0.9rem; }
  .story p { color: var(--global-text-color-light); line-height: 1.6; font-size: 0.97rem; margin: 0 0 0.8rem; }
  .story .links { margin-top: 1rem; display: flex; flex-wrap: wrap; gap: 0.4rem 1.2rem; font-size: 0.88rem; font-weight: 700; }
  @media (max-width: 820px) { .story { grid-template-columns: 1fr; gap: 1.4rem; padding: 2.2rem 0; }
    .story:nth-child(even) .story-copy, .story:nth-child(even) .research-plate { order: initial; } }

  .tinted { position: relative; }
  .tinted::before { content: ""; position: absolute; inset: 0; left: 50%; transform: translateX(-50%); width: 100vw; background: color-mix(in srgb, var(--global-theme-color) 4%, var(--global-bg-color)); border-block: 1px solid var(--global-divider-color); z-index: -1; }
  .rs-sec h2.big { font-size: clamp(1.6rem, 3.4vw, 2.3rem); font-weight: 650; line-height: 1.15; margin: 0 0 1.6rem; max-width: 24ch; }
  .res-list article { display: grid; grid-template-columns: 8rem 11rem 1fr auto; gap: 1rem; align-items: baseline; padding: 0.85rem 0; border-top: 1px solid var(--global-divider-color); font-size: 0.92rem; }
  .res-list article:last-child { border-bottom: 1px solid var(--global-divider-color); }
  .res-list .role { color: var(--global-theme-color); font-size: 0.74rem; font-weight: 650; letter-spacing: 0.08em; text-transform: uppercase; }
  .res-list .name { font-weight: 700; }
  .res-list .desc { color: var(--global-text-color-light); }
  .res-list .act a { font-weight: 700; font-size: 0.86rem; margin-left: 0.8rem; }
  @media (max-width: 720px) { .res-list article { grid-template-columns: 1fr; gap: 0.2rem; } .res-list .act a { margin: 0 0.8rem 0 0; } }

  .outlook { display: grid; grid-template-columns: 1fr 1fr; gap: 2.4rem; }
  .outlook article { padding-top: 1rem; border-top: 3px solid var(--global-theme-color); }
  .outlook span { display: block; margin-bottom: 1rem; color: var(--global-text-color-light); font-size: 0.84rem; font-weight: 650; }
  .outlook h3 { font-size: 1.2rem; font-weight: 650; margin: 0 0 0.5rem; }
  .outlook p { color: var(--global-text-color-light); margin: 0; line-height: 1.6; font-size: 0.95rem; }
  @media (max-width: 640px) { .outlook { grid-template-columns: 1fr; } }
  .found { font-size: 0.92rem; color: var(--global-text-color-light); line-height: 1.6; max-width: 46rem; }
</style>

<section class="rs-hero">
  <div>
    <p class="kicker">Research</p>
    <h1>From molecular interventions to system-level responses.</h1>
    <p class="lead">I develop AI methods that learn how a molecular intervention&mdash;a small molecule binding a protein or RNA&mdash;reshapes interactions, networks, cellular states, and ultimately phenotype, and I hold every model to one standard: it has to be trustworthy.</p>
    <nav aria-label="Research topics">
      <ul class="research-index">
        <li><a href="#molecular-recognition">Molecular recognition</a></li>
        <li><a href="#rna-biology">RNA biology</a></li>
        <li><a href="#molecular-representation">Molecular representations</a></li>
        <li><a href="#structure-elucidation">Spectroscopy</a></li>
        <li><a href="#network-medicine">Network medicine</a></li>
        <li><a href="#trustworthy-methods">Trustworthy methods</a></li>
      </ul>
    </nav>
  </div>
  <figure>
    <svg viewBox="0 0 520 170" role="img" aria-label="Five biological scales, molecule to organism, under the three questions understand, predict, intervene">
      <rect class="lad-band" x="0" y="0" width="520" height="34"/>
      <text class="lad-q" x="90" y="21" text-anchor="middle">UNDERSTAND</text>
      <text class="lad-q" x="260" y="21" text-anchor="middle">PREDICT</text>
      <text class="lad-q" x="430" y="21" text-anchor="middle">INTERVENE</text>
      <g class="lad-ic">
        <polygon points="56,70 70,78 70,94 56,102 42,94 42,78"/><line x1="70" y1="78" x2="78" y2="74"/>
        <circle cx="148" cy="96" r="6"/><circle cx="172" cy="76" r="6"/><line x1="153" y1="92" x2="167" y2="80"/>
        <circle cx="260" cy="86" r="5"/><circle cx="244" cy="72" r="3.5"/><circle cx="276" cy="72" r="3.5"/><circle cx="244" cy="100" r="3.5"/><circle cx="276" cy="100" r="3.5"/>
        <line x1="260" y1="86" x2="244" y2="72"/><line x1="260" y1="86" x2="276" y2="72"/><line x1="260" y1="86" x2="244" y2="100"/><line x1="260" y1="86" x2="276" y2="100"/>
        <ellipse cx="362" cy="86" rx="19" ry="14"/><circle cx="358" cy="84" r="5"/>
        <circle cx="464" cy="72" r="7"/><path d="M450,104 C450,92 456,86 464,86 C472,86 478,92 478,104"/>
      </g>
      <g class="lad-arr"><path d="M96,86 h30 m-5,-4 l5,4 l-5,4"/><path d="M200,86 h26 m-5,-4 l5,4 l-5,4"/><path d="M300,86 h28 m-5,-4 l5,4 l-5,4"/><path d="M398,86 h30 m-5,-4 l5,4 l-5,4"/></g>
      <text class="lad-node" x="56" y="126" text-anchor="middle">Molecule</text>
      <text class="lad-node" x="160" y="126" text-anchor="middle">Interaction</text>
      <text class="lad-node" x="260" y="126" text-anchor="middle">Network</text>
      <text class="lad-node" x="362" y="126" text-anchor="middle">Cell</text>
      <text class="lad-node" x="464" y="126" text-anchor="middle">Organism</text>
      <text class="lad-sub" x="56" y="140" text-anchor="middle">structure, sequence</text>
      <text class="lad-sub" x="160" y="140" text-anchor="middle">binding, modification</text>
      <text class="lad-sub" x="260" y="140" text-anchor="middle">pathways, interactome</text>
      <text class="lad-sub" x="362" y="140" text-anchor="middle">cell state</text>
      <text class="lad-sub" x="464" y="140" text-anchor="middle">disease, outcome</text>
      <text class="lad-sub" x="260" y="160" text-anchor="middle">Interventions propagate upward; observations at higher scales constrain mechanisms below.</text>
    </svg>
    <figcaption class="fig-note">Five scales where biological states can be measured and modeled. Solid work sits at the first three; the last two are the next steps.</figcaption>
  </figure>
</section>

<section class="rs-sec">
  <div class="rs-core">
    <div>
      <p class="kicker">Core question</p>
      <h2>How does a molecular intervention propagate across biological scales?</h2>
    </div>
    <div>
      <p>Most biological AI models live within a single scale: a binding affinity, a modification site, a cell type. Living systems are coupled across scales, and the quantity that matters clinically is the response of the whole system. My work builds models at each scale that are explicit about mechanism, honest about uncertainty, and consistent with each other, so they can be composed into a world model of biological response.</p>
      <div class="method-line">
        <span>Mechanistic representation</span><span>Learning across molecular modalities</span>
        <span>Network propagation</span><span>Uncertainty and experimental validation</span>
      </div>
    </div>
  </div>
</section>

<details class="research-cycle rs-sec">
  <summary>World-model framework</summary>
  {% include research-cycle.liquid %}
</details>

<div class="stories">

<article class="story" id="molecular-recognition">
  <div class="story-copy">
    <p class="kicker">Interaction &middot; Understand</p>
    <h2>Explaining how molecules recognize proteins and RNA</h2>
    <p>ExplainBind predicts protein&ndash;ligand binding through explicit non-covalent interactions, so every prediction exposes its physicochemical determinants instead of a bare score. Ongoing work extends the same mechanistic framing to RNA&ndash;ligand recognition.</p>
    <div class="links"><a href="{{ '/publications/#xu2026explainbind' | relative_url }}">ExplainBind (bioRxiv 2026)</a><a href="{{ '/publications/#meng2026interactbind' | relative_url }}">InteractBind benchmark (arXiv 2026)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-binding.webp" caption="Illustration of a ligand in a protein binding pocket." %}
</article>

<article class="story" id="rna-biology">
  <div class="story-copy">
    <p class="kicker">Interaction &middot; Predict</p>
    <h2>Interpretable prediction of RNA modification in biological context</h2>
    <p>RNA modifications sit between sequence and function. EvoRMD integrates biological context with evolutionary RNA language models to predict modification sites interpretably, a step toward modeling how interventions on RNA propagate to cellular state.</p>
    <div class="links"><a href="{{ '/publications/#wang2026evormd' | relative_url }}">EvoRMD (Genome Biology 2026)</a><a href="{{ '/publications/#wang2026marri' | relative_url }}">MARRI (bioRxiv preprint)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-rna.webp" caption="Illustration of a folded RNA strand with a highlighted modification site." source="/assets/img/research/evormd-fig1.png" credit="Original Figure 1 · Wang et al., Genome Biology (CC BY-NC-ND)" %}
</article>

<article class="story" id="molecular-representation">
  <div class="story-copy">
    <p class="kicker">Molecule &middot; Understand / Predict</p>
    <h2>Learning molecular representations across complementary modalities</h2>
    <p>Chemical structure is observed through complementary views: graphs, spectra, text, and 3D geometry. Aligning them, asymmetrically and with relational learning, yields representations that transfer to property prediction and drug discovery while staying consistent with chemistry.</p>
    <div class="links"><a href="{{ '/publications/#wang2025advancing' | relative_url }}">Asymmetric contrastive learning (JCIM 2025)</a><a href="{{ '/publications/#zhou2025multimodal' | relative_url }}">Multimodal fusion (Commun. Chem. 2025)</a><a href="{{ '/publications/#liu2025matinstructions' | relative_url }}">Mat-Instructions (IJCAI 2025)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-fusion.webp" caption="Illustration of several complementary views of the same molecule." source="/assets/img/research/mmfusion-fig1.png" credit="Original Figure 1 · Zhou et al., Communications Chemistry (CC BY-NC-ND)" %}
</article>

<article class="story" id="structure-elucidation">
  <div class="story-copy">
    <p class="kicker">Molecule &middot; Understand</p>
    <h2>Self-verifying structure elucidation from spectra</h2>
    <p>Determining a molecule's structure from its spectra is a problem where a model must be able to check its own answer. This line builds solvent-aware 2D NMR prediction, an annotated experimental benchmark, and reasoning-based elucidation from mass spectra, toward NMRScape: self-verifying structure determination.</p>
    <div class="links"><a href="{{ '/publications/#li2025transpeaknet' | relative_url }}">TransPeakNet (Commun. Chem. 2025)</a><a href="{{ '/publications/#li2025dnmrgym' | relative_url }}">2DNMRGym (LoG 2025)</a><a href="{{ '/publications/#wang2026howwell' | relative_url }}">LLMs on mass spectra (J. Cheminform. 2026)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-spectra.webp" caption="Illustration of a candidate molecular structure alongside a schematic spectrum." source="/assets/img/research/transpeaknet-fig1.png" credit="Original Figure 1 · Li, Xu et al., Communications Chemistry (CC BY-NC-ND)" %}
</article>

<article class="story" id="network-medicine">
  <div class="story-copy">
    <p class="kicker">Network &middot; Understand / Intervene</p>
    <h2>From molecular interactions to disease networks and drug repurposing</h2>
    <p>Molecular interactions act through networks. Connecting binding and interactome structure to disease modules provides the route from a single intervention to a system-level response, and the basis for principled drug repurposing. Ongoing work builds affinity-weighted protein&ndash;protein interaction networks.</p>
    <div class="links"><a href="{{ '/publications/#wang2025systems' | relative_url }}">Systems chemical biology</a><a href="{{ '/publications/#xu2026drugrepurposing' | relative_url }}">Drug repurposing review (2026)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-network.webp" caption="Illustration of a disease module within a larger interaction network." %}
</article>

<article class="story" id="trustworthy-methods">
  <div class="story-copy">
    <p class="kicker">Methods &middot; Trustworthiness</p>
    <h2>Foundation-model methods that stay reliable on scientific data</h2>
    <p>Scientific data are scarce and shift between experiments, so the foundation models behind these systems must adapt cheaply and remain grounded. This work studies which parameter directions matter during adaptation and how to keep multimodal models faithful to their inputs.</p>
    <div class="links"><a href="{{ '/publications/#xiao2026notall' | relative_url }}">Not All Directions Matter (ACL 2026)</a><a href="{{ '/publications/#xiao2026vigilant' | relative_url }}">VIGIL (ECCV 2026)</a><a href="{{ '/publications/#zhang2026hyperadalora' | relative_url }}">HyperAdaLoRA (ACL Findings 2026)</a><a href="{{ '/publications/#zhang2025sensitivitylora' | relative_url }}">Sensitivity-LoRA (EMNLP Findings 2025)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-reliability.webp" caption="Illustration of comparing subtle changes in visual evidence." %}
</article>

</div>

<section class="rs-sec tinted" id="resources">
  <p class="kicker">Open resources</p>
  <h2 class="big">Benchmarks, datasets, and models built around these questions</h2>
  <div class="res-list">
    <article><span class="role">Benchmark</span><span class="name">InteractBind</span><span class="desc">Roughly 100k protein&ndash;ligand pairs with residue&ndash;atom interaction maps across six non-covalent interaction types, binding-site annotations, affinities, and similarity-controlled splits.</span><span class="act"><a href="https://arxiv.org/abs/2605.24045" target="_blank" rel="noopener">Paper</a><a href="https://huggingface.co/datasets/Zhaohan-Meng/InteractBind" target="_blank" rel="noopener">Dataset</a><a href="https://github.com/ZhaohanM/InteractBind" target="_blank" rel="noopener">Code</a></span></article>
    <article><span class="role">Benchmark</span><span class="name">2DNMRGym</span><span class="desc">Annotated experimental 2D NMR dataset for atom-level molecular representation learning.</span><span class="act"><a href="https://arxiv.org/abs/2505.18181" target="_blank" rel="noopener">Paper</a><a href="https://huggingface.co/papers/2505.18181" target="_blank" rel="noopener">Dataset</a><a href="https://github.com/siriusxiao62/2DNMRGym" target="_blank" rel="noopener">Code</a></span></article>
  </div>
</section>

<section class="rs-sec" id="toward-world-models">
  <p class="kicker">Outlook</p>
  <h2 class="big">Closing the loop from molecule to patient</h2>
  <div class="outlook">
    <article><span>01</span><h3>Cellular perturbation response</h3><p>Extend mechanistic, uncertainty-aware prediction to single-cell and Perturb-seq data, so that interventions learned at the molecular and network scales can be tested against measured cell states.</p></article>
    <article><span>02</span><h3>Precision intervention</h3><p>Invert the models: identify the molecular interventions that move a biological system toward a desired state, with explicit uncertainty and experimental validation in the loop. At the patient scale, phenotype is the readout: a first step is predicting <em>TP53</em> mutation status in hepatocellular carcinoma directly from MRI (<a href="{{ '/publications/#jia2025p53' | relative_url }}">BMC Med. Imaging 2025</a>).</p></article>
  </div>
</section>

<section class="rs-sec" id="foundations">
  <p class="kicker">Foundations</p>
  <p class="found">Earlier work in cobalt-catalyzed asymmetric radical reactions and total synthesis (<a href="{{ '/publications/#xu2024enantioselective' | relative_url }}">Chem 2024</a>, <a href="{{ '/publications/#riartferrer2021metalloradical' | relative_url }}">Chem 2021</a>) is the physical-organic foundation for building mechanism-aware models.</p>
</section>
