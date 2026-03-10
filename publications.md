---
layout: default
title: Publications
description: Selected publications by Seo Younggeon.
permalink: /publications/
---
<div class="page-shell page-shell-narrow">
  <header class="subpage-header">
    <a class="back-link" href="{{ '/' | relative_url }}">Back to Home</a>
    <p class="eyebrow">Publications</p>
    <h1>Selected Work</h1>
    <p class="lead">A simplified Jekyll publication list.</p>
  </header>

  <main class="publication-list">
    {% assign publications = site.publications | sort: 'year' | reverse %}
    {% for publication in publications %}
    <article class="publication-card">
      <p class="pub-year">{{ publication.year }}</p>
      <h2><a href="{{ publication.url | relative_url }}">{{ publication.title }}</a></h2>
      <p class="pub-meta">{{ publication.authors }}</p>
      <p class="pub-meta">{{ publication.venue }}</p>
      {% if publication.award %}
      <p class="pub-badge">{{ publication.award }}</p>
      {% endif %}
    </article>
    {% endfor %}
  </main>
</div>
