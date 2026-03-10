---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in Industrial and Management Engineering, Hanyang University ERICA, 2025 - Present
* B.S. in Applied Mathematics, Hanyang University ERICA, 2020 - 2025
* B.S. in Computer Science (Double Major), Hanyang University ERICA, 2021 - 2025

Research interests
======
* Prognostics and Health Management for lithium-ion batteries
* Battery state-of-health estimation
* Physics-Informed Neural Networks
* Time-series forecasting
* Edge AI and model compression

Research and industry experience
======
* Intern, CMES AI ROBOTICS, Mar - Jun 2024
  * Developed a Human Action Recognition and safety monitoring model demonstrated at KOREA MAT 2024.
  * Investigated model architectures for improved small object detection performance.
  * Participated in technical seminars reviewing recent computer vision research.

Honors and awards
======
* Best Paper Award, IEEE Global Reliability and PHM Conference, 2025
* Excellence in Presentation Award, Korean Reliability Society Spring Conference, 2025
* Excellence Scholarship for Master's Students in Science and Engineering, 2025

Publications
======
{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h3>{{ category[1].title }}</h3>
        <ul>
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single-cv.html %}
    {% endfor %}
    {% if title_shown %}
        </ul>
    {% endif %}
  {% endfor %}
{% else %}
  <ul>
  {% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}
  </ul>
{% endif %}
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  {% if site.teaching and site.teaching.size > 0 %}
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  {% else %}
  No formal teaching appointments listed yet.
  {% endif %}
  
Professional links
======
* [Google Scholar](https://scholar.google.com/citations?user=zrN7X3gAAAAJ&hl=ko)
* [ORCID](https://orcid.org/0009-0007-7334-4284)
* [GitHub](https://github.com/Kertyite)
