---
layout: archive
title: "新闻动态"
permalink: /zh/news/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/projects/">项目</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/news/">EN</a>
</nav>

团队活动与科研动态。尚未核实的活动日期统一标记为“日期待确认”。

{% assign news_items = site.news | sort: "order" %}
<div class="news-grid">
{% for item in news_items %}
  <article class="news-card">
    {% if item.image %}<a href="{{ item.url }}#zh"><img src="{{ item.image }}" alt="{{ item.image_alt_zh }}" loading="lazy"></a>{% endif %}
    <div class="news-card__body">
      <p class="news-meta">{{ item.category_zh }} · {{ item.date_zh }}</p>
      <h2><a href="{{ item.url }}#zh">{{ item.title_zh }}</a></h2>
      <p>{{ item.summary_zh }}</p>
    </div>
  </article>
{% endfor %}
</div>
