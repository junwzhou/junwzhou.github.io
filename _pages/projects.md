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
    <p class="project-meta">{{ project.period }}{% if project.type_en %} · {{ project.type_en }}{% endif %}</p>
    <h2>{{ project.title_en }}</h2>
    {% if project.role_en or project.number or project.funding_en %}<p>{% if project.role_en %}<strong>{{ project.role_en }}</strong>{% endif %}{% if project.number %}{% if project.role_en %} · {% endif %}Project No. {{ project.number }}{% endif %}{% if project.funding_en %}{% if project.role_en or project.number %} · {% endif %}Funding: {{ project.funding_en }}{% endif %}</p>{% endif %}
  </article>
{% endfor %}
</div>
