---
layout: default
title: Updates
permalink: /updates/
---
<div class="page-head">
  <div class="container">
    <h1>Updates</h1>
    <p>A lightweight academic news page for publications, conferences, research milestones, and professional activities.</p>
  </div>
</div>
<section class="container">
  {% for update in site.data.updates %}
    <article class="pub">
      <div class="pub-title">{{ update.title }}</div>
      <div class="pub-meta">{{ update.date }}</div>
      <p>{{ update.text }}</p>
    </article>
  {% endfor %}
</section>
