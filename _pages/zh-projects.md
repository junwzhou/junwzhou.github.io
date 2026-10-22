---
layout: archive
title: "科研项目"
permalink: /zh/projects/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/projects/">项目</a><a href="/zh/intellectual-property/">成果</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/projects/">EN</a>
</nav>

<div class="project-list">
{% for project in site.data.projects %}
  <article class="project-entry">
    <p class="project-meta">{{ project.period }}{% if project.type_zh %} · {{ project.type_zh }}{% endif %}</p>
    <h2>{{ project.title_zh }}</h2>
    {% if project.role_zh or project.number %}<p>{% if project.role_zh %}<strong>{{ project.role_zh }}</strong>{% endif %}{% if project.number %}{% if project.role_zh %} · {% endif %}项目编号 {{ project.number }}{% endif %}</p>{% endif %}
  </article>
{% endfor %}
</div>
