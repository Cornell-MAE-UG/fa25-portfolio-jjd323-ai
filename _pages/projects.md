---
layout: default
title: Joseph D'Arcangelo - Portfolio
permalink: /projects/
---

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          
          <p class="project-title">{{ project.title }}</p>
          <p>{{ project.description | default: "NO DESCRIPTION FOUND" }}</p>
          
        </a>
      </div>
    {% endfor %}
  </div>
</div>
<style>
.project-title {
  font-weight: bold;
  margin: 10px 0 5px 0;
}

.project-description {
  font-size: 0.9rem;
  color: #555;
  margin: 0;
}
</style>