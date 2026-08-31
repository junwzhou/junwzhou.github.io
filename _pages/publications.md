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
    <p class="publication-links">
      {% if pub.doi != "" %}<a href="https://doi.org/{{ pub.doi }}" target="_blank" rel="noopener">DOI</a>{% endif %}
      {% assign doi_url = "https://doi.org/" | append: pub.doi %}
      {% if pub.publisher_url != "" and pub.publisher_url != doi_url %}<a href="{{ pub.publisher_url }}" target="_blank" rel="noopener">Publisher</a>{% endif %}
      {% if pub.full_text_url != "" %}<a href="{{ pub.full_text_url }}" target="_blank" rel="noopener">Full text</a>{% endif %}
    </p>
  </article>
{% endfor %}
{% unless current_year == "" %}</section>{% endunless %}
</div>
