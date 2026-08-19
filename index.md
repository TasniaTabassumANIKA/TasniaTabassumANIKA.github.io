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

    <aside>
  <img class="profile-photo"
       src="{{ '/assets/img/profile.jpg' | relative_url }}"
       alt="Tasnia Tabassum Anika">

  <p><strong>Current focus</strong></p>
  <p class="small">
    Sustainable infrastructure, structural materials, urban environmental systems, and transportation environments, with an emphasis on GIS, spatiotemporal analysis, machine learning, environmental exposure, and data-driven prediction and optimization.
  </p>

  <p class="small">
    <a href="{{ site.author.scholar }}">Google Scholar</a> ·
    <a href="{{ site.author.orcid }}">ORCID</a>
  </p>
</aside>
  </div>
</section>

<section class="container">
  <div class="two-col">
    <div>
      <h2 class="section-title">Research profile</h2>
      <hr class="rule">
      <p>I am a civil engineering researcher and lecturer working at the intersection of **sustainable infrastructure, structural materials, urban environmental systems, transportation, and data-driven engineering**. My research focuses on improving infrastructure **sustainability, resilience, performance, and environmental outcomes** through experimental, spatial, environmental, and computational approaches. I am particularly interested in integrating **machine learning, explainable AI, GIS, and spatiotemporal modeling** to understand infrastructure–environment interactions and develop sustainable, resilient, and data-driven solutions for civil infrastructure.</p>
      <p>My current graduate research integrates field monitoring, statistical analysis, GIS, and explainable machine learning to study PM<sub>2.5</sub> exposure among Dhaka MRT Line-6 commuters.</p>
    </div>

    <div>
  <h2 class="section-title">Research Interests</h2>
  <hr class="rule">

  <div class="research-interest-groups">

    <div class="research-interest-group">
      <h3>Sustainable Infrastructure</h3>
      <div class="tag-wrap">
        <span class="tag">Sustainable &amp; Resilient Infrastructure</span>
        <span class="tag">Structural Materials &amp; Concrete Engineering</span>
        <span class="tag">Infrastructure Durability &amp; Performance</span>
        <span class="tag">Life-Cycle &amp; Environmental Assessment</span>
      </div>
    </div>

    <div class="research-interest-group">
      <h3>Urban Environmental Systems</h3>
      <div class="tag-wrap">
        <span class="tag">Urban Air Quality &amp; Environmental Modeling</span>
        <span class="tag">Environmental Exposure &amp; Health-Risk Assessment</span>
        <span class="tag">Urban Climate &amp; Infrastructure Interactions</span>
      </div>
    </div>

    <div class="research-interest-group">
      <h3>Transportation &amp; Mobility</h3>
      <div class="tag-wrap">
        <span class="tag">Transportation Infrastructure</span>
        <span class="tag">Sustainable Urban Mobility</span>
        <span class="tag">Transportation Environmental Impacts</span>
        <span class="tag">Traffic &amp; Transportation Modeling</span>
      </div>
    </div>

    <div class="research-interest-group">
      <h3>Data-Driven Civil Engineering</h3>
      <div class="tag-wrap">
        <span class="tag">Machine Learning &amp; Explainable AI</span>
        <span class="tag">GIS &amp; Spatial Analysis</span>
        <span class="tag">Spatiotemporal Modeling</span>
        <span class="tag">Data-Driven Prediction &amp; Optimization</span>
      </div>
    </div>

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
