---
layout: default
title: Projects
nav_order: 2
has_children: true
permalink: /projects/
---

# Projects

A collection of my research projects and technical work in particle physics and machine learning.

{% assign sorted_projects = site._projects | sort: "nav_order" %}
{% for project in sorted_projects %}
<div class="project-card">
  <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
  {% if project.image %}
  <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
  {% endif %}
  <p>{{ project.description }}</p>
</div>
{% endfor %}

<style>
.project-card {
    border: 1px solid #e1e4e8;
    border-radius: 6px;
    padding: 16px;
    margin-bottom: 16px;
}

.project-image {
    max-width: 100%;
    height: auto;
    margin: 10px 0;
    border-radius: 4px;
}
</style>
