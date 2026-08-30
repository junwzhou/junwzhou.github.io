---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

[中文列表](/zh/publications/)

{% if author.googlescholar %}
You can also find the latest citation information on <a href="{{ author.googlescholar }}">Google Scholar</a>.
{% endif %}

{% assign current_year = "" %}
<div class="publication-list">
{% for pub in site.data.publications %}
  {% if pub.year != current_year %}
    {% unless current_year == "" %}</section>{% endunless %}
    <section class="publication-year">
    <h2>{{ pub.year }}</h2>
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
