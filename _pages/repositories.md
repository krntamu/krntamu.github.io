---
layout: page
permalink: /repositories/
title: repositories
description: GitHub profile activity and selected open-source repositories.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
{% if site.data.repositories.github_users.size > 1 %}

  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.liquid username=user %}
  </div>

---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_repos %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}

{% if site.data.repositories.additional_repository_links and site.data.repositories.additional_repository_links.size > 0 %}

## More repositories

<ul class="post-list">
  {% for link in site.data.repositories.additional_repository_links %}
    <li>
      <a href="{{ link.url }}" target="_blank" rel="noopener noreferrer">{{ link.label }}</a>
    </li>
  {% endfor %}
</ul>

<p class="text-muted small mt-2">
  Stats and pin cards only support GitHub user accounts and public repositories (public API).
</p>
{% endif %}
