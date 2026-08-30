---
layout: archive
title: "专利与软件著作权"
permalink: /zh/intellectual-property/
author_profile: true
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a><a href="/zh/publications/">论文</a><a href="/zh/projects/">项目</a><a href="/zh/intellectual-property/">专利与软著</a><a href="/zh/team/">团队</a><a href="/zh/news/">新闻</a><a href="/intellectual-property/">EN</a>
</nav>

本页依据2026年8月30日校内系统导出清单，列出8项授权发明专利和14项软件著作权。证书扫描件及申请材料不予公开。

## 授权发明专利

{% assign patents = site.data.intellectual_property | where: "type", "patent" %}
{% for item in patents %}
- **{{ item.zh_title }}**<br>
  专利号：{{ item.number }} · 授权日期：{{ item.date }}
{% endfor %}

## 软件著作权

{% assign software = site.data.intellectual_property | where: "type", "software" %}
{% for item in software %}
- **{{ item.zh_title }}**<br>
  编号：{{ item.number }} · 获批日期：{{ item.date }}
{% endfor %}
