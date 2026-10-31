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
  .rs-hero h1 { font-size: clamp(2rem, 4.4vw, 2.8rem); font-weight: 800; line-height: 1.1; margin: 0 0 1rem; max-width: 18ch; }
  .rs-hero .lead { font-size: 1.05rem; line-height: 1.6; max-width: 34rem; margin: 0; }
  .rs-hero figure { margin: 0; }
  .rs-hero svg { display: block; width: 100%; height: auto; background: var(--global-card-bg-color); border: 1px solid var(--global-divider-color); border-radius: 8px; }
  .rs-hero .lad-node { fill: var(--global-text-color); font-size: 11px; font-weight: 700; }
  .rs-hero .lad-sub { fill: var(--global-text-color-light); font-size: 8px; }
  .rs-hero .lad-ic { fill: none; stroke: var(--global-theme-color); stroke-width: 1.5; stroke-linejoin: round; stroke-linecap: round; }
  .rs-hero .lad-arr { stroke: var(--global-text-color-light); stroke-width: 1.2; fill: none; }
  .rs-hero .lad-q { fill: var(--global-theme-color); font-size: 8.5px; font-weight: 800; letter-spacing: 0.12em; }
  .rs-hero .lad-band { fill: color-mix(in srgb, var(--global-theme-color) 6%, transparent); }
  @media (max-width: 820px) { .rs-hero { grid-template-columns: 1fr; gap: 1.6rem; } }

  .rs-sec { padding: 3.4rem 0; border-top: 1px solid var(--global-divider-color); }
  .rs-core { display: grid; grid-template-columns: minmax(0, 0.95fr) minmax(280px, 0.8fr); gap: 3rem; align-items: start; }
  .rs-core h2 { font-size: clamp(1.6rem, 3.4vw, 2.3rem); font-weight: 800; line-height: 1.15; margin: 0; }
  .rs-core p { margin: 0 0 1rem; color: var(--global-text-color-light); line-height: 1.6; font-size: 0.97rem; }
  .method-line { display: grid; grid-template-columns: 1fr 1fr; border-top: 1px solid var(--global-divider-color); }
  .method-line span { padding: 0.7rem 0.6rem 0.7rem 0; border-bottom: 1px solid var(--global-divider-color); color: var(--global-theme-color); font-size: 0.86rem; font-weight: 700; }
  @media (max-width: 820px) { .rs-core { grid-template-columns: 1fr; gap: 1.4rem; } }

  .stories { padding-top: 0.5rem; }
  .story { display: grid; grid-template-columns: minmax(0, 1fr) minmax(280px, 0.85fr); gap: 2.8rem; align-items: center; padding: 3rem 0; border-top: 1px solid var(--global-divider-color); scroll-margin-top: 4.5rem; }
  .story:nth-child(even) .story-copy { order: 2; }
  .story:nth-child(even) .story-visual { order: 1; }
  .story .index { margin: 0 0 0.9rem; color: var(--global-text-color-light); font-size: 0.86rem; font-weight: 800; letter-spacing: 0.06em; }
  .story h2 { font-size: clamp(1.45rem, 3vw, 2rem); font-weight: 800; line-height: 1.15; margin: 0 0 0.9rem; }
  .story p { color: var(--global-text-color-light); line-height: 1.6; font-size: 0.97rem; margin: 0 0 0.8rem; }
  .story .links { margin-top: 1rem; display: flex; flex-wrap: wrap; gap: 0.4rem 1.2rem; font-size: 0.88rem; font-weight: 700; }
  .story-visual { margin: 0; padding: 1rem; background: var(--global-card-bg-color); border: 1px solid var(--global-divider-color); border-radius: 8px; }
  .story-visual img { display: block; width: 100%; max-height: 380px; object-fit: contain; }
  .story-visual figcaption { margin-top: 0.6rem; color: var(--global-text-color-light); font-size: 0.78rem; line-height: 1.45; }
  .story-visual.panel dl { margin: 0; }
  .story-visual.panel dl > div { padding: 0.55rem 0; border-bottom: 1px solid var(--global-divider-color); }
  .story-visual.panel dl > div:last-child { border-bottom: 0; }
  .story-visual.panel dt { font-size: 0.68rem; font-weight: 800; letter-spacing: 0.12em; text-transform: uppercase; color: var(--global-theme-color); margin-bottom: 0.15rem; }
  .story-visual.panel dd { margin: 0; font-size: 0.88rem; line-height: 1.45; }
  @media (max-width: 820px) { .story { grid-template-columns: 1fr; gap: 1.4rem; padding: 2.2rem 0; }
    .story:nth-child(even) .story-copy, .story:nth-child(even) .story-visual { order: initial; } }

  .tinted { position: relative; }
  .tinted::before { content: ""; position: absolute; inset: 0; left: 50%; transform: translateX(-50%); width: 100vw; background: color-mix(in srgb, var(--global-theme-color) 4%, var(--global-bg-color)); border-block: 1px solid var(--global-divider-color); z-index: -1; }
  .rs-sec h2.big { font-size: clamp(1.6rem, 3.4vw, 2.3rem); font-weight: 800; line-height: 1.15; margin: 0 0 1.6rem; max-width: 24ch; }
  .res-list article { display: grid; grid-template-columns: 8rem 11rem 1fr auto; gap: 1rem; align-items: baseline; padding: 0.85rem 0; border-top: 1px solid var(--global-divider-color); font-size: 0.92rem; }
  .res-list article:last-child { border-bottom: 1px solid var(--global-divider-color); }
  .res-list .role { color: var(--global-theme-color); font-size: 0.74rem; font-weight: 800; letter-spacing: 0.08em; text-transform: uppercase; }
  .res-list .name { font-weight: 700; }
  .res-list .desc { color: var(--global-text-color-light); }
  .res-list .act a { font-weight: 700; font-size: 0.86rem; margin-left: 0.8rem; }
  @media (max-width: 720px) { .res-list article { grid-template-columns: 1fr; gap: 0.2rem; } .res-list .act a { margin: 0 0.8rem 0 0; } }

  .outlook { display: grid; grid-template-columns: 1fr 1fr; gap: 2.4rem; }
  .outlook article { padding-top: 1rem; border-top: 3px solid var(--global-theme-color); }
  .outlook span { display: block; margin-bottom: 1rem; color: var(--global-text-color-light); font-size: 0.84rem; font-weight: 800; }
  .outlook h3 { font-size: 1.2rem; font-weight: 800; margin: 0 0 0.5rem; }
  .outlook p { color: var(--global-text-color-light); margin: 0; line-height: 1.6; font-size: 0.95rem; }
  @media (max-width: 640px) { .outlook { grid-template-columns: 1fr; } }
  .fx { display: block; width: 100%; height: auto; }
  .fx .n { fill: var(--global-card-bg-color); stroke: var(--global-text-color-light); stroke-width: 1.3; }
  .fx .n.m { fill: color-mix(in srgb, var(--global-theme-color) 18%, var(--global-card-bg-color)); stroke: var(--global-theme-color); }
  .fx .n.t { fill: var(--global-theme-color); stroke: var(--global-theme-color); }
  .fx .e { stroke: var(--global-text-color-light); fill: none; opacity: 0.55; stroke-linecap: round; }
  .fx .e.a { stroke: var(--global-theme-color); opacity: 1; }
  .fx .mod { fill: color-mix(in srgb, var(--global-theme-color) 8%, transparent); stroke: var(--global-theme-color); stroke-dasharray: 4 3; stroke-width: 1; }
  .fx .ring { fill: none; stroke: var(--global-theme-color); stroke-width: 1; stroke-dasharray: 3 3; }
  .fx .drug { fill: var(--global-card-bg-color); stroke: var(--global-theme-color); stroke-width: 2; }
  .fx .lbl { fill: var(--global-text-color); font-size: 10px; font-weight: 700; }
  .fx .sub { fill: var(--global-text-color-light); font-size: 8.5px; }
  .fx .pn { fill: var(--global-theme-color); font-size: 10px; font-weight: 800; }
  .fx .box { fill: var(--global-card-bg-color); stroke: var(--global-text-color-light); stroke-width: 1.2; }
  .fx .box.frozen { fill: color-mix(in srgb, var(--global-text-color-light) 12%, var(--global-card-bg-color)); }
  .fx .box.acc { fill: color-mix(in srgb, var(--global-theme-color) 14%, var(--global-card-bg-color)); stroke: var(--global-theme-color); }
  .fx .dir { stroke: var(--global-text-color-light); stroke-width: 1; opacity: 0.5; }
  .fx .dir.a { stroke: var(--global-theme-color); stroke-width: 2.4; opacity: 1; }
  .fx .arr { stroke: var(--global-text-color-light); stroke-width: 1.2; fill: none; }
  .fx .ok { stroke: var(--global-theme-color); stroke-width: 2; fill: none; stroke-linecap: round; stroke-linejoin: round; }
  .fx .img { fill: none; stroke: var(--global-text-color); stroke-width: 1.2; }
  .fx .img.cf { stroke: var(--global-theme-color); }
  .found { font-size: 0.92rem; color: var(--global-text-color-light); line-height: 1.6; max-width: 46rem; }
</style>

<section class="rs-hero">
  <div>
    <p class="kicker">Research program &middot; Brigham and Women's Hospital &middot; Harvard Medical School</p>
    <h1>From molecular interventions to system-level responses.</h1>
    <p class="lead">I develop AI methods that learn how a molecular intervention&mdash;a small molecule binding a protein or RNA&mdash;reshapes interactions, networks, cellular states, and ultimately phenotype, and I hold every model to one standard: it has to be trustworthy.</p>
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

<div class="stories">

<article class="story" id="molecular-recognition">
  <div class="story-copy">
    <p class="index">01</p>
    <p class="kicker">Interaction &middot; Understand</p>
    <h2>Explaining how molecules recognize proteins and RNA</h2>
    <p>ExplainBind predicts protein&ndash;ligand binding through explicit non-covalent interactions, so every prediction exposes its physicochemical determinants instead of a bare score. Ongoing work extends the same mechanistic framing to RNA&ndash;ligand recognition.</p>
    <div class="links"><a href="{{ '/publications/#xu2026explainbind' | relative_url }}">ExplainBind (bioRxiv 2026)</a></div>
  </div>
  <div class="story-visual panel"><dl><div><dt>Scale</dt><dd>Biomolecular interaction</dd></div><div><dt>Question</dt><dd>Which non-covalent interactions determine binding, and why?</dd></div><div><dt>Trustworthiness</dt><dd>Interpretability, mechanistic consistency</dd></div><div><dt>Status</dt><dd>Preprint; RNA&ndash;ligand extension in progress</dd></div></dl></div>
</article>

<article class="story" id="rna-biology">
  <div class="story-copy">
    <p class="index">02</p>
    <p class="kicker">Interaction &middot; Predict</p>
    <h2>Interpretable prediction of RNA modification in biological context</h2>
    <p>RNA modifications sit between sequence and function. EvoRMD integrates biological context with evolutionary RNA language models to predict modification sites interpretably, a step toward modeling how interventions on RNA propagate to cellular state.</p>
    <div class="links"><a href="{{ '/publications/#wang2026evormd' | relative_url }}">EvoRMD (Genome Biology 2026)</a></div>
  </div>
  <figure class="story-visual">
    <img src="{{ '/assets/img/research/evormd-fig1.png' | relative_url }}" alt="Overview of EvoRMD. Figure 1 from Wang et al., Genome Biology 2026 (CC BY-NC-ND)." loading="lazy">
    <figcaption>Overview of EvoRMD. Figure 1 from Wang et al., Genome Biology 2026 (CC BY-NC-ND).</figcaption>
  </figure>
</article>

<article class="story" id="molecular-representation">
  <div class="story-copy">
    <p class="index">03</p>
    <p class="kicker">Molecule &middot; Understand / Predict</p>
    <h2>Learning molecular representations across complementary modalities</h2>
    <p>Chemical structure is observed through complementary views: graphs, spectra, text, and 3D geometry. Aligning them, asymmetrically and with relational learning, yields representations that transfer to property prediction and drug discovery while staying consistent with chemistry.</p>
    <div class="links"><a href="{{ '/publications/#wang2025advancing' | relative_url }}">Asymmetric contrastive learning (JCIM 2025)</a><a href="{{ '/publications/#zhou2025multimodal' | relative_url }}">Multimodal fusion (Commun. Chem. 2025)</a><a href="{{ '/publications/#liu2025matinstructions' | relative_url }}">Mat-Instructions (IJCAI 2025)</a></div>
  </div>
  <figure class="story-visual">
    <img src="{{ '/assets/img/research/mmfusion-fig1.png' | relative_url }}" alt="Multimodal fusion with relational learning. Figure 1 from Zhou et al., Communications Chemistry 2025 (CC BY-NC-ND)." loading="lazy">
    <figcaption>Multimodal fusion with relational learning. Figure 1 from Zhou et al., Communications Chemistry 2025 (CC BY-NC-ND).</figcaption>
  </figure>
</article>

<article class="story" id="structure-elucidation">
  <div class="story-copy">
    <p class="index">04</p>
    <p class="kicker">Molecule &middot; Understand</p>
    <h2>Self-verifying structure elucidation from spectra</h2>
    <p>Determining a molecule's structure from its spectra is a problem where a model must be able to check its own answer. This line builds solvent-aware 2D NMR prediction, an annotated experimental benchmark, and reasoning-based elucidation from mass spectra, toward NMRScape: self-verifying structure determination.</p>
    <div class="links"><a href="{{ '/publications/#li2025transpeaknet' | relative_url }}">TransPeakNet (Commun. Chem. 2025)</a><a href="{{ '/publications/#li2025dnmrgym' | relative_url }}">2DNMRGym (LoG 2025)</a><a href="{{ '/publications/#wang2026howwell' | relative_url }}">LLMs on mass spectra (J. Cheminform. 2026)</a></div>
  </div>
  <figure class="story-visual">
    <img src="{{ '/assets/img/research/transpeaknet-fig1.png' | relative_url }}" alt="Model design and training strategy of TransPeakNet. Figure 1 from Li, Xu et al., Communications Chemistry 2025 (CC BY-NC-ND)." loading="lazy">
    <figcaption>Model design and training strategy of TransPeakNet. Figure 1 from Li, Xu et al., Communications Chemistry 2025 (CC BY-NC-ND).</figcaption>
  </figure>
</article>

<article class="story" id="network-medicine">
  <div class="story-copy">
    <p class="index">05</p>
    <p class="kicker">Network &middot; Understand / Intervene</p>
    <h2>From molecular interactions to disease networks and drug repurposing</h2>
    <p>Molecular interactions act through networks. Connecting binding and interactome structure to disease modules provides the route from a single intervention to a system-level response, and the basis for principled drug repurposing. Ongoing work builds affinity-weighted protein&ndash;protein interaction networks.</p>
    <div class="links"><a href="{{ '/publications/#wang2025systems' | relative_url }}">Systems chemical biology (2025)</a><a href="{{ '/publications/#xu2026drugrepurposing' | relative_url }}">Drug repurposing review (2026)</a><a href="{{ '/publications/#jia2025p53' | relative_url }}">MRI prediction of P53-mutated HCC (2025)</a></div>
  </div>
  <figure class="story-visual">
    <svg class="fx" viewBox="0 0 420 300" role="img" aria-label="Schematic: a drug binds a target protein; the perturbation propagates through an affinity-weighted interaction network into a disease module">
      <ellipse class="mod" cx="262" cy="152" rx="66" ry="58"/>
      <text class="sub" x="262" y="84" text-anchor="middle">disease module</text>
      <g class="e">
        <line x1="80" y1="60" x2="130" y2="40" stroke-width="1"/><line x1="80" y1="60" x2="60" y2="150" stroke-width="0.8"/>
        <line x1="130" y1="40" x2="190" y2="70" stroke-width="1"/><line x1="190" y1="70" x2="150" y2="120" stroke-width="1"/>
        <line x1="130" y1="40" x2="150" y2="120" stroke-width="0.8"/><line x1="60" y1="150" x2="150" y2="120" stroke-width="1.2"/>
        <line x1="110" y1="230" x2="150" y2="120" stroke-width="0.8"/><line x1="110" y1="230" x2="170" y2="270" stroke-width="0.8"/>
        <line x1="170" y1="270" x2="300" y2="260" stroke-width="0.8"/><line x1="300" y1="260" x2="270" y2="190" stroke-width="1"/>
        <line x1="190" y1="70" x2="230" y2="120" stroke-width="1"/><line x1="360" y1="60" x2="275" y2="110" stroke-width="0.8"/>
        <line x1="360" y1="60" x2="390" y2="130" stroke-width="0.8"/><line x1="390" y1="130" x2="340" y2="190" stroke-width="1"/>
        <line x1="300" y1="150" x2="340" y2="190" stroke-width="1"/><line x1="340" y1="190" x2="370" y2="230" stroke-width="0.8"/>
        <line x1="230" y1="120" x2="275" y2="110" stroke-width="1.5"/><line x1="275" y1="110" x2="300" y2="150" stroke-width="1.5"/>
        <line x1="300" y1="150" x2="270" y2="190" stroke-width="1.5"/><line x1="270" y1="190" x2="225" y2="185" stroke-width="1.5"/>
        <line x1="225" y1="185" x2="230" y2="120" stroke-width="1"/>
        <line x1="255" y1="150" x2="230" y2="120" stroke-width="1.2"/><line x1="255" y1="150" x2="275" y2="110" stroke-width="1.2"/>
        <line x1="255" y1="150" x2="300" y2="150" stroke-width="1.2"/><line x1="255" y1="150" x2="270" y2="190" stroke-width="1.2"/>
        <line x1="255" y1="150" x2="225" y2="185" stroke-width="1.2"/>
      </g>
      <line class="e a" x1="150" y1="120" x2="230" y2="120" stroke-width="2.4"/>
      <line class="e a" x1="150" y1="120" x2="225" y2="185" stroke-width="1.8"/>
      <line class="e a" x1="48" y1="120" x2="150" y2="120" stroke-width="3.4"/>
      <circle class="ring" cx="150" cy="120" r="26"/><circle class="ring" cx="150" cy="120" r="44" opacity="0.5"/>
      <g>
        <circle class="n" cx="80" cy="60" r="5"/><circle class="n" cx="130" cy="40" r="5"/><circle class="n" cx="60" cy="150" r="5"/>
        <circle class="n" cx="110" cy="230" r="5"/><circle class="n" cx="170" cy="270" r="5"/><circle class="n" cx="300" cy="260" r="5"/>
        <circle class="n" cx="190" cy="70" r="5"/><circle class="n" cx="360" cy="60" r="5"/><circle class="n" cx="390" cy="130" r="5"/>
        <circle class="n" cx="340" cy="190" r="5"/><circle class="n" cx="370" cy="230" r="5"/>
        <circle class="n m" cx="230" cy="120" r="6"/><circle class="n m" cx="275" cy="110" r="6"/><circle class="n m" cx="300" cy="150" r="6"/>
        <circle class="n m" cx="270" cy="190" r="6"/><circle class="n m" cx="225" cy="185" r="6"/><circle class="n m" cx="255" cy="150" r="6"/>
        <circle class="n t" cx="150" cy="120" r="7"/>
        <polygon class="drug" points="48,106 60,113 60,127 48,134 36,127 36,113"/>
      </g>
      <text class="lbl" x="48" y="150" text-anchor="middle">drug</text>
      <text class="lbl" x="150" y="142" text-anchor="middle">target</text>
      <g class="sub">
        <line class="e a" x1="30" y1="282" x2="52" y2="282" stroke-width="3"/><text x="58" y="285">edge width = binding affinity</text>
        <circle class="n m" cx="196" cy="282" r="5"/><text x="206" y="285">disease-module protein</text>
        <circle class="ring" cx="330" cy="282" r="6"/><text x="341" y="285">perturbation spreads</text>
      </g>
    </svg>
    <figcaption>Affinity-weighted interaction networks. A drug binds its target; the perturbation propagates along weighted edges into a disease module. Schematic, work in progress.</figcaption>
  </figure>
</article>

<article class="story" id="trustworthy-methods">
  <div class="story-copy">
    <p class="index">06</p>
    <p class="kicker">Methods &middot; Trustworthiness</p>
    <h2>Foundation-model methods that stay reliable on scientific data</h2>
    <p>Scientific data are scarce and shift between experiments, so the foundation models behind these systems must adapt cheaply and remain grounded. This work studies which parameter directions matter during adaptation and how to keep multimodal models faithful to their inputs.</p>
    <div class="links"><a href="{{ '/publications/#xiao2026notall' | relative_url }}">Not All Directions Matter (ACL 2026)</a><a href="{{ '/publications/#xiao2026vigilant' | relative_url }}">VIGIL (ECCV 2026)</a><a href="{{ '/publications/#zhang2026hyperadalora' | relative_url }}">HyperAdaLoRA (ACL Findings 2026)</a><a href="{{ '/publications/#zhang2025sensitivitylora' | relative_url }}">Sensitivity-LoRA (EMNLP Findings 2025)</a></div>
  </div>
  <figure class="story-visual">
    <svg class="fx" viewBox="0 0 420 300" role="img" aria-label="Schematic: a, structured task-aware low-rank adaptation keeps few parameter directions; b, counterfactual visual alignment makes answers change when the image changes">
      <text class="pn" x="14" y="20">a</text><text class="lbl" x="28" y="20">Task-aware low-rank adaptation</text>
      <g>
        <rect class="box frozen" x="40" y="44" width="70" height="16" rx="3"/><rect class="box frozen" x="40" y="66" width="70" height="16" rx="3"/>
        <rect class="box frozen" x="40" y="88" width="70" height="16" rx="3"/><rect class="box frozen" x="40" y="110" width="70" height="16" rx="3"/>
        <text class="sub" x="75" y="142" text-anchor="middle">frozen foundation model</text>
        <rect class="box acc" x="122" y="66" width="22" height="16" rx="3"/><rect class="box acc" x="122" y="88" width="22" height="16" rx="3"/>
        <text class="sub" x="133" y="120" text-anchor="middle">adapters</text>
      </g>
      <g transform="translate(110,215)">
        <g class="dir">
          <line x1="0" y1="0" x2="0" y2="-44"/><line x1="0" y1="0" x2="22" y2="-38"/><line x1="0" y1="0" x2="38" y2="-22"/>
          <line x1="0" y1="0" x2="44" y2="0"/><line x1="0" y1="0" x2="38" y2="22"/><line x1="0" y1="0" x2="22" y2="38"/>
          <line x1="0" y1="0" x2="0" y2="44"/><line x1="0" y1="0" x2="-22" y2="38"/><line x1="0" y1="0" x2="-38" y2="22"/>
          <line x1="0" y1="0" x2="-44" y2="0"/><line x1="0" y1="0" x2="-38" y2="-22"/><line x1="0" y1="0" x2="-22" y2="-38"/>
        </g>
        <line class="dir a" x1="0" y1="0" x2="31" y2="-31"/><line class="dir a" x1="0" y1="0" x2="-44" y2="0"/><line class="dir a" x1="0" y1="0" x2="14" y2="42"/>
        <circle class="n t" cx="0" cy="0" r="3"/>
      </g>
      <text class="sub" x="110" y="276" text-anchor="middle">parameter directions: few matter for a task</text>

      <line class="e" x1="210" y1="14" x2="210" y2="286" stroke-width="1" stroke-dasharray="3 3"/>
      <text class="pn" x="224" y="20">b</text><text class="lbl" x="238" y="20">Counterfactual visual alignment</text>
      <g>
        <rect class="img" x="236" y="44" width="46" height="34" rx="3"/><path class="img" d="M240,74 l12,-14 l8,9 l7,-7 l11,12"/><circle class="img" cx="270" cy="52" r="3"/>
        <line class="e" x1="290" y1="52" x2="320" y2="52" stroke-width="1.5"/><line class="e" x1="290" y1="60" x2="314" y2="60" stroke-width="1.5"/><line class="e" x1="290" y1="68" x2="322" y2="68" stroke-width="1.5"/>
        <path class="arr" d="M330,61 h18 m-4,-4 l4,4 l-4,4"/>
        <rect class="box" x="352" y="46" width="34" height="30" rx="4"/><text class="sub" x="369" y="65" text-anchor="middle">MLLM</text>
        <path class="arr" d="M390,61 h10"/><text class="lbl" x="404" y="65">A</text>
      </g>
      <g>
        <rect class="img cf" x="236" y="120" width="46" height="34" rx="3"/><path class="img cf" d="M240,150 l9,-7 l9,7 l9,-16 l11,16"/><circle class="img cf" cx="248" cy="128" r="3"/>
        <line class="e" x1="290" y1="128" x2="320" y2="128" stroke-width="1.5"/><line class="e" x1="290" y1="136" x2="314" y2="136" stroke-width="1.5"/><line class="e" x1="290" y1="144" x2="322" y2="144" stroke-width="1.5"/>
        <path class="arr" d="M330,137 h18 m-4,-4 l4,4 l-4,4"/>
        <rect class="box" x="352" y="122" width="34" height="30" rx="4"/><text class="sub" x="369" y="141" text-anchor="middle">MLLM</text>
        <path class="arr" d="M390,137 h10"/><text class="lbl" x="404" y="141">B</text>
      </g>
      <text class="sub" x="259" y="172" text-anchor="middle">counterfactual image</text>
      <text class="sub" x="305" y="172" text-anchor="middle">&nbsp;</text>
      <text class="sub" x="308" y="100" text-anchor="middle">same question</text>
      <path class="ok" d="M236,214 l6,6 l12,-12"/><text class="sub" x="260" y="219">answer changes with the image: A &ne; B</text>
      <path class="ok" d="M236,240 l6,6 l12,-12" opacity="0.45"/><text class="sub" x="260" y="245">the image, not text priors, drives the answer</text>
    </svg>
    <figcaption><b>a</b>, Structured, task-aware low-rank adaptation keeps only the parameter directions that matter. <b>b</b>, Counterfactual visual alignment trains multimodal models whose answers must change when the image changes. Schematic.</figcaption>
  </figure>
</article>

</div>

<section class="rs-sec tinted" id="resources">
  <p class="kicker">Open resources</p>
  <h2 class="big">Benchmarks, datasets, and models built around these questions</h2>
  <div class="res-list">
    <article><span class="role">Benchmark</span><span class="name">2DNMRGym</span><span class="desc">Annotated experimental 2D NMR dataset for atom-level molecular representation learning.</span><span class="act"><a href="{{ '/publications/#li2025dnmrgym' | relative_url }}">Paper</a></span></article>
    <article><span class="role">Dataset</span><span class="name">Mat-Instructions</span><span class="desc">Large-scale inorganic materials instruction dataset for large language models.</span><span class="act"><a href="{{ '/publications/#liu2025matinstructions' | relative_url }}">Paper</a></span></article>
    <article><span class="role">Model</span><span class="name">TransPeakNet</span><span class="desc">Solvent-aware 2D NMR prediction; patent application filed with Brandeis University.</span><span class="act"><a href="{{ '/publications/#li2025transpeaknet' | relative_url }}">Paper</a><a href="{{ '/publications/#hong2024nmrpatent' | relative_url }}">Patent</a></span></article>
    <article><span class="role">Model</span><span class="name">ExplainBind</span><span class="desc">Explainable protein&ndash;ligand binding prediction via non-covalent interactions.</span><span class="act"><a href="{{ '/publications/#xu2026explainbind' | relative_url }}">Preprint</a></span></article>
  </div>
</section>

<section class="rs-sec" id="toward-world-models">
  <p class="kicker">Outlook</p>
  <h2 class="big">Closing the loop from molecule to patient</h2>
  <div class="outlook">
    <article><span>01</span><h3>Cellular perturbation response</h3><p>Extend mechanistic, uncertainty-aware prediction to single-cell and Perturb-seq data, so that interventions learned at the molecular and network scales can be tested against measured cell states.</p></article>
    <article><span>02</span><h3>Precision intervention</h3><p>Invert the models: identify the molecular interventions that move a biological system toward a desired state, with explicit uncertainty and experimental validation in the loop.</p></article>
  </div>
</section>

<section class="rs-sec" id="foundations">
  <p class="kicker">Foundations</p>
  <p class="found">Earlier work in cobalt-catalyzed asymmetric radical reactions and total synthesis (<a href="{{ '/publications/#xu2024enantioselective' | relative_url }}">Chem 2024</a>, <a href="{{ '/publications/#riartferrer2021metalloradical' | relative_url }}">Chem 2021</a>) is the physical-organic foundation for building mechanism-aware models.</p>
</section>
