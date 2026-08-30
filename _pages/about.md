---
permalink: /
title: "Junwei Zhou"
excerpt: "Professor and Doctoral Supervisor | System & Software Security"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="research-hero">
  <p class="eyebrow"><a href="https://www.whut.edu.cn/">Wuhan University of Technology</a></p>
  <h1>Junwei Zhou <span>周俊伟</span></h1>
  <p class="hero-role">Professor · Doctoral Supervisor · Deputy Dean</p>
  <p class="hero-summary"><a href="https://csai.whut.edu.cn/">School of Artificial Intelligence</a></p>
  <div class="hero-actions">
    <a class="button button--primary" href="/publications/">Selected publications</a>
    <a class="button button--outline" href="/zh/">中文主页</a>
  </div>
</div>

## About

I am a Professor and Doctoral Supervisor at the [School of Artificial Intelligence](https://csai.whut.edu.cn/), [Wuhan University of Technology](https://www.whut.edu.cn/), where I currently serve as Deputy Dean. My research focuses on AI for system and software security, coding, compression, and vision.

## Research Areas

<div class="research-grid">
  <div class="research-card"><strong>AI for System &amp; Software Security</strong><span>Intelligent log analysis, industrial control security, data security, vulnerability analysis, fault diagnosis, and dependable software systems.</span></div>
  <div class="research-card"><strong>AI for Coding and Vision</strong><span>AI coding, AI compression, image and video compression, visual recognition, and privacy-aware visual intelligence.</span></div>
</div>

## Selected Publications

- **LogDLR: Unsupervised Cross-System Log Anomaly Detection Through Domain-Invariant Latent Representation.** *IEEE Transactions on Dependable and Secure Computing*, 2025. [DOI](https://doi.org/10.1109/TDSC.2025.3548050)
- **DeepSyslog: Deep Anomaly Detection on Syslog Using Sentence Embedding and Metadata.** *IEEE Transactions on Information Forensics and Security*, 2022. [DOI](https://doi.org/10.1109/TIFS.2022.3201379)
- **Poster: GLog: Self-Evolving Log Anomaly Type Prediction via Instruction-Tuned LLM and Clustering.** *ACM CCS*, 2025. [DOI](https://doi.org/10.1145/3719027.3760727)

[View all listed publications →](/publications/)

## Current Research Projects

- Multimodal embodied intelligence through tactile-visual fusion (2025–2027), Principal Investigator.
- Intelligent fault localization and analysis based on system runtime logs (2026–2027), Principal Investigator.
- Artificial intelligence and factor-based quantitative trading systems (2026–2028), Principal Investigator.

## Latest News

{% assign news_items = site.news | sort: "order" %}
<div class="news-list">
{% for item in news_items limit:3 %}
  <article class="news-item">
    <p class="news-meta">{{ item.category_en }}</p>
    <h3><a href="{{ item.url }}">{{ item.title_en }}</a></h3>
    <p>{{ item.summary_en }}</p>
  </article>
{% endfor %}
</div>

[All news →](/news/)

## Join the Team

We welcome motivated doctoral and master's students interested in system security, software reliability, intelligent log analysis, and industrial control system security. For academic enquiries, please contact [junweizhou@whut.edu.cn](mailto:junweizhou@whut.edu.cn).
