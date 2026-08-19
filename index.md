---
layout: default
title: Home
---

<section class="hero">
  <div class="hero-grid">
    <div>
      <div class="kicker">Civil Engineering · Research · Data-Driven Infrastructure</div>
      <h1>Tasnia Tabassum Anika</h1>
      <h2>Lecturer, Department of Civil Engineering, Dhaka International University</h2>
      <p class="lead">Civil engineering researcher working at the intersection of sustainable infrastructure, urban environmental systems, and data-driven modeling. My work spans sustainable construction materials, AI-based concrete strength prediction, urban transportation environments, PM<sub>2.5</sub> exposure assessment, GIS, spatial analysis, health-risk assessment, and explainable machine learning.</p>
      <div class="hero-actions">
        <a class="button" href="{{ '/research/' | relative_url }}">Explore Research</a>
        <a class="button secondary" href="{{ '/publications/' | relative_url }}">View Publications</a>
        <a class="button secondary" href="{{ '/cv/' | relative_url }}">Academic CV</a>
      </div>
    </div>

    <aside
      <img class="profile-photo"
      src="{{ '/assets/img/profile.jpg' | relative_url }}"
      alt="Tasnia Tabassum Anika">
      <p><strong>Current focus</strong></p>
      <p class="small">Infrastructure–urban climate interactions, sustainable materials, spatial and spatiotemporal analysis, machine learning, and environmental exposure.</p>
      <p class="small"><a href="{{ site.author.scholar }}">Google Scholar</a> · <a href="{{ site.author.orcid }}">ORCID</a></p>
    </aside>
  </div>
</section>

<section class="container">
  <div class="two-col">
    <div>
      <h2 class="section-title">Research profile</h2>
      <hr class="rule">
      <p>I am particularly interested in understanding how infrastructure characteristics and urban context interact to shape local environmental conditions, human exposure, and climate-related impacts. I aim to develop spatial, computational, and data-driven approaches for understanding infrastructure–environment interactions and supporting sustainable, climate-responsive urban infrastructure.</p>
      <p>My current graduate research integrates field monitoring, statistical analysis, GIS, and explainable machine learning to study PM<sub>2.5</sub> exposure among Dhaka MRT Line-6 commuters.</p>
    </div>

    <div>
      <h2 class="section-title">Research interests</h2>
      <hr class="rule">
      <div class="tag-wrap">
        <span class="tag">Infrastructure–Urban Climate Interactions</span>
        <span class="tag">Urban Environmental Modeling</span>
        <span class="tag">Spatiotemporal &amp; Life-Cycle Analysis</span>
        <span class="tag">Machine Learning &amp; Explainable AI</span>
        <span class="tag">Sustainable &amp; Climate-Responsive Infrastructure</span>
        <span class="tag">Environmental Exposure &amp; Risk Assessment</span>
      </div>
    </div>
  </div>
</section>

<section class="container" style="padding-top:10px;">
  <h2 class="section-title">Selected research</h2>
  <p class="section-subtitle">A small set of projects that represent my current and previous research trajectory.</p>
  <div class="card-grid">
    {% for project in site.data.projects limit:4 %}
      <article class="card">
        <h3>{{ project.title }}</h3>
        <p>{{ project.summary }}</p>
        <div class="tag-wrap">
          {% for tag in project.tags limit:3 %}<span class="tag">{{ tag }}</span>{% endfor %}
        </div>
      </article>
    {% endfor %}
  </div>
</section>

<section class="container" style="padding-top:10px;">
  <div class="two-col">
    <div>
      <h2 class="section-title">Education</h2>
      <hr class="rule">
      {% for item in site.data.education limit:3 %}
        <div style="margin-bottom:18px;">
          <strong>{{ item.degree }}</strong><br>
          <span>{{ item.institution }}</span><br>
          <span class="small">{{ item.years }}{% if item.detail %} · {{ item.detail }}{% endif %}</span>
        </div>
      {% endfor %}
    </div>
    <div>
      <h2 class="section-title">Latest updates</h2>
      <hr class="rule">
      {% for update in site.data.updates limit:3 %}
        <div style="margin-bottom:18px;">
          <strong>{{ update.title }}</strong><br>
          <span class="small">{{ update.date }}</span>
          <p class="small">{{ update.text }}</p>
        </div>
      {% endfor %}
    </div>
  </div>
</section>
