---
layout: archive
title: "Patents & Software Copyrights"
permalink: /intellectual-property/
author_profile: true
---

This page lists 8 granted invention patents and 14 software copyright records from a university system export dated August 30, 2026. Certificate scans and private application materials are not published. [中文版](/zh/intellectual-property/)

## Granted Invention Patents

{% assign patents = site.data.intellectual_property | where: "type", "patent" %}
{% for item in patents %}
- **{{ item.en_title }}**<br>
  Patent No. {{ item.number }} · Granted {{ item.date }}
{% endfor %}

## Software Copyrights

{% assign software = site.data.intellectual_property | where: "type", "software" %}
{% for item in software %}
- **{{ item.en_title }}**<br>
  Record No. {{ item.number }} · Approved {{ item.date }}
{% endfor %}
