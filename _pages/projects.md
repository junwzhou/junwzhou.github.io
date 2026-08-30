---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /cv/
  - /resume
---

[中文项目列表](/zh/projects/)

<div class="project-list">
{% for project in site.data.projects %}
  <article class="project-entry">
    <p class="project-meta">{{ project.period }} · {{ project.type_en }}</p>
    <h2>{{ project.title_en }}</h2>
    <p><strong>{{ project.role_en }}</strong>{% if project.number %} · Project No. {{ project.number }}{% endif %}</p>
  </article>
{% endfor %}
</div>
