---
layout: page
permalink: /repositories/
title: Resources
description: Selected research code, course repositories, and project resources.
nav: true
nav_order: 4
---

This page collects selected code repositories, course materials, and project resources connected to my research and teaching.

{% if site.data.repositories.github_repos %}

## Research Code

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>

{% endif %}

{% if site.data.repositories.course_repositories and site.data.repositories.course_repositories.size > 0 %}

## Teaching Materials

<ul class="post-list">
  {% for link in site.data.repositories.course_repositories %}
    <li>
      <a href="{{ link.url }}" target="_blank" rel="noopener noreferrer">{{ link.label }}</a>
      {% if link.description %}
        <br>
        <span class="text-muted small">{{ link.description }}</span>
      {% endif %}
    </li>
  {% endfor %}
</ul>

{% endif %}

{% if site.data.repositories.additional_repository_links and site.data.repositories.additional_repository_links.size > 0 %}

## Organizations and Additional Resources

<ul class="post-list">
  {% for link in site.data.repositories.additional_repository_links %}
    <li>
      <a href="{{ link.url }}" target="_blank" rel="noopener noreferrer">{{ link.label }}</a>
      {% if link.description %}
        <br>
        <span class="text-muted small">{{ link.description }}</span>
      {% endif %}
    </li>
  {% endfor %}
</ul>

{% endif %}
