---
layout: page
permalink: /repositories/
title: repositories
description: GitHub profile statistics and selected repositories.
nav: true
nav_order: 6
---

{% if site.repository_page.show_user_stats and site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

---

{% if site.repository_page.show_trophies and site.repo_trophies.enabled %}
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

{% assign public_starred_repos = site.data.github_public_repos | where_exp: "repo", "repo.private != true and repo.stargazers_count >= 1" | sort: "stargazers_count" | reverse %}
{% assign fallback_repos = site.data.repositories.github_repos %}

{% if public_starred_repos and public_starred_repos.size > 0 %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in public_starred_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% elsif fallback_repos %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in fallback_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
