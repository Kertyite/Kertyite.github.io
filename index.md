---
layout: default
title: Home
description: Research portfolio for Seo Younggeon.
---
<div class="page-shell">
  <header class="hero">
    <nav class="topbar">
      <div class="brand">Kertyite</div>
      <div class="nav-links">
        <a href="#about">About</a>
        <a href="#research">Research</a>
        <a href="{{ '/publications/' | relative_url }}">Publications</a>
      </div>
    </nav>
    <div class="hero-copy">
      <p class="eyebrow">Research Portfolio</p>
      <h1>Seo Younggeon</h1>
      <p class="lead">Master's student in Industrial and Management Engineering working on battery prognostics, health management, and reliable edge AI.</p>
      <div class="hero-actions">
        <a class="button primary" href="{{ '/publications/' | relative_url }}">View Publications</a>
        <a class="button secondary" href="mailto:tjdudrjs8745@hanyang.ac.kr">Contact</a>
      </div>
    </div>
  </header>

  <main>
    <section id="about" class="panel two-column">
      <div>
        <p class="section-label">About</p>
        <h2>Focused on practical reliability problems.</h2>
      </div>
      <div>
        <p>I study data-driven prognostics for lithium-ion batteries, with emphasis on state-of-health prediction, model compression, and deployable ML systems.</p>
        <p>I am currently affiliated with Hanyang University in Seoul.</p>
      </div>
    </section>

    <section id="research" class="panel research-grid">
      <article>
        <p class="section-label">Research Area</p>
        <h3>Battery SOH Estimation</h3>
        <p>Sequence models and physically meaningful signals for robust state estimation.</p>
      </article>
      <article>
        <p class="section-label">Research Area</p>
        <h3>Edge AI Compression</h3>
        <p>Reducing model cost while preserving reliability for deployment on constrained devices.</p>
      </article>
      <article>
        <p class="section-label">Research Area</p>
        <h3>Industrial Reliability</h3>
        <p>Methods that move from benchmark performance toward maintainable field systems.</p>
      </article>
    </section>
  </main>
</div>
