---
layout: default
title: Experiences
nav_order: 3
has_children: true
permalink: /experiences/
---

# Experiences

A chronicle of my research experiences and international collaborations.

{% assign sorted_experiences = site._experiences | sort: "nav_order" %}
{% for experience in sorted_experiences %}
<div class="experience-card">
  <h2><a href="{{ experience.url | relative_url }}">{{ experience.title }}</a></h2>
  {% if experience.image %}
  <img src="{{ experience.image | relative_url }}" alt="{{ experience.title }}" class="experience-image">
  {% endif %}
  <p>{{ experience.description }}</p>
</div>
{% endfor %}

<style>
.experience-card {
    border: 1px solid #e1e4e8;
    border-radius: 6px;
    padding: 16px;
    margin-bottom: 16px;
}

.experience-image {
    max-width: 100%;
    height: auto;
    margin: 10px 0;
    border-radius: 4px;
}
</style>
