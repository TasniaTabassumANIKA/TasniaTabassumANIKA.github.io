---
layout: default
title: Research
permalink: /research/
---
<div class="page-head">
  <div class="container">
    <h1>Research</h1>
    <p>My research portfolio connects sustainable infrastructure, urban environmental systems, spatial analysis, and data-driven modeling.</p>
  </div>
</div>

<section class="container">
  <h2 class="section-title">Current research direction</h2>
  <hr class="rule">
  <p>My current work emphasizes computational and empirical approaches for understanding infrastructure–environment interactions. A major focus is the use of monitoring data, GIS, statistical methods, and explainable machine learning to quantify environmental exposure and identify the factors that drive spatial and temporal variability.</p>

  <div class="card-grid" style="margin-top:28px;">
    {% for project in site.data.projects %}
      <article class="card">
        <h3>{{ project.title }}</h3>
        <p>{{ project.summary }}</p>
        {% if project.status %}<p class="small" style="margin-top:10px;"><strong>Status:</strong> {{ project.status }}</p>{% endif %}
        <div class="tag-wrap">
          {% for tag in project.tags %}<span class="tag">{{ tag }}</span>{% endfor %}
        </div>
      </article>
    {% endfor %}
  </div>
</section>

<section class="container" style="padding-top:10px;">
  <h2 class="section-title">Research themes</h2>
  <hr class="rule">
  <div class="card-grid">
    <div class="card"><h3>Sustainable Infrastructure Materials</h3><p>AI-assisted concrete strength prediction, geopolymer systems, waste-derived materials, and environmentally conscious construction materials.</p></div>
    <div class="card"><h3>Urban Environmental Systems</h3><p>Air quality in transportation environments, PM<sub>2.5</sub> exposure, urban mobility settings, and environmental monitoring.</p></div>
    <div class="card"><h3>Spatial &amp; Spatiotemporal Modeling</h3><p>GIS-based mapping, spatial variability, monitoring datasets, and methods for linking environmental conditions with infrastructure and urban context.</p></div>
    <div class="card"><h3>Machine Learning &amp; Explainable AI</h3><p>Predictive modeling, feature importance, explainability, and decision-support frameworks for civil and environmental engineering problems.</p></div>
  </div>
</section>
