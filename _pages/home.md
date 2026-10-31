---
layout: home
permalink: /
title: Home
description: Hao Xu builds trustworthy AI systems that learn how biological interventions propagate across scales, from molecular recognition to system-level biological responses.
---

<style>
  /* ---------- shared ---------- */
  .home h1, .home h2, .home h3 { letter-spacing: -0.01em; }
  .home .sec { margin-top: 0; padding: 3.6rem 0; border-top: 1px solid var(--global-divider-color); scroll-margin-top: 4.5rem; }
  .home .sec-head { margin-bottom: 1.4rem; display: flex; align-items: flex-end; justify-content: space-between; gap: 1rem; }
  .home .sec-head h2 { margin: 0; font-size: clamp(1.5rem, 3vw, 2rem); font-weight: 800; line-height: 1.15; max-width: 30ch; }
  .home .sec-head a { font-size: 0.88rem; font-weight: 700; white-space: nowrap; padding-bottom: 0.3rem; }
  @media (max-width: 560px) { .home .sec-head { flex-wrap: wrap; } .home .sec-head a { width: 100%; } }
  .home .muted { color: var(--global-text-color-light); }
  .home .sec.tinted { position: relative; }
  .home .sec.tinted::before { content: ""; position: absolute; inset: 0 -100vw; left: 50%; transform: translateX(-50%); width: 100vw; background: color-mix(in srgb, var(--global-theme-color) 4%, var(--global-bg-color)); border-block: 1px solid var(--global-divider-color); z-index: -1; }
  .home .lede { max-width: 46rem; font-size: 1.05rem; line-height: 1.65; }

  /* ---------- hero: text left, schematic right ---------- */
  .hero { display: grid; grid-template-columns: 1fr 1.05fr; gap: 2.2rem; align-items: center; padding: 2.4rem 0 3.4rem; }
  .hero-title { font-size: clamp(2rem, 4.6vw, 2.9rem); font-weight: 800; line-height: 1.08; margin: 0 0 0.9rem; }
  .hero-title b { color: var(--global-theme-color); font-weight: 800; white-space: nowrap; }
  .hero-title::after { content: ""; display: block; width: 3.2rem; height: 3px; background: var(--global-theme-color); margin-top: 0.9rem; }
  .hero-tag { font-size: clamp(1.05rem, 2.3vw, 1.28rem); font-weight: 600; line-height: 1.4; margin: 0 0 0.9rem; font-style: italic; }
  .hero-lede { font-size: 1rem; line-height: 1.6; margin: 0 0 1.3rem; max-width: 34rem; }
  .hero-who { margin: 0 0 1.3rem; font-size: 0.9rem; line-height: 1.5; color: var(--global-text-color-light); }
  .hero-who b { color: var(--global-text-color); font-weight: 700; }
  .hero-actions { display: flex; flex-wrap: wrap; gap: 0.55rem; }
  .hero-actions a { padding: 0.42rem 1rem; border-radius: 6px; border: 1.5px solid var(--global-theme-color);
    font-weight: 600; font-size: 0.9rem; text-decoration: none !important; color: var(--global-theme-color); }
  .hero-actions a.primary { background: var(--global-theme-color); color: var(--global-bg-color) !important; }
  @media (max-width: 820px) { .hero { grid-template-columns: 1fr; gap: 1.4rem; } }

  /* schematic: understand-centered cycle inside a trustworthiness ring */
  .sv { margin: 0; }
  .sv svg { display: block; width: 100%; height: auto; max-width: 30rem; margin: 0 auto; }
  .sv .ring { fill: color-mix(in srgb, var(--global-theme-color) 5%, transparent); stroke: var(--global-divider-color); stroke-width: 1; }
  .sv .ring2 { fill: color-mix(in srgb, var(--global-theme-color) 4%, transparent); stroke: var(--global-divider-color); stroke-width: 1; stroke-dasharray: 2 4; }
  .sv .ringlbl { font-size: 11.5px; font-weight: 800; letter-spacing: 0.32em; fill: var(--global-text-color); }
  .sv .pr { font-size: 10.5px; font-weight: 600; fill: var(--global-text-color); }
  .sv .arc { fill: none; stroke: var(--global-theme-color); stroke-width: 2; stroke-dasharray: 6 4; }
  .sv .core { fill: color-mix(in srgb, var(--global-theme-color) 10%, var(--global-bg-color)); stroke: var(--global-theme-color); stroke-width: 1.2; }
  .sv .corelbl { font-size: 12.5px; font-weight: 800; letter-spacing: 0.02em; fill: var(--global-theme-color); }
  .sv .coresub { font-size: 8px; fill: var(--global-text-color-light); }
  .sv .node rect { fill: var(--global-card-bg-color); stroke: var(--global-divider-color); stroke-width: 1; }
  .sv .nlbl { font-size: 10.5px; font-weight: 800; letter-spacing: 0.04em; fill: var(--global-text-color); }
  .sv .nsub { font-size: 7.4px; fill: var(--global-text-color-light); }
  @media (prefers-reduced-motion: no-preference) {
    .sv .arc { animation: arcflow 1.6s linear infinite; }
    @keyframes arcflow { to { stroke-dashoffset: -10; } }
  }
  .sv-base { margin-top: 0.7rem; padding: 0.55rem 0.9rem 0.6rem; border: 1px solid var(--global-divider-color); border-radius: 8px;
    display: flex; flex-wrap: wrap; justify-content: center; align-items: center; gap: 0.15rem 0.3rem; font-size: 0.74rem; }
  .sv-base b { width: 100%; text-align: center; font-weight: 700; font-size: 0.68rem; letter-spacing: 0.1em; text-transform: uppercase; color: var(--global-text-color-light); margin-bottom: 0.25rem; }
  .sv-base span { font-weight: 600; display: inline-flex; align-items: center; gap: 0.3rem; }
  .sv-base span svg { width: 0.95rem; height: 0.95rem; fill: none; stroke: var(--global-theme-color); stroke-width: 1.4; stroke-linejoin: round; stroke-linecap: round; }
  .sv-base i { color: var(--global-theme-color); font-style: normal; }

  /* ---------- why ---------- */
  .why { display: grid; grid-template-columns: 1.1fr 0.9fr; gap: 2rem; align-items: center; }
  .why p { margin: 0; font-size: 1rem; line-height: 1.65; }
  .why .big { font-size: clamp(1.25rem, 2.6vw, 1.6rem); font-weight: 700; line-height: 1.35; padding-left: 1rem; border-left: 3px solid var(--global-theme-color); }
  @media (max-width: 720px) { .why { grid-template-columns: 1fr; } }

  /* ---------- three questions ---------- */
  .qs { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.4rem; margin-top: 2rem; }
  .qs div { padding: 0.9rem 0 0; border-top: 2px solid var(--global-theme-color); }
  .trustline { margin: 1.6rem 0 0; font-size: 0.9rem; }
  .qs h3 { margin: 0 0 0.3rem; font-size: 0.8rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; color: var(--global-theme-color); }
  .qs p { margin: 0; font-size: 0.98rem; font-weight: 600; line-height: 1.4; }
  @media (max-width: 720px) { .qs { grid-template-columns: 1fr; } }

  /* ---------- selected research cards ---------- */
  .cards { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1rem; }
  .card-r { padding: 1rem 1.1rem 0.9rem; border: 1px solid var(--global-divider-color); border-radius: 8px; display: flex; flex-direction: column; }
  .card-r h3 { margin: 0 0 0.35rem; font-size: 1.05rem; font-weight: 700; }
  .card-r p { margin: 0 0 0.5rem; font-size: 0.93rem; line-height: 1.5; flex: 1; }
  .card-r .meta { font-size: 0.8rem; color: var(--global-text-color-light); }
  .card-r .meta a { margin-right: 0.9rem; font-weight: 600; }
  .card-r { transition: border-color 0.15s; }
  .card-r:hover { border-color: color-mix(in srgb, var(--global-theme-color) 55%, transparent); }
  @media (max-width: 640px) { .cards { grid-template-columns: 1fr; } }

  /* ---------- about ---------- */
  .about-h { display: grid; grid-template-columns: 11rem 1fr; gap: 1.6rem; align-items: start; }
  .about-h img { width: 100%; border-radius: 8px; }
  .about-h p { margin: 0 0 0.8rem; font-size: 0.98rem; line-height: 1.6; }
  .about-h .links a { margin-right: 1rem; font-weight: 600; font-size: 0.9rem; }
  @media (max-width: 560px) { .about-h { grid-template-columns: 1fr; } .about-h img { max-width: 11rem; } }

  /* ---------- news ---------- */
  .home .news table { margin-bottom: 0; font-size: 0.92rem; }
  .home .news th { font-weight: 600; color: var(--global-text-color-light); white-space: nowrap; }
</style>

<section class="hero" id="top">
  <div>
    <p class="kicker">Trustworthy AI for molecular and systems biology &middot; Boston</p>
    <h1 class="hero-title">Trustworthy<br>World Models<br>for <b>Life Science</b></h1>
    <p class="hero-tag">Understand biological systems well enough to predict and act reliably.</p>
    <p class="hero-lede">We develop AI systems that learn representations of biological states, predict their responses to perturbations, and guide interventions across scales, from molecules to patients.</p>
    <p class="hero-who"><b>Hao Xu, Ph.D.</b><br>Investigator, Brigham and Women's Hospital<br>Instructor in Medicine, Harvard Medical School</p>
    <div class="hero-actions">
      <a class="primary" href="#vision">Research Vision</a>
      <a href="#selected">Selected Work</a>
    </div>
  </div>

  <figure class="sv" aria-label="Schematic: an understand-centered cycle of observe, represent, predict, and act, surrounded by a ring of trustworthiness principles, applied across biological scales from molecule to phenotype">
    <svg viewBox="0 0 480 430" role="img" aria-hidden="true">
      <defs>
        <marker id="ah" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
          <path d="M0,0 L10,5 L0,10 z" fill="var(--global-theme-color)"/>
        </marker>
        <path id="ringTop" d="M60,210 A180,180 0 0 1 420,210"/>
      </defs>
      <!-- outer ring -->
      <circle class="ring" cx="240" cy="210" r="200"/>
      <circle class="ring2" cx="240" cy="210" r="150"/>
      <text class="ringlbl"><textPath href="#ringTop" startOffset="50%" text-anchor="middle">TRUSTWORTHINESS</textPath></text>
      <!-- principles -->
      <text class="pr" x="109" y="86" text-anchor="middle">Interpretability</text>
      <text class="pr" x="371" y="80" text-anchor="middle">Mechanistic<tspan x="371" dy="12">Consistency</tspan></text>
      <text class="pr" x="38" y="214" text-anchor="middle">Uncertainty</text>
      <text class="pr" x="442" y="214" text-anchor="middle">Robustness</text>
      <text class="pr" x="109" y="346" text-anchor="middle">Validation</text>
      <text class="pr" x="371" y="346" text-anchor="middle">Generalization</text>
      <!-- cycle arcs (clockwise) -->
      <path class="arc" d="M282.3,118.4 A100,100 0 0 1 330.6,167.7" marker-end="url(#ah)"/>
      <path class="arc" d="M330.6,252.3 A100,100 0 0 1 282.3,301.6" marker-end="url(#ah)"/>
      <path class="arc" d="M197.7,301.6 A100,100 0 0 1 149.4,252.3" marker-end="url(#ah)"/>
      <path class="arc" d="M149.4,167.7 A100,100 0 0 1 197.7,118.4" marker-end="url(#ah)"/>
      <!-- center -->
      <circle class="core" cx="240" cy="210" r="62"/>
      <text class="corelbl" x="240" y="206" text-anchor="middle">UNDERSTAND</text>
      <text class="coresub" x="240" y="222" text-anchor="middle">Mechanisms &#183; Principles</text>
      <text class="coresub" x="240" y="234" text-anchor="middle">Biological organization</text>
      <!-- nodes -->
      <g class="node">
        <rect x="184" y="88" width="112" height="44" rx="10"/>
        <text class="nlbl" x="240" y="107" text-anchor="middle">OBSERVE</text>
        <text class="nsub" x="240" y="121" text-anchor="middle">Measure biological systems</text>
      </g>
      <g class="node">
        <rect x="296" y="188" width="112" height="44" rx="10"/>
        <text class="nlbl" x="352" y="207" text-anchor="middle">REPRESENT</text>
        <text class="nsub" x="352" y="221" text-anchor="middle">Learn biological states</text>
      </g>
      <g class="node">
        <rect x="184" y="288" width="112" height="44" rx="10"/>
        <text class="nlbl" x="240" y="307" text-anchor="middle">PREDICT</text>
        <text class="nsub" x="240" y="321" text-anchor="middle">Model responses to perturbation</text>
      </g>
      <g class="node">
        <rect x="72" y="188" width="112" height="44" rx="10"/>
        <text class="nlbl" x="128" y="207" text-anchor="middle">ACT</text>
        <text class="nsub" x="128" y="221" text-anchor="middle">Design interventions</text>
      </g>
    </svg>
    <div class="sv-base">
      <b>Across biological scales</b>
      <span><svg viewBox="0 0 20 20"><polygon points="10,3 16,6.5 16,13.5 10,17 4,13.5 4,6.5"/><line x1="16" y1="6.5" x2="19" y2="5"/></svg>Molecule</span><i>&rarr;</i>
      <span><svg viewBox="0 0 20 20"><circle cx="5" cy="14" r="2.6"/><circle cx="15" cy="6" r="2.6"/><line x1="7" y1="12.4" x2="13" y2="7.6"/><circle cx="15" cy="15" r="1.4"/></svg>Interaction</span><i>&rarr;</i>
      <span><svg viewBox="0 0 20 20"><circle cx="10" cy="10" r="2.2"/><circle cx="3.5" cy="5" r="1.6"/><circle cx="16.5" cy="5" r="1.6"/><circle cx="4" cy="16" r="1.6"/><circle cx="16" cy="16" r="1.6"/><line x1="10" y1="10" x2="3.5" y2="5"/><line x1="10" y1="10" x2="16.5" y2="5"/><line x1="10" y1="10" x2="4" y2="16"/><line x1="10" y1="10" x2="16" y2="16"/></svg>Network</span><i>&rarr;</i>
      <span><svg viewBox="0 0 20 20"><ellipse cx="10" cy="10" rx="8" ry="6.5"/><circle cx="8.5" cy="9.5" r="2.4"/></svg>Cell</span><i>&rarr;</i>
      <span><svg viewBox="0 0 20 20"><circle cx="10" cy="5" r="3"/><path d="M4,18 C4,12.5 6.5,10 10,10 C13.5,10 16,12.5 16,18"/></svg>Organism</span>
    </div>
  </figure>
</section>

<section class="sec" id="vision">
  <div class="sec-head"><div><p class="kicker"><span class="no">01</span>Vision</p><h2>Why World Models for Life Science?</h2></div><a href="{{ '/research/' | relative_url }}">Research program &rarr;</a></div>
  <div class="why">
    <p>Biological AI is increasingly powerful, but most models remain isolated within a single scale: molecules, proteins, cells, or patients. Living systems are connected across scales. A molecular intervention can alter binding, reshape interaction networks, change cellular states, and ultimately affect phenotype.</p>
    <p class="big">The challenge is not only to predict biology, but to understand how interventions propagate through it.</p>
  </div>
  <div class="qs">
    <div><h3>Understand</h3><p>What biological mechanisms govern response to intervention?</p></div>
    <div><h3>Predict</h3><p>What will happen under an unseen intervention, and how sure are we?</p></div>
    <div><h3>Intervene</h3><p>What intervention will drive biology toward a desired state?</p></div>
  </div>
  <p class="muted trustline">Across all three, one standard: interpretability, uncertainty, robustness, generalization, mechanistic consistency, and experimental validation.</p>
</section>

<section class="sec tinted" id="selected">
  <div class="sec-head"><div><p class="kicker"><span class="no">02</span>Selected research</p><h2>Selected Research</h2></div><a href="{{ '/publications/' | relative_url }}">All publications &rarr;</a></div>
  <div class="cards">
    <div class="card-r">
      <h3>ExplainBind</h3>
      <p>Learning interpretable physicochemical determinants of protein&ndash;ligand binding through explicit non-covalent interactions.</p>
      <div class="meta"><a href="{{ '/publications/#xu2026explainbind' | relative_url }}">bioRxiv 2026</a></div>
    </div>
    <div class="card-r">
      <h3>EvoRMD</h3>
      <p>Integrating biological context and evolutionary RNA language models for interpretable RNA modification prediction.</p>
      <div class="meta"><a href="{{ '/publications/#wang2026evormd' | relative_url }}">Genome Biology 2026</a></div>
    </div>
    <div class="card-r">
      <h3>Asymmetric Multimodal Learning</h3>
      <p>Learning richer molecular representations across complementary chemical modalities for property prediction and drug discovery.</p>
      <div class="meta"><a href="{{ '/publications/#wang2025advancing' | relative_url }}">J. Chem. Inf. Model. 2025</a><a href="{{ '/publications/#zhou2025multimodal' | relative_url }}">Commun. Chem. 2025</a></div>
    </div>
    <div class="card-r">
      <h3>NMRScape</h3>
      <p>Self-verifying molecular structure elucidation from experimental spectra, built on solvent-aware 2D NMR prediction and an annotated experimental benchmark.</p>
      <div class="meta"><a href="{{ '/publications/#li2025transpeaknet' | relative_url }}">Commun. Chem. 2025</a><a href="{{ '/publications/#li2025dnmrgym' | relative_url }}">LoG 2025</a></div>
    </div>
  </div>
</section>

<section class="sec" id="about">
  <div class="sec-head"><div><p class="kicker"><span class="no">03</span>About</p><h2>About Hao</h2></div><a href="{{ '/about/' | relative_url }}">Appointments and education &rarr;</a></div>
  <div class="about-h">
    <img src="{{ '/assets/img/prof_pic.png' | relative_url }}" alt="Hao Xu">
    <div>
      <p>Hao Xu is an Investigator at Brigham and Women's Hospital and an Instructor in Medicine at Harvard Medical School. His research develops trustworthy AI for molecular and systems biology, with a long-term goal of building world models that connect molecular interventions to system-level biological responses.</p>
      <p class="links">
        <a href="{{ '/cv/' | relative_url }}">CV</a>
        <a href="https://scholar.google.com/citations?user=tcYaFAcAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
        <a href="https://github.com/GainGod-Xu" target="_blank" rel="noopener">GitHub</a>
        <a href="https://orcid.org/0000-0002-9795-5633" target="_blank" rel="noopener">ORCID</a>
        <a href="mailto:haoxu0303@gmail.com">Email</a>
      </p>
    </div>
  </div>
</section>

<section class="sec" id="news">
  <div class="sec-head"><div><p class="kicker"><span class="no">04</span>News</p><h2>News</h2></div></div>
  {% include news.liquid limit=true %}
</section>
