---
layout: archive
title: "论文发表"
permalink: /zh/publications/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/projects/">项目</a><a href="/zh/intellectual-property/">专利与软著</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/publications/">EN</a>
</nav>

{% assign current_year = "" %}
<div class="publication-list">
{% for pub in site.data.publications %}
  {% if pub.year != current_year %}
    {% unless current_year == "" %}</section>{% endunless %}
    <section class="publication-year">
    <h2>{{ pub.year }}年</h2>
    {% assign current_year = pub.year %}
  {% endif %}
  <article class="publication-entry">
    <h3>{{ pub.title }}</h3>
    <p class="publication-authors">{{ pub.authors }}</p>
    <p class="publication-venue">{{ pub.venue }}</p>
  </article>
{% endfor %}
{% unless current_year == "" %}</section>{% endunless %}
</div>
