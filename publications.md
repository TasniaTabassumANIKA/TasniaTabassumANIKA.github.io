---
layout: default
title: Publications
permalink: /publications/
---
<div class="page-head">
  <div class="container">
    <h1>Publications</h1>
    <p>Selected peer-reviewed conference publications and manuscripts currently under review.</p>
  </div>
</div>

<section class="container">
  {% assign published = site.data.publications | where: "status", "Published" %}
  {% for pub in published %}
    <article class="pub">
      <div class="pub-title">{{ pub.title }}</div>
      <div class="pub-meta">{{ pub.authors }} ({{ pub.year }}). <em>{{ pub.venue }}</em>.</div>
      {% if pub.details %}<div class="pub-meta">{{ pub.details }}</div>{% endif %}
      {% if pub.link %}<div class="pub-actions"><a href="{{ pub.link }}">DOI / Publication link →</a></div>{% endif %}
    </article>
  {% endfor %}

  <h2 class="section-title" style="margin-top:48px;">Manuscripts under review</h2>
  <hr class="rule">
  {% assign review = site.data.publications | where: "status", "Under review" %}
  {% for pub in review %}
    <article class="pub">
      <div class="pub-title">{{ pub.title }} <span class="badge">Under review</span></div>
      <div class="pub-meta">{{ pub.authors }}</div>
      {% if pub.venue %}<div class="pub-meta">{{ pub.venue }}</div>{% endif %}
    </article>
  {% endfor %}
</section>
