---
layout: archive
title: "成果"
permalink: /zh/intellectual-property/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/projects/">项目</a><a href="/zh/intellectual-property/">成果</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/intellectual-property/">EN</a>
</nav>

<span id="awards"></span>
## 获奖

{% for item in site.data.awards %}
- **{{ item.title_zh }}**<br>
  {{ item.category_zh }} · {{ item.year }}年 · 本人排名{{ item.rank_zh }} · 证书编号{{ item.number }}
{% endfor %}

<span id="patents"></span>
## 授权发明专利

{% assign patents = site.data.intellectual_property | where: "type", "patent" %}
{% for item in patents %}
- **{{ item.zh_title }}**<br>
  专利号：{{ item.number }} · 授权日期：{{ item.date }}
{% endfor %}

<span id="software"></span>
## 软件著作权

{% assign software = site.data.intellectual_property | where: "type", "software" %}
{% for item in software %}
- **{{ item.zh_title }}**<br>
  编号：{{ item.number }} · 获批日期：{{ item.date }}
{% endfor %}
