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
  .story .clinical-imaging { margin-top: 1.25rem; }
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
        <li><a href="#clinical-ai">Clinical AI</a></li>
        <li><a href="#trustworthy-methods">Trustworthy methods</a></li>
      </ul>
    </nav>
  </div>
  <figure class="research-scale">
    <div class="research-scale-plate">
      <ul class="research-scale-actions" aria-label="Research goals">
        <li>Understand</li>
        <li>Predict</li>
        <li>Intervene</li>
      </ul>
      <img src="{{ '/assets/img/research/editorial-scales.webp' | relative_url }}" width="1440" height="480" alt="" decoding="async" fetchpriority="high">
      <ol class="research-scale-labels" aria-label="Biological scales">
        <li>Molecule</li>
        <li>Interaction</li>
        <li>Network</li>
        <li>Cell</li>
        <li>Organism</li>
      </ol>
    </div>
    <figcaption class="fig-note">Five scales where biological states can be measured and modeled, from molecular structure to patient outcomes.</figcaption>
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
  {% include research-plate.liquid image="/assets/img/research/editorial-rna-separated.webp" caption="Illustration of a folded RNA strand with a highlighted modification site." %}
</article>

<article class="story" id="molecular-representation">
  <div class="story-copy">
    <p class="kicker">Molecule &middot; Understand / Predict</p>
    <h2>Learning molecular representations across complementary modalities</h2>
    <p>Chemical structure is observed through complementary views: graphs, spectra, text, and 3D geometry. Aligning them, asymmetrically and with relational learning, yields representations that transfer to property prediction and drug discovery while staying consistent with chemistry.</p>
    <div class="links"><a href="{{ '/publications/#wang2025advancing' | relative_url }}">Asymmetric contrastive learning (JCIM 2025)</a><a href="{{ '/publications/#zhou2025multimodal' | relative_url }}">Multimodal fusion (Commun. Chem. 2025)</a><a href="{{ '/publications/#liu2025matinstructions' | relative_url }}">Mat-Instructions (IJCAI 2025)</a></div>
  </div>
  <figure class="research-plate">
    <div class="research-modalities">
      <img src="{{ '/assets/img/research/editorial-modalities-graph.webp' | relative_url }}" width="960" height="640" alt="" loading="lazy" decoding="async">
      <ul class="research-modality-labels" aria-label="Input modalities">
        <li>Molecular graph</li>
        <li>Spectrum</li>
        <li>Text</li>
        <li>3D geometry</li>
      </ul>
    </div>
    <figcaption class="fig-note">Four kinds of input contribute to a shared molecular representation.</figcaption>
  </figure>
</article>

<article class="story" id="structure-elucidation">
  <div class="story-copy">
    <p class="kicker">Molecule &middot; Understand</p>
    <h2>Self-verifying structure elucidation from spectra</h2>
    <p>Determining a molecule's structure from its spectra is a problem where a model must be able to check its own answer. This line builds solvent-aware 2D NMR prediction, an annotated experimental benchmark, and reasoning-based elucidation from mass spectra, toward NMRScape: self-verifying structure determination.</p>
    <div class="links"><a href="{{ '/publications/#li2025transpeaknet' | relative_url }}">TransPeakNet (Commun. Chem. 2025)</a><a href="{{ '/publications/#li2025dnmrgym' | relative_url }}">2DNMRGym (LoG 2025)</a><a href="{{ '/publications/#wang2026howwell' | relative_url }}">LLMs on mass spectra (J. Cheminform. 2026)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-spectra.webp" caption="Illustration of a candidate molecular structure alongside a schematic spectrum." %}
</article>

<article class="story" id="network-medicine">
  <div class="story-copy">
    <p class="kicker">Network &middot; Understand / Intervene</p>
    <h2>From molecular interactions to disease networks and drug repurposing</h2>
    <p>Molecular interactions act through networks. Connecting binding and interactome structure to disease modules provides the route from a single intervention to a system-level response, and the basis for principled drug repurposing. Ongoing work builds affinity-weighted protein&ndash;protein interaction networks.</p>
    <div class="links"><a href="{{ '/publications/#wang2025systems' | relative_url }}">Systems chemical biology (Book Chapter)</a><a href="{{ '/publications/#xu2026drugrepurposing' | relative_url }}">Drug repurposing review (2026)</a></div>
  </div>
  {% include research-plate.liquid image="/assets/img/research/editorial-network-stars.webp" caption="A constellation represents a disease module within a larger interaction network." %}
</article>

<article class="story" id="clinical-ai">
  <div class="story-copy">
    <p class="kicker">Patient outcomes &middot; Clinical AI</p>
    <h2>Heart failure outcomes and cancer imaging</h2>
    <p><strong>Cardiovascular outcomes.</strong> We used network analysis and machine learning to study clinical factors associated with in-hospital mortality and survival in heart failure. The work appeared in <em>Circulation</em> as an American Heart Association Scientific Sessions abstract.</p>
    <div class="links">
      <a href="{{ '/publications/#xu2026heartfailure' | relative_url }}">Heart failure outcomes (Circulation, AHA abstract 2026)</a>
    </div>
    <p class="clinical-imaging"><strong>Radiology.</strong> We studied how MRI can predict <em>TP53</em> mutation status and how contrast-enhanced CT can identify the macrotrabecular-massive subtype of hepatocellular carcinoma.</p>
    <div class="links">
      <a href="{{ '/publications/#jia2025p53' | relative_url }}">MRI and <em>TP53</em> status (BMC Medical Imaging 2025)</a>
      <a href="{{ '/publications/#jia2025macrotrabecular' | relative_url }}">CT and tumor subtype (Insights into Imaging 2025)</a>
    </div>
  </div>
  <figure class="research-plate">
    <img src="{{ '/assets/img/research/editorial-heart-liver.webp' | relative_url }}" width="960" height="640" alt="" loading="lazy" decoding="async">
    <figcaption class="research-paired-labels">
      <strong>Heart</strong>
      <strong>Liver</strong>
    </figcaption>
  </figure>
</article>

<article class="story" id="trustworthy-methods">
  <div class="story-copy">
    <p class="kicker">Methods &middot; Trustworthiness</p>
    <h2>Language and vision&ndash;language reasoning</h2>
    <p><strong>LLM reasoning.</strong> We study how language models retrieve and connect evidence across multiple reasoning steps.</p>
    <p><strong>VLM reasoning.</strong> We study whether a model’s answer follows the visual evidence when the image changes.</p>
    <p>We also develop parameter-efficient methods for adapting foundation models to new tasks.</p>
    <div class="links">
      <a href="{{ '/publications/#meng2026ssebio' | relative_url }}">SSE-Bio (EMNLP Findings 2026)</a>
      <a href="{{ '/publications/#xiao2026vigilant' | relative_url }}">VIGIL (ECCV 2026)</a>
      <a href="{{ '/publications/#xiao2026notall' | relative_url }}">Not All Directions Matter (ACL 2026)</a>
      <a href="{{ '/publications/#zhang2026hyperadalora' | relative_url }}">HyperAdaLoRA (ACL Findings 2026)</a>
      <a href="{{ '/publications/#zhang2025sensitivitylora' | relative_url }}">Sensitivity-LoRA (EMNLP Findings 2025)</a>
    </div>
  </div>
  <figure class="research-plate">
    <img src="{{ '/assets/img/research/editorial-reasoning.webp' | relative_url }}" width="960" height="640" alt="" loading="lazy" decoding="async">
    <dl class="research-paired-labels">
      <div><dt>LLM reasoning</dt><dd>Link evidence across passages</dd></div>
      <div><dt>VLM reasoning</dt><dd>Ground a response in the image</dd></div>
    </dl>
  </figure>
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
    <article><span>02</span><h3>Precision intervention</h3><p>Invert the models: identify the molecular interventions that move a biological system toward a desired state, with explicit uncertainty and experimental validation in the loop. At the patient scale, this builds on our <a href="#clinical-ai">work with clinical outcomes and imaging</a>.</p></article>
  </div>
</section>

<section class="rs-sec" id="foundations">
  <p class="kicker">Foundations</p>
  <p class="found">Earlier work in cobalt-catalyzed asymmetric radical reactions and total synthesis (<a href="{{ '/publications/#xu2024enantioselective' | relative_url }}">Chem 2024</a>, <a href="{{ '/publications/#riartferrer2021metalloradical' | relative_url }}">Chem 2021</a>) is the physical-organic foundation for building mechanism-aware models.</p>
</section>
