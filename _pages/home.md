---
layout: home
permalink: /
title: Home
description: Hao Xu builds trustworthy AI systems that learn how molecular interventions propagate across biological scales, from molecular recognition to system-level biological responses.
---

<style>
  /* ---------- shared ---------- */
  .home h1, .home h2, .home h3 { letter-spacing: -0.01em; }
  .home .sec { margin-top: 3.6rem; }
  .home .sec-head {
    display: flex; align-items: baseline; justify-content: space-between; gap: 1rem;
    margin-bottom: 1rem; padding-bottom: 0.4rem;
    border-bottom: 1px solid var(--global-divider-color);
  }
  .home .sec-head h2 { margin: 0; font-size: 1.45rem; font-weight: 700; }
  .home .sec-head a { font-size: 0.88rem; font-weight: 600; white-space: nowrap; }
  .home .muted { color: var(--global-text-color-light); }
  .home .lede { max-width: 46rem; font-size: 1.05rem; line-height: 1.65; }

  /* ---------- hero ---------- */
  .hero { padding: 2.6rem 0 1.2rem; }
  .hero-kicker {
    font-size: 0.78rem; font-weight: 600; letter-spacing: 0.1em; text-transform: uppercase;
    color: var(--global-text-color-light); margin-bottom: 0.9rem;
  }
  .hero-title {
    font-size: clamp(2rem, 5.6vw, 3.1rem); font-weight: 800; line-height: 1.08;
    margin: 0 0 0.6rem; max-width: 18ch;
  }
  .hero-upi {
    font-size: clamp(1.15rem, 2.8vw, 1.45rem); font-weight: 600; margin: 0 0 0.9rem;
    color: var(--global-theme-color); letter-spacing: 0.01em;
  }
  .hero-upi span + span::before { content: "\00a0\00a0"; }
  .hero-lede { max-width: 44rem; font-size: 1.1rem; line-height: 1.6; margin: 0 0 1.3rem; }
  .hero-actions { display: flex; flex-wrap: wrap; gap: 0.55rem; margin: 0 0 2.2rem; }
  .hero-actions a {
    padding: 0.42rem 1rem; border-radius: 6px; border: 1.5px solid var(--global-theme-color);
    font-weight: 600; font-size: 0.9rem; text-decoration: none !important; color: var(--global-theme-color);
  }
  .hero-actions a.primary { background: var(--global-theme-color); color: var(--global-bg-color) !important; }

  /* ---------- schematic: molecule -> phenotype ---------- */
  .scales { margin: 0; padding: 1.4rem 1.2rem 1rem; border: 1px solid var(--global-divider-color); border-radius: 10px; }
  .scales-row { display: flex; align-items: center; justify-content: center; gap: 0.5rem; flex-wrap: nowrap; }
  .scales-top { margin-bottom: 1.1rem; }
  .scales-top .step {
    font-size: 0.8rem; font-weight: 700; letter-spacing: 0.08em; text-transform: uppercase;
    color: var(--global-theme-color); padding: 0.2rem 0.75rem; border-radius: 999px;
    border: 1px solid color-mix(in srgb, var(--global-theme-color) 45%, transparent);
  }
  .scales-top .arr { color: var(--global-theme-color); font-weight: 700; }
  .scales-chain { gap: 0; }
  .scales-chain .node {
    display: flex; flex-direction: column; align-items: center; gap: 0.45rem;
    min-width: 6.2rem; text-align: center;
  }
  .scales-chain .node i {
    display: block; border-radius: 50%; border: 2px solid var(--global-text-color);
    background: var(--global-bg-color); width: var(--d); height: var(--d);
  }
  .scales-chain .node b { font-size: 0.92rem; font-weight: 700; line-height: 1.2; }
  .scales-chain .node small { font-size: 0.74rem; color: var(--global-text-color-light); line-height: 1.25; max-width: 8.5rem; }
  .scales-chain .link {
    flex: 1 1 2.2rem; height: 2px; min-width: 1.4rem; margin-top: -2.6rem; position: relative;
    background: linear-gradient(90deg, var(--global-text-color-light) 0 50%, transparent 50% 100%);
    background-size: 8px 2px; opacity: 0.8;
  }
  .scales-chain .link::after {
    content: ""; position: absolute; right: -1px; top: 50%; transform: translateY(-50%);
    border: 4px solid transparent; border-left: 6px solid var(--global-text-color-light); border-right: 0;
  }
  @media (prefers-reduced-motion: no-preference) {
    .scales-chain .link { animation: flow 1.2s linear infinite; }
    @keyframes flow { from { background-position: 0 0; } to { background-position: 8px 0; } }
  }
  .scales-base {
    margin-top: 1.3rem; padding-top: 0.75rem; border-top: 2px solid var(--global-theme-color);
    display: flex; flex-wrap: wrap; justify-content: center; align-items: baseline; gap: 0.3rem 0.9rem;
    font-size: 0.8rem; color: var(--global-text-color-light);
  }
  .scales-base b { color: var(--global-text-color); font-weight: 700; letter-spacing: 0.08em; text-transform: uppercase; font-size: 0.76rem; }
  .scales-base span::before { content: "\00b7"; margin-right: 0.9rem; opacity: 0.6; }
  .scales-base span:first-of-type::before { content: ""; margin: 0; }
  @media (max-width: 640px) {
    .scales { padding: 1rem 0.8rem; }
    .scales-chain { flex-direction: column; gap: 0.5rem; }
    .scales-chain .node { flex-direction: row; min-width: 0; text-align: left; gap: 0.7rem; width: 100%; max-width: 20rem; }
    .scales-chain .node i { flex: none; }
    .scales-chain .node small { max-width: none; }
    .scales-chain .node b { min-width: 5.6rem; }
    .scales-chain .link { width: 2px; height: 1.1rem; flex: none; margin: 0; min-width: 0;
      background: linear-gradient(180deg, var(--global-text-color-light) 0 50%, transparent 50% 100%); background-size: 2px 8px; }
    .scales-chain .link::after { right: auto; left: 50%; top: auto; bottom: -1px; transform: translateX(-50%);
      border: 4px solid transparent; border-top: 6px solid var(--global-text-color-light); border-bottom: 0; }
    .scales-top .step { font-size: 0.7rem; padding: 0.15rem 0.5rem; }
  }

  /* ---------- research vision ---------- */
  .vision-q { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem; margin-top: 1.2rem; }
  .vision-q div { padding: 0.2rem 0 0 0.9rem; border-left: 3px solid var(--global-theme-color); }
  .vision-q h3 { margin: 0 0 0.3rem; font-size: 1.05rem; font-weight: 700; }
  .vision-q p { margin: 0; font-size: 0.95rem; line-height: 1.5; }
  .vision-trust { margin: 1.3rem 0 0; font-size: 0.95rem; }
  @media (max-width: 640px) { .vision-q { grid-template-columns: 1fr; } }

  /* ---------- research map ---------- */
  .rmap { width: 100%; border-collapse: separate; border-spacing: 0; table-layout: fixed; margin: 0; font-size: 0.84rem; }
  .rmap th, .rmap td { padding: 0.55rem 0.5rem; vertical-align: top; border-bottom: 1px solid var(--global-divider-color); }
  .rmap thead th { font-size: 0.76rem; font-weight: 700; letter-spacing: 0.08em; text-transform: uppercase;
    color: var(--global-theme-color); border-bottom: 2px solid var(--global-theme-color); text-align: left; }
  .rmap thead th:first-child { color: var(--global-text-color-light); }
  .rmap tbody th { font-weight: 700; text-align: left; white-space: nowrap; width: 7.2rem; font-size: 0.86rem; }
  .rmap tbody th small { display: block; font-weight: 400; color: var(--global-text-color-light); font-size: 0.72rem; white-space: normal; }
  .rmap tbody tr:last-child th, .rmap tbody tr:last-child td { border-bottom: 0; }
  .rmap .chip {
    display: inline-block; margin: 0 0.25rem 0.3rem 0; padding: 0.12rem 0.55rem; border-radius: 5px;
    border: 1px solid var(--global-divider-color); background: var(--global-card-bg-color);
    color: var(--global-text-color); text-decoration: none !important; line-height: 1.4;
  }
  .rmap a.chip { border-color: color-mix(in srgb, var(--global-theme-color) 50%, transparent); }
  .rmap a.chip:hover { background: color-mix(in srgb, var(--global-theme-color) 10%, transparent); }
  .rmap .chip.future { border-style: dashed; color: var(--global-text-color-light); background: transparent; }
  .rmap-legend { margin: 0.6rem 0 0; font-size: 0.78rem; color: var(--global-text-color-light); }
  .rmap-legend .chip { display: inline-block; padding: 0 0.45rem; border-radius: 5px; border: 1px solid var(--global-divider-color); margin-right: 0.3rem; }
  .rmap-legend .chip.future { border-style: dashed; }
  .rmap-wrap { overflow-x: auto; }
  @media (max-width: 640px) {
    .rmap { min-width: 34rem; }
  }

  /* ---------- trustworthy AI ---------- */
  .trust { display: grid; grid-template-columns: repeat(5, 1fr); gap: 0.8rem; margin-top: 1.2rem; }
  .trust div { padding: 0.9rem 0.9rem 0.8rem; border: 1px solid var(--global-divider-color); border-top: 3px solid var(--global-theme-color); border-radius: 8px; }
  .trust h3 { margin: 0 0 0.35rem; font-size: 0.98rem; font-weight: 700; }
  .trust p { margin: 0; font-size: 0.86rem; line-height: 1.45; color: var(--global-text-color-light); }
  .trust-note { margin: 1rem 0 0; font-size: 0.92rem; }
  @media (max-width: 900px) { .trust { grid-template-columns: repeat(3, 1fr); } }
  @media (max-width: 560px) { .trust { grid-template-columns: 1fr 1fr; } }

  /* ---------- selected research ---------- */
  .sel { list-style: none; margin: 0; padding: 0; }
  .sel li { display: grid; grid-template-columns: 13rem 1fr; gap: 0.4rem 1.4rem; padding: 0.95rem 0; border-bottom: 1px solid var(--global-divider-color); }
  .sel li:last-child { border-bottom: 0; }
  .sel .name { font-weight: 700; font-size: 1.02rem; line-height: 1.3; }
  .sel .name small { display: block; font-weight: 400; font-size: 0.76rem; color: var(--global-text-color-light); margin-top: 0.15rem; }
  .sel .what { margin: 0; font-size: 0.95rem; line-height: 1.5; }
  .sel .refs { margin: 0.3rem 0 0; font-size: 0.82rem; color: var(--global-text-color-light); }
  .sel .refs a { margin-right: 0.7rem; }
  @media (max-width: 640px) { .sel li { grid-template-columns: 1fr; gap: 0.2rem; } }

  /* ---------- news + contact ---------- */
  .home .news table { margin-bottom: 0; font-size: 0.92rem; }
  .home .news th { font-weight: 600; color: var(--global-text-color-light); white-space: nowrap; }
  .contact { margin: 3rem 0 1rem; padding-top: 1rem; border-top: 1px solid var(--global-divider-color); font-size: 0.92rem; color: var(--global-text-color-light); }
  .contact p { margin: 0 0 0.3rem; }
</style>

<section class="hero">
  <p class="hero-kicker">Hao Xu &middot; Brigham and Women's Hospital &middot; Harvard Medical School</p>
  <h1 class="hero-title">Trustworthy World Models for Life Science</h1>
  <p class="hero-upi"><span>Understand.</span><span>Predict.</span><span>Intervene.</span></p>
  <p class="hero-lede">Building AI systems that learn how molecular interventions propagate across biological scales&mdash;from molecular recognition to system-level biological responses.</p>
  <div class="hero-actions">
    <a class="primary" href="#vision">Research vision</a>
    <a href="#selected">Selected research</a>
    <a href="{{ '/about/' | relative_url }}">About Hao Xu</a>
  </div>

  <figure class="scales" aria-label="Schematic: understand, predict, and intervene across biological scales, from molecule to interaction, network, cell, and phenotype, grounded in trustworthiness">
    <div class="scales-row scales-top" aria-hidden="true">
      <span class="step">Understand</span><span class="arr">&rarr;</span>
      <span class="step">Predict</span><span class="arr">&rarr;</span>
      <span class="step">Intervene</span>
    </div>
    <div class="scales-row scales-chain">
      <div class="node" style="--d: 0.7rem;"><i></i><b>Molecule</b><small>small molecules, proteins, RNA</small></div>
      <div class="link" aria-hidden="true"></div>
      <div class="node" style="--d: 0.95rem;"><i></i><b>Interaction</b><small>binding, recognition, modification</small></div>
      <div class="link" aria-hidden="true"></div>
      <div class="node" style="--d: 1.2rem;"><i></i><b>Network</b><small>pathways, PPI, regulation</small></div>
      <div class="link" aria-hidden="true"></div>
      <div class="node" style="--d: 1.45rem;"><i></i><b>Cell</b><small>cellular states and responses</small></div>
      <div class="link" aria-hidden="true"></div>
      <div class="node" style="--d: 1.7rem;"><i></i><b>Phenotype</b><small>disease and treatment outcomes</small></div>
    </div>
    <div class="scales-base">
      <b>Trustworthiness</b>
      <span>Interpretability</span><span>Uncertainty</span><span>Robustness</span><span>Generalization</span><span>Mechanistic consistency</span>
    </div>
  </figure>
</section>

<section class="sec" id="vision">
  <div class="sec-head"><h2>Research Vision</h2></div>
  <p class="lede">Biology is a world of interventions. A small molecule binds a protein or RNA, reshapes molecular interactions, perturbs biological networks, alters cellular states, and ultimately changes phenotype. My research asks three fundamental questions:</p>
  <div class="vision-q">
    <div>
      <h3>Understand</h3>
      <p>What mechanisms and representations govern biological responses to intervention?</p>
    </div>
    <div>
      <h3>Predict</h3>
      <p>Can AI predict how unseen interventions reshape biological states, while knowing when its predictions are uncertain?</p>
    </div>
    <div>
      <h3>Intervene</h3>
      <p>Can we invert these models to identify interventions that drive biological systems toward desired states?</p>
    </div>
  </div>
  <p class="vision-trust">Across all three questions, I focus on <strong>trustworthiness</strong>: interpretability, uncertainty, robustness, generalization, and mechanistic consistency. The long-term goal is a trustworthy world model of life&mdash;one that connects molecular interventions to system-level biological responses and is consistent with biological mechanisms.</p>
</section>

<section class="sec" id="map">
  <div class="sec-head"><h2>Research Map</h2><a href="{{ '/research/' | relative_url }}">Research directions &rarr;</a></div>
  <p class="muted" style="margin-bottom: 0.9rem;">Where current and planned work sits: scales of biology (rows) against the three questions (columns).</p>
  <div class="rmap-wrap">
  <table class="rmap">
    <thead>
      <tr><th>Scale</th><th>Understand</th><th>Predict</th><th>Intervene</th></tr>
    </thead>
    <tbody>
      <tr>
        <th>Molecule<small>chemical structure and representation</small></th>
        <td><a class="chip" href="{{ '/publications/#wang2025advancing' | relative_url }}">Multimodal molecular learning</a><a class="chip" href="{{ '/publications/#li2025transpeaknet' | relative_url }}">NMR structure elucidation</a></td>
        <td><a class="chip" href="{{ '/publications/#zhou2025multimodal' | relative_url }}">Molecular property prediction</a><a class="chip" href="{{ '/publications/#wang2026howwell' | relative_url }}">Structure from mass spectra</a></td>
        <td></td>
      </tr>
      <tr>
        <th>Interaction<small>recognition and modification</small></th>
        <td><a class="chip" href="{{ '/publications/#xu2026explainbind' | relative_url }}">ExplainBind</a></td>
        <td><a class="chip" href="{{ '/publications/#wang2026evormd' | relative_url }}">EvoRMD</a><span class="chip">RNA&ndash;ligand recognition</span></td>
        <td></td>
      </tr>
      <tr>
        <th>Network<small>pathways and interactomes</small></th>
        <td><a class="chip" href="{{ '/publications/#wang2025systems' | relative_url }}">Network medicine</a></td>
        <td><span class="chip">Affinity-weighted PPI</span><span class="chip">Systems pharmacology</span></td>
        <td><a class="chip" href="{{ '/publications/#xu2026drugrepurposing' | relative_url }}">Drug repurposing</a></td>
      </tr>
      <tr>
        <th>Cell<small>cellular states</small></th>
        <td><span class="chip future">Perturbation biology</span></td>
        <td><span class="chip future">Single-cell response</span></td>
        <td></td>
      </tr>
      <tr>
        <th>Phenotype<small>organism and disease</small></th>
        <td><span class="chip future">Cross-scale state transition</span></td>
        <td></td>
        <td><span class="chip future">Precision intervention</span></td>
      </tr>
    </tbody>
  </table>
  </div>
  <p class="rmap-legend"><span class="chip">solid</span> current work &nbsp; <span class="chip future">dashed</span> planned directions</p>
</section>

<section class="sec" id="trust">
  <div class="sec-head"><h2>Trustworthy AI</h2></div>
  <p class="lede">A prediction is only useful if we know why it was made, when it may be wrong, and whether it respects the biology.</p>
  <div class="trust">
    <div><h3>Interpretability</h3><p>Why does the model make this prediction?</p></div>
    <div><h3>Uncertainty</h3><p>When does the model know that it may be wrong?</p></div>
    <div><h3>Robustness</h3><p>Does the prediction survive perturbations and measurement noise?</p></div>
    <div><h3>Generalization</h3><p>Does the learned principle transfer beyond the training distribution?</p></div>
    <div><h3>Mechanistic Consistency</h3><p>Does the prediction respect physical, chemical, and biological mechanisms?</p></div>
  </div>
  <p class="trust-note muted">Methodological foundations include parameter-efficient adaptation and multimodal alignment of foundation models (<a href="{{ '/publications/#xiao2026notall' | relative_url }}">ACL 2026</a>, <a href="{{ '/publications/#xiao2026vigilant' | relative_url }}">ECCV 2026</a>), which make large models reliable and cheap to adapt to scientific data.</p>
</section>

<section class="sec" id="selected">
  <div class="sec-head"><h2>Selected Research</h2><a href="{{ '/publications/' | relative_url }}">All publications &rarr;</a></div>
  <ul class="sel">
    <li>
      <div class="name">ExplainBind<small>Interaction &middot; Understand</small></div>
      <div>
        <p class="what">Mechanistically interpretable AI for protein&ndash;ligand recognition: predicting binding through explicit non-covalent interactions, so every prediction comes with its physicochemical determinants.</p>
        <p class="refs"><a href="{{ '/publications/#xu2026explainbind' | relative_url }}">bioRxiv 2026</a></p>
      </div>
    </li>
    <li>
      <div class="name">EvoRMD<small>Interaction &middot; Predict</small></div>
      <div>
        <p class="what">Context-aware and interpretable modeling of RNA modification, integrating biological context with evolutionary RNA language models.</p>
        <p class="refs"><a href="{{ '/publications/#wang2026evormd' | relative_url }}">Genome Biology 2026</a></p>
      </div>
    </li>
    <li>
      <div class="name">Multimodal Molecular Learning<small>Molecule &middot; Understand / Predict</small></div>
      <div>
        <p class="what">Learning chemical representations across complementary molecular modalities&mdash;graphs, spectra, text, and 3D structure&mdash;for property prediction and drug discovery.</p>
        <p class="refs"><a href="{{ '/publications/#wang2025advancing' | relative_url }}">JCIM 2025</a><a href="{{ '/publications/#zhou2025multimodal' | relative_url }}">Commun. Chem. 2025</a></p>
      </div>
    </li>
    <li>
      <div class="name">NMRScape<small>Molecule &middot; Understand</small></div>
      <div>
        <p class="what">Self-verifying AI for molecular structure elucidation from NMR and mass spectra, built on solvent-aware 2D NMR prediction and an annotated experimental benchmark.</p>
        <p class="refs"><a href="{{ '/publications/#li2025transpeaknet' | relative_url }}">Commun. Chem. 2025</a><a href="{{ '/publications/#li2025dnmrgym' | relative_url }}">LoG 2025</a><a href="{{ '/publications/#wang2026howwell' | relative_url }}">J. Cheminform. 2026</a></p>
      </div>
    </li>
    <li>
      <div class="name">Network Medicine &amp; Systems Pharmacology<small>Network &middot; Understand / Intervene</small></div>
      <div>
        <p class="what">Connecting molecular interactions to system-level disease mechanisms, and using those connections to reason about drug repurposing and intervention.</p>
        <p class="refs"><a href="{{ '/publications/#wang2025systems' | relative_url }}">Comprehensive Medicinal Chemistry 2025</a><a href="{{ '/publications/#xu2026drugrepurposing' | relative_url }}">Drug Repurposing 2026</a></p>
      </div>
    </li>
  </ul>
</section>

<section class="sec" id="news">
  <div class="sec-head"><h2>News</h2></div>
  {% include news.liquid limit=true %}
</section>

<section class="contact">
  <p>Hao Xu &middot; Department of Medicine, Brigham and Women's Hospital &middot; Harvard Medical School &middot; Boston, MA</p>
  <p><a href="mailto:haoxu0303@gmail.com">haoxu0303@gmail.com</a> &middot; Inquiries from prospective students and collaborators are welcome.</p>
</section>
