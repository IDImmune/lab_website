---
title: Research
nav:
  order: 1
  tooltip: Current research
---

# {% include icon.html icon="fa-solid fa-wrench" %} Research Projects

<span style="font-size: 20px; line-height: 1.4; display: block; margin-bottom: 10px;">
Our work focuses on using cutting-edge techology to understand mechanisms of immune recognition.
</span>

{% include section.html %}

<div class="project-grid">
  {% for project in site.data.projects %}
    {% if project.group == "featured" %}
    <div class="project-card">
      <img src="{{ project.image }}" alt="{{ project.title }}">
      <div class="project-card-text">
        <h3>{{ project.title }}</h3>
        {% if project.subtitle %}
          <p class="subtitle">{{ project.subtitle }}</p>
        {% endif %}
        <p>{{ project.description }}</p>
      </div>
    </div>
    {% endif %}
  {% endfor %}
</div>

<style>
.project-grid {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  margin-top: 2rem;
}

.project-card {
  display: flex;
  gap: 1.5rem;
  background: #f9f9f9;
  padding: 1rem;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  align-items: flex-start;
}

.project-card img {
  width: 33.33%;      /* image takes one-third of card width */
  height: auto;
  object-fit: cover;
  border-radius: 8px;
  flex-shrink: 0;
}

.project-card-text {
  width: 66.66%;      /* text takes two-thirds */
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.project-card h3 {
  font-size: 1.25rem;
  margin: 0 0 0.25rem 0;
}

.project-card .subtitle {
  font-weight: 600;
  color: #666;
  margin: 0 0 0.5rem 0;
}

.project-card p {
  margin: 0;
}
</style>
