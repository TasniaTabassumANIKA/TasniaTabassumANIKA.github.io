---
layout: default
title: Education & Work
permalink: /education-work/
---
<div class="page-head">
  <div class="container">
    <h1>Education &amp; Work</h1>
    <p>Academic training, research experience, and professional appointments.</p>
  </div>
</div>

<section class="container">
  <h2 class="section-title">Education</h2>
  <hr class="rule">
  <div class="timeline">
    {% for item in site.data.education %}
      <div class="timeline-item">
        <div class="timeline-year">{{ item.years }}</div>
        <div class="timeline-title">{{ item.degree }}</div>
        <div class="timeline-meta">{{ item.institution }}</div>
        {% if item.detail %}<div class="small">{{ item.detail }}</div>{% endif %}
      </div>
    {% endfor %}
  </div>

  <h2 class="section-title" style="margin-top:46px;">Professional experience</h2>
  <hr class="rule">
  <div class="timeline">
    {% for item in site.data.experience %}
      <div class="timeline-item">
        <div class="timeline-year">{{ item.years }}</div>
        <div class="timeline-title">{{ item.role }}</div>
        <div class="timeline-meta">{{ item.organization }}</div>
        {% if item.description %}<p>{{ item.description }}</p>{% endif %}
      </div>
    {% endfor %}
  </div>
</section>
