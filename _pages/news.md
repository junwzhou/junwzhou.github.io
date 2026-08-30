---
layout: archive
title: "News"
permalink: /news/
author_profile: true
---

Team activities and research updates. Dates are shown only after they have been confirmed. [中文新闻](/zh/news/)

{% assign news_items = site.news | sort: "order" %}
<div class="news-grid">
{% for item in news_items %}
  <article class="news-card">
    {% if item.image %}<a href="{{ item.url }}"><img src="{{ item.image }}" alt="{{ item.image_alt_en }}" loading="lazy"></a>{% endif %}
    <div class="news-card__body">
      <p class="news-meta">{{ item.category_en }} · {{ item.date_en }}</p>
      <h2><a href="{{ item.url }}">{{ item.title_en }}</a></h2>
      <p>{{ item.summary_en }}</p>
    </div>
  </article>
{% endfor %}
</div>
