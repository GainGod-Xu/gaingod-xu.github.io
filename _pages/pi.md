---
layout: about
title: PI
permalink: /pi/
nav: true
nav_order: 2
subtitle: Investigator, Brigham and Women's Hospital &bull; Instructor in Medicine, Harvard Medical School

profile:
  align: right
  image: prof_pic.png
  image_circular: false # crops the image to make it circular
  more_info: >
    <p style="font-size: 1.5rem;">
      <a href="mailto:haoxu0303@gmail.com" title="Email"><i class="fa-solid fa-envelope"></i></a>
      <a href="https://github.com/GainGod-Xu" target="_blank" title="GitHub"><i class="fa-brands fa-github"></i></a>
      <a href="https://www.linkedin.com/in/hao-xu-62bb11169/" target="_blank" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>
      <a href="https://scholar.google.com/citations?user=tcYaFAcAAAAJ&hl=en" target="_blank" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
      <a href="https://orcid.org/0000-0002-9795-5633" target="_blank" title="ORCID"><i class="ai ai-orcid"></i></a>
    </p>
    <p>
      <em>Courage is the grace under pressure.</em>
    </p>
    <style>
      @media (min-width: 576px) {
        .profile {
          width: 22%;
        }
      }
    </style>

announcements:
  enabled: false
selected_papers: false # moved to the XLab page
social: false # includes social icons at the bottom of the page
---

Dr. Hao Xu is currently an Investigator at Brigham and Women's Hospital and Instructor in Medicine at Harvard Medical School. His research pioneers **Micro-to-Macro Mechanistic AI**, a research paradigm that seeks to understand and control complex systems by linking microscopic mechanisms to macroscopic behaviors across both artificial intelligence and scientific discovery. In fundamental AI, he develops parameter-efficient fine-tuning (PEFT) and multimodal foundation models that connect micro-scale parameter dynamics with emergent model behaviors. In AI for Science, he combines physicochemical mechanisms with 3D geometric deep learning to reveal molecular-level principles governing biological function, enabling more interpretable molecular discovery and precision medicine.

Research interests include:

- AI for Science
- AI for Healthcare
- Quantum Computing for Scientific Discovery
- Large Language Model Reasoning
- Vision Understanding and Generation

<style>
  .pi-card {
    border-left: 4px solid var(--accent, var(--global-theme-color));
  }
  .pi-card > h3 {
    color: var(--accent, var(--global-theme-color));
  }

  /* Career path: chemistry -> computation -> AI for science -> medicine */
  .path {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 0.5rem;
    margin: 0;
    padding: 0;
    list-style: none;
  }
  .path li {
    position: relative;
    padding: 1.1rem 0.6rem 0 0;
  }
  .path li::before {
    content: "";
    position: absolute;
    top: 0.35rem;
    left: 0;
    right: -0.5rem;
    height: 3px;
    background: var(--accent);
  }
  .path li:last-child::before {
    right: 0;
    background: linear-gradient(to right, var(--accent) 60%, transparent);
  }
  .path li::after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 0.85rem;
    height: 0.85rem;
    border-radius: 50%;
    background: var(--global-card-bg-color);
    border: 3px solid var(--accent);
  }
  .path-years {
    display: block;
    font-size: 0.75rem;
    font-weight: 700;
    color: var(--global-text-color-light);
  }
  .path-stage {
    display: block;
    font-weight: 700;
    color: var(--accent);
    margin: 0.1rem 0 0.2rem;
  }
  .path-where {
    display: block;
    font-size: 0.82rem;
    line-height: 1.35;
  }
  @media (max-width: 640px) {
    .path {
      grid-template-columns: 1fr;
      gap: 0;
    }
    .path li {
      padding: 0 0 0.9rem 1.5rem;
    }
    .path li::before {
      top: 0.4rem;
      bottom: -0.4rem;
      left: 0.35rem;
      right: auto;
      width: 3px;
      height: auto;
    }
    .path li:last-child::before {
      background: linear-gradient(to bottom, var(--accent) 40%, transparent);
    }
  }
</style>

<div class="card pi-card mt-3 p-3">
  <h3 class="card-title font-weight-medium">Path</h3>
  <ol class="path">
    <li style="--accent: #3fa65b;">
      <span class="path-years">2011&ndash;2017</span>
      <span class="path-stage">Chemistry</span>
      <span class="path-where">B.S., China Agricultural University &middot; M.S. Computational Chemistry, SMU</span>
    </li>
    <li style="--accent: #7b52c7;">
      <span class="path-years">2017&ndash;2022</span>
      <span class="path-stage">Chemistry + Computing</span>
      <span class="path-where">Ph.D. Chemistry, Boston College &middot; M.S. Computer Science, Georgia Tech</span>
    </li>
    <li style="--accent: #3a7bd5;">
      <span class="path-years">2023&ndash;2024</span>
      <span class="path-stage">AI for Science</span>
      <span class="path-where">Postdoc, Computer Science, Brandeis University &middot; GlycoMIP</span>
    </li>
    <li style="--accent: #d9534f;">
      <span class="path-years">2024&ndash;now</span>
      <span class="path-stage">AI for Medicine</span>
      <span class="path-where">Brigham and Women's Hospital &amp; Harvard Medical School</span>
    </li>
  </ol>
</div>

<div class="card pi-card mt-3 p-3" style="--accent: #3a7bd5;">
  <h3 class="card-title font-weight-medium">Work Experience</h3>
  <ul class="mb-0">
    <li><strong>Apr 2026&ndash;Present:</strong> Investigator & Instructor, Department of Medicine, Brigham and Women's Hospital, Harvard Medical School</li>
    <li><strong>Jun 2024&ndash;Apr 2026:</strong> Research Fellow, Department of Medicine, Brigham and Women's Hospital, Harvard Medical School</li>
    <li><strong>Jun 2024&ndash;Apr 2026:</strong> Affiliated Research Fellow, Department of Physics, Network Science Institute, Northeastern University</li>
    <li><strong>Apr 2023&ndash;May 2024:</strong> Postdoctoral Associate, Department of Computer Science, Brandeis University</li>
    <li><strong>Apr 2023&ndash;May 2024:</strong> Affiliated Postdoctoral Associate, GlycoMIP (NSF-funded Materials Innovation Platform, Virginia Tech & University of Georgia)</li>
  </ul>
</div>

<div class="card pi-card mt-3 p-3" style="--accent: #7b52c7;">
  <h3 class="card-title font-weight-medium">Education</h3>
  <ul class="mb-0">
    <li><strong>Aug 2017&ndash;Dec 2022:</strong> Ph.D. in Chemistry, Boston College</li>
    <li><strong>Aug 2020&ndash;Aug 2022:</strong> M.S. in Computer Science, Georgia Institute of Technology</li>
    <li><strong>Aug 2015&ndash;May 2017:</strong> M.S. in Computational Chemistry, Southern Methodist University</li>
    <li><strong>Sep 2011&ndash;Jul 2015:</strong> B.S. in Chemistry & B.Econ. in Finance, China Agricultural University</li>
  </ul>
</div>

<div class="card pi-card mt-3 p-3" style="--accent: #3fa65b;">
  <h3 class="card-title font-weight-medium">Academic Service</h3>
  <p><strong>Reviewer for Journals (JCR Q1):</strong> Nature Communications, Communications Chemistry, Journal of Cheminformatics, Journal of Chemical Information and Modeling, Quantum Science and Technology, Journal of Medical Internet Research, ACM Transactions on Intelligent Systems and Technology, IEEE Transactions on Medical Imaging, IEEE Transactions on Pattern Analysis and Machine Intelligence, Knowledge-Based Systems, Scientific Reports, Patterns, Sustainable Food Technology</p>
  <p class="mb-0"><strong>Reviewer for Conferences:</strong> ACM MM, COLM, NeurIPS, CVPR, COLING, ECCV</p>
</div>
