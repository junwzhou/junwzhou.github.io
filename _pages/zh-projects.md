---
layout: archive
title: "科研项目"
permalink: /zh/projects/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/projects/">项目</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/projects/">EN</a>
</nav>

<div class="project-list">
{% for project in site.data.projects %}
  <article class="project-entry">
    <p class="project-meta">{{ project.period }} · {{ project.type_zh }}</p>
    <h2>{{ project.title_zh }}</h2>
    <p><strong>{{ project.role_zh }}</strong>{% if project.number %} · 项目编号 {{ project.number }}{% endif %}</p>
  </article>
{% endfor %}
</div>
