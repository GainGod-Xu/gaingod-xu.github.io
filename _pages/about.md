---
layout: about
title: About
permalink: /about/
nav: true
nav_order: 7
subtitle: Investigator, Brigham and Women's Hospital &bull; Instructor in Medicine, Harvard Medical School

profile:
  align: right
  image: prof_pic.png
  image_circular: false
  more_info: >
    <p style="font-size: 1.5rem;">
      <a href="mailto:haoxu0303@gmail.com" title="Email"><i class="fa-solid fa-envelope"></i></a>
      <a href="https://github.com/GainGod-Xu" target="_blank" title="GitHub"><i class="fa-brands fa-github"></i></a>
      <a href="https://www.linkedin.com/in/hao-xu-62bb11169/" target="_blank" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>
      <a href="https://scholar.google.com/citations?user=tcYaFAcAAAAJ&hl=en" target="_blank" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
      <a href="https://orcid.org/0000-0002-9795-5633" target="_blank" title="ORCID"><i class="ai ai-orcid"></i></a>
    </p>
    <style>
      @media (min-width: 576px) {
        .profile {
          width: 24%;
        }
      }
    </style>

announcements:
  enabled: false
selected_papers: false
social: false
---

Hao Xu is an Investigator at Brigham and Women's Hospital and an Instructor in Medicine at Harvard Medical School. His research develops trustworthy AI for molecular and systems biology, with a long-term goal of building world models that connect molecular interventions to system-level biological responses. See [Research]({{ '/research/' | relative_url }}) for the research program and current directions.

<style>
  .about-list { list-style: none; margin: 0; padding: 0; }
  .about-list li { display: grid; grid-template-columns: 9.5rem 1fr; gap: 0.2rem 1rem; padding: 0.45rem 0; border-bottom: 1px solid var(--global-divider-color); font-size: 0.95rem; }
  .about-list li:last-child { border-bottom: 0; }
  .about-list .when { color: var(--global-text-color-light); font-size: 0.86rem; white-space: nowrap; }
  .about-list .what strong { font-weight: 700; }
  .about-list .affiliated-role { display: block; margin-top: 0.45rem; }
  .about-list .what span { display: block; color: var(--global-text-color-light); font-size: 0.86rem; }
  .about h2 { margin: 1.8rem 0 0.5rem; font-size: 1.15rem; font-weight: 700; padding-bottom: 0.3rem; border-bottom: 1px solid var(--global-divider-color); }
  .about h2[id] { scroll-margin-top: 5rem; }
  .about .service-list li + li { margin-top: 0.65rem; }
  @media (max-width: 560px) { .about-list li { grid-template-columns: 1fr; gap: 0; } }
</style>

<div class="about">

<h2>Appointments</h2>
<ul class="about-list">
  <li><span class="when">Apr 2026 &ndash; present</span><span class="what"><strong>Investigator &amp; Instructor in Medicine</strong><span>Department of Medicine, Brigham and Women's Hospital, Harvard Medical School</span></span></li>
  <li>
    <span class="when">Jun 2024 &ndash; Apr 2026</span>
    <span class="what">
      <strong>Research Fellow</strong>
      <span>Department of Medicine, Brigham and Women's Hospital, Harvard Medical School</span>
      <strong class="affiliated-role">Affiliated Research Fellow</strong>
      <span>Network Science Institute, Northeastern University</span>
    </span>
  </li>
  <li><span class="when">Apr 2023 &ndash; May 2024</span><span class="what"><strong>Postdoctoral Associate</strong><span>Department of Computer Science, Brandeis University; affiliated with GlycoMIP (NSF Materials Innovation Platform)</span></span></li>
</ul>

<h2>Education</h2>
<ul class="about-list">
  <li><span class="when">2017 &ndash; 2022</span><span class="what"><strong>Ph.D. in Chemistry</strong><span>Boston College</span></span></li>
  <li><span class="when">2020 &ndash; 2022</span><span class="what"><strong>M.S. in Computer Science</strong><span>Georgia Institute of Technology</span></span></li>
  <li><span class="when">2015 &ndash; 2017</span><span class="what"><strong>M.S. in Chemistry</strong><span>Southern Methodist University</span></span></li>
  <li><span class="when">2011 &ndash; 2015</span><span class="what"><strong>B.S. in Chemistry &amp; B.Econ. in Finance</strong><span>China Agricultural University</span></span></li>
</ul>

<h2 id="academic-service">Academic Service</h2>
<ul class="service-list">
  {% assign service = site.data.cv.cv.sections['Academic Service'] %}
  {% for item in service %}
    <li>{{ item.bullet | markdownify }}</li>
  {% endfor %}
</ul>

<h2 id="teaching">Teaching</h2>
<ul class="about-list">
  <li><span class="when">2024 &ndash; 2026</span><span class="what"><strong>Brigham and Women’s Hospital</strong><span>Organized and taught two Python and machine learning workshops for research group members.</span></span></li>
  <li><span class="when">2017 &ndash; 2022</span><span class="what"><strong>Boston College</strong><span>Teaching assistant for Organic Chemistry, General Chemistry, and Advanced Method I &amp; II laboratory courses.</span></span></li>
  <li><span class="when">2015 &ndash; 2017</span><span class="what"><strong>Southern Methodist University</strong><span>Teaching assistant for the Inorganic Chemistry laboratory course.</span></span></li>
</ul>

</div>
