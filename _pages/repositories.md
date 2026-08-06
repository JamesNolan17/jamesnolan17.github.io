---
layout: page
permalink: /repositories/
title: repositories
description: Selected code and paper replication packages. The full list lives on my <a href="https://github.com/JamesNolan17" target="_blank" rel="noopener noreferrer">GitHub profile</a>.
nav: true
nav_order: 4
---

<p>
  <a href="https://github.com/JamesNolan17" target="_blank" rel="noopener noreferrer">
    <img alt="GitHub followers" src="https://img.shields.io/github/followers/JamesNolan17?style=social">
  </a>
</p>

<div class="row row-cols-1 row-cols-md-2 g-4 my-2">

  {% assign repos = site.data.repositories.github_repos %}
  {% for repo in repos %}
  <div class="col">
    <div class="card h-100">
      <div class="card-body">
        <h5 class="card-title mb-1">
          <a href="https://github.com/{{ repo.name }}" target="_blank" rel="noopener noreferrer">{{ repo.title }}</a>
        </h5>
        <p class="card-text mb-2">{{ repo.description }}</p>
        <img alt="stars" src="https://img.shields.io/github/stars/{{ repo.name }}?style=flat&label=%E2%98%85">
        <img alt="language" src="https://img.shields.io/github/languages/top/{{ repo.name }}">
        <img alt="last commit" src="https://img.shields.io/github/last-commit/{{ repo.name }}?display_timestamp=author">
      </div>
    </div>
  </div>
  {% endfor %}

</div>
