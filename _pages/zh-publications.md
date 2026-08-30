---
layout: archive
title: "论文发表"
permalink: /zh/publications/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/publications/">EN</a>
</nav>

本页列出已经核验基本书目信息的代表性论文。论文题目保持原文，DOI链接指向出版社页面。

{% include base_path %}
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
