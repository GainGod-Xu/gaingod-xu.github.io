---
layout: page
permalink: /
title: XLab
description: News from XLab.
---

## News

<div class="mt-2" markdown="1">

{% include news.liquid limit=true %}

</div>

## Mission
{: .mt-4 }

<style>
  /* Micro-to-Macro mission diagram */
  .mission {
    margin: 0.75rem 0 0;
  }
  .mission-lead {
    text-align: center;
    margin-bottom: 1.25rem;
  }
  .mission-lead strong {
    display: block;
    font-weight: 700;
    font-size: 1.35rem;
    color: var(--global-theme-color);
  }
  .mission-lead span {
    color: var(--global-text-color-light);
    font-size: 0.95rem;
  }
  .mission-body {
    display: grid;
    grid-template-columns: 1.6rem repeat(3, 1fr);
    gap: 0.9rem;
  }
  /* Shared micro -> macro scale axis */
  .mission-axis {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 4.2rem;
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    color: var(--global-text-color-light);
  }
  .mission-axis i {
    flex: 1;
    width: 3px;
    margin: 0.4rem 0;
    border-radius: 2px;
    background: linear-gradient(to bottom, var(--global-divider-color), var(--global-theme-color));
    position: relative;
  }
  .mission-axis i::after {
    content: "";
    position: absolute;
    bottom: -2px;
    left: 50%;
    transform: translateX(-50%);
    border: 6px solid transparent;
    border-top-color: var(--global-theme-color);
    border-bottom: 0;
  }
  .mission-axis b {
    writing-mode: vertical-rl;
    transform: rotate(180deg);
  }
  .track {
    display: flex;
    flex-direction: column;
  }
  .track-head {
    padding: 0.55rem 0.75rem;
    border-radius: 8px;
    background: var(--accent);
    color: #fff;
    min-height: 3.6rem;
    margin-bottom: 0.6rem;
  }
  .track-head span {
    color: #fff !important;
  }
  .track-head .track-no {
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    opacity: 0.85;
  }
  .track-head .track-name {
    display: block;
    font-weight: 700;
    font-size: 1rem;
  }
  .track-head .track-name i {
    margin-right: 0.35rem;
  }
  .track-sub {
    font-size: 0.78rem;
    color: var(--global-text-color-light);
    margin: -0.2rem 0 0.6rem;
    min-height: 2.7em;
    line-height: 1.35;
  }
  .track ol {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    flex: 1;
  }
  .track li {
    position: relative;
    flex: 1;
    padding: 0.5rem 0.7rem 0.5rem 2.3rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 6px;
    background: var(--global-card-bg-color);
    font-size: 0.8rem;
    line-height: 1.35;
    color: var(--global-text-color-light);
  }
  .track li + li {
    margin-top: 1.1rem;
  }
  /* connector arrow between levels */
  .track li + li::after {
    content: "";
    position: absolute;
    top: -1rem;
    left: 50%;
    transform: translateX(-50%);
    border: 5px solid transparent;
    border-top: 7px solid var(--accent);
    border-bottom: 0;
    margin-top: 0.15rem;
  }
  .track li + li::before {
    content: "";
    position: absolute;
    top: -1.05rem;
    left: 50%;
    width: 2px;
    height: 0.55rem;
    transform: translateX(-50%);
    background: var(--accent);
  }
  .track li:last-child {
    background: color-mix(in srgb, var(--accent) 10%, var(--global-card-bg-color));
    border-color: color-mix(in srgb, var(--accent) 45%, transparent);
  }
  .track li strong {
    display: block;
    font-weight: 700;
    color: var(--global-text-color);
    font-size: 0.88rem;
  }
  .track li .lvl {
    position: absolute;
    left: 0.6rem;
    top: 0.55rem;
    width: 1.25rem;
    height: 1.25rem;
    border-radius: 50%;
    background: var(--accent);
    color: #fff;
    font-size: 0.7rem;
    font-weight: 700;
    line-height: 1.25rem;
    text-align: center;
  }
  /* Mission bar */
  .mission-bar {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.6rem 1rem;
    margin-top: 1.2rem;
    padding: 0.8rem 1rem;
    border-radius: 8px;
    border: 1px solid var(--global-divider-color);
    background: color-mix(in srgb, var(--global-theme-color) 8%, var(--global-card-bg-color));
  }
  .mission-bar .goal {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-weight: 700;
    color: var(--global-text-color);
  }
  .mission-bar .goal i {
    color: var(--global-theme-color);
    font-size: 1.15rem;
  }
  .mission-bar .sep {
    color: var(--global-theme-color);
    font-weight: 700;
  }
  .mission-bar .tag {
    font-size: 0.7rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    color: var(--global-text-color-light);
    padding-right: 1rem;
    border-right: 1px solid var(--global-divider-color);
  }
  @media (max-width: 768px) {
    .mission-body {
      grid-template-columns: 1fr;
    }
    .mission-axis {
      display: none;
    }
    .track-head,
    .track-sub {
      min-height: 0;
    }
    .track + .track {
      margin-top: 0.6rem;
    }
    .mission-bar .tag {
      width: 100%;
      text-align: center;
      border-right: 0;
      padding-right: 0;
    }
  }
</style>

<figure class="mission" aria-label="XLab mission: Micro-to-Macro Mechanistic AI, one principle applied across three research tracks">
  <div class="mission-lead">
    <strong>Micro-to-Macro Mechanistic AI</strong>
    <span>Building AI that links micro-scale dynamics to macro-scale behavior &mdash; one principle, three research tracks.</span>
  </div>
  <div class="mission-body">
    <div class="mission-axis" aria-hidden="true"><b>MICRO</b><i></i><b>MACRO</b></div>
    <div class="track" style="--accent: #7b52c7;">
      <div class="track-head"><span class="track-no">TRACK I</span><span class="track-name"><i class="fa-solid fa-microchip"></i>Fundamental AI</span></div>
      <div class="track-sub">From parameter dynamics to reliable model behavior</div>
      <ol>
        <li><span class="lvl">1</span><strong>Parameter Dynamics</strong>Parameter sensitivity and structure; efficient, task-aware adaptation</li>
        <li><span class="lvl">2</span><strong>Multimodal Understanding</strong>Visual grounding and cross-modal reasoning</li>
        <li><span class="lvl">3</span><strong>Visual Alignment</strong>Counterfactual alignment; mitigating visual laziness and modality bias</li>
        <li><span class="lvl">4</span><strong>Reliable AI Systems</strong>Robust, efficient multimodal intelligence across tasks and domains</li>
      </ol>
    </div>
    <div class="track" style="--accent: #3a7bd5;">
      <div class="track-head"><span class="track-no">TRACK II</span><span class="track-name"><i class="fa-solid fa-dna"></i>Life Science</span></div>
      <div class="track-sub">From molecular mechanisms to health outcomes</div>
      <ol>
        <li><span class="lvl">1</span><strong>Molecular Mechanisms</strong>Physicochemical drivers of binding, catalysis, and conformational change</li>
        <li><span class="lvl">2</span><strong>Cellular Systems</strong>Molecular networks, pathways, regulation, and cell states</li>
        <li><span class="lvl">3</span><strong>Organismal Mechanisms</strong>Integrated physiology, disease, and treatment response</li>
        <li><span class="lvl">4</span><strong>Health Outcomes</strong>Clinical and population-level diagnosis, prognosis, and intervention</li>
      </ol>
    </div>
    <div class="track" style="--accent: #3fa65b;">
      <div class="track-head"><span class="track-no">TRACK III</span><span class="track-name"><i class="fa-solid fa-atom"></i>Materials Science</span></div>
      <div class="track-sub">From atomic interactions to materials discovery and impact</div>
      <ol>
        <li><span class="lvl">1</span><strong>Atomic Interactions</strong>Atomic structure, bonding, electrons, and defects</li>
        <li><span class="lvl">2</span><strong>Structure&ndash;Property Mechanisms</strong>Surfaces, phases, transport, and stability</li>
        <li><span class="lvl">3</span><strong>Materials Discovery &amp; Catalysis</strong>ML-potential&ndash;guided search and generative design</li>
        <li><span class="lvl">4</span><strong>Applications &amp; Impact</strong>Materials for energy, environment, electronics, and beyond</li>
      </ol>
    </div>
  </div>
  <div class="mission-bar">
    <span class="tag">OUR MISSION</span>
    <span class="goal"><i class="fa-solid fa-brain" aria-hidden="true"></i>Understand mechanisms</span>
    <span class="sep" aria-hidden="true">&rarr;</span>
    <span class="goal"><i class="fa-solid fa-sliders" aria-hidden="true"></i>Shape behaviors</span>
    <span class="sep" aria-hidden="true">&rarr;</span>
    <span class="goal"><i class="fa-solid fa-earth-americas" aria-hidden="true"></i>Enable discovery</span>
  </div>
</figure>
