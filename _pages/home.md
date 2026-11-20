---
layout: home
permalink: /
title: Home
description: Hao Xu develops trustworthy AI for biomedicine, from molecular mechanisms to precision medicine.
---

<section class="home-intro">
  <div>
    <h1>Trustworthy AI for <em>Biomedicine</em></h1>
    <p class="home-deck">From molecular mechanisms to precision medicine</p>
    <p class="home-appointment">Investigator, Brigham and Women’s Hospital<br>Instructor in Medicine, Harvard Medical School</p>
    <div class="editorial-actions">
      <a class="editorial-button primary" href="{{ '/research/' | relative_url }}">Explore research</a>
      <a class="editorial-button" href="{{ '/publications/' | relative_url }}">Publications</a>
    </div>
  </div>
  <figure class="home-image">
    <img src="{{ '/assets/img/research/biomedicine-hero.webp' | relative_url }}" width="1440" height="960" alt="" fetchpriority="high">
    <figcaption class="fig-note">Conceptual illustration of molecular interactions, networks, and cell states.</figcaption>
  </figure>
</section>

<section class="home-section" aria-labelledby="selected-research">
  <h2 id="selected-research">Selected research</h2>
  <div class="home-projects">
    <article>
      <p class="kicker">Molecular recognition</p>
      <h3><a href="{{ '/research/#molecular-recognition' | relative_url }}">ExplainBind</a></h3>
      <p>Explaining protein–ligand binding through non-covalent interactions.</p>
    </article>
    <article>
      <p class="kicker">RNA biology</p>
      <h3><a href="{{ '/research/#rna-biology' | relative_url }}">EvoRMD</a></h3>
      <p>Predicting RNA modification sites with evolutionary and biological context.</p>
    </article>
    <article>
      <p class="kicker">Network medicine</p>
      <h3><a href="{{ '/research/#network-medicine' | relative_url }}">Disease networks</a></h3>
      <p>Connecting molecular interactions to disease modules and drug repurposing.</p>
    </article>
  </div>
</section>

<section class="home-section" id="news" aria-labelledby="latest-news">
  <div class="editorial-section-heading">
    <h2 id="latest-news">Latest news</h2>
    <a href="{{ '/news/' | relative_url }}">News archive</a>
  </div>
  {% include editorial-news.liquid limit=site.news_limit %}
</section>
