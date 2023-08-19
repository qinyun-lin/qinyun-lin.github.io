---
layout: page
permalink: /repositories/
title: GitHub Repositories
description: Here are some projects I've been contributing to
nav: false
nav_order: 99
---

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
