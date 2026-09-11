---
layout: archive
title: "Results"
permalink: /intellectual-property/
author_profile: true
---

[中文版](/zh/intellectual-property/)

<span id="awards"></span>
## Awards

{% for item in site.data.awards %}
- **{{ item.title_en }}**<br>
  {{ item.category_en }} · {{ item.year }} · Contributor rank {{ item.rank_en }} · Certificate No. {{ item.number }}
{% endfor %}

<span id="patents"></span>
## Granted Invention Patents

{% assign patents = site.data.intellectual_property | where: "type", "patent" %}
{% for item in patents %}
- **{{ item.en_title }}**<br>
  Patent No. {{ item.number }} · Granted {{ item.date }}
{% endfor %}

<span id="software"></span>
## Software Copyrights

{% assign software = site.data.intellectual_property | where: "type", "software" %}
{% for item in software %}
- **{{ item.en_title }}**<br>
  Record No. {{ item.number }} · Approved {{ item.date }}
{% endfor %}
