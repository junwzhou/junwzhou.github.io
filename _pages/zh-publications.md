---
layout: archive
title: "论文发表"
permalink: /zh/publications/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/publications/">EN</a>
</nav>

本列表由本人提供的 Google Scholar 导出文件整理，已排除预印本、委员会条目、明显的同名作者误收结果，以及明确发表于完全开放获取期刊的论文。仅在导出信息能够明确识别出版来源时规范化来源名称。

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
