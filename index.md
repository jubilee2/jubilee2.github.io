---
layout: default
title: Jubilee Tan
permalink: /
---

# Jubilee Tan

<div class="home-hero">
  <img
    class="home-avatar"
    src="{{ '/assets/e379bc5f-b6cd-406e-8694-de4ddaf624a4.png' | relative_url }}"
    alt="Headshot of Jubilee Tan"
  />
  <div>
    <p><strong>Senior Application Developer | Research Informatics & Healthcare Data Engineering</strong></p>
    <div class="hero-cta-group" aria-label="Primary contact links">
      <a class="hero-cta" href="{{ '/assets/Jubilee_Tan_CV.pdf' | relative_url }}">Download CV (PDF)</a>
      <a class="hero-cta" href="https://www.linkedin.com/in/jubilee-tan-17b642109/" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      <a class="hero-cta" href="https://github.com/jubilee2" target="_blank" rel="noopener noreferrer">GitHub</a>
      <a class="hero-cta" href="mailto:jubilee2@gmail.com">Email</a>
    </div>
    <p>I build reliable data systems for clinical and biomedical research, with experience across large-scale cohort analytics, automated reporting, and REDCap-based study operations.</p>
  </div>
</div>

## Highlights

<div class="home-card-grid home-card-grid--highlights">
  <article class="home-card">
    <h3>Years</h3>
    <p class="home-card__metric">13+ years</p>
    <p>Professional software and data platform experience.</p>
  </article>
  <article class="home-card">
    <h3>Platforms</h3>
    <p class="home-card__metric">BigQuery · Databricks · REDCap</p>
    <p>Cross-platform delivery for cohort analytics, automation, and integrations.</p>
  </article>
  <article class="home-card">
    <h3>Impact</h3>
    <p class="home-card__metric">200+ reports/week</p>
    <p>Scaled recurring reporting and operational workflows for research teams.</p>
  </article>
</div>

## Featured Projects

{% assign featured_projects = site.projects | sort: "order" | slice: 0, 4 %}
<div class="home-card-grid">
  {% for project in featured_projects %}
  <article class="home-card home-card--project">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    {% if project.home_metrics and project.home_metrics.size > 0 %}
    <ul>
      {% for metric in project.home_metrics limit: 2 %}
      <li>{{ metric }}</li>
      {% endfor %}
    </ul>
    {% else %}
    <p>{{ project.summary }}</p>
    {% endif %}
  </article>
  {% endfor %}
</div>

## Quick Links

- [About]({{ '/about/' | relative_url }})
- [Projects]({{ '/projects/' | relative_url }})
- [CV]({{ '/cv/' | relative_url }})
- [Contact]({{ '/contact/' | relative_url }})
