---
layout: archive
title: "周俊伟"
permalink: /zh/
author_profile: true
redirect_from:
  - /chinese/
---

<nav class="language-nav" aria-label="中文页面导航">
  <a href="/zh/">首页</a>
  <a href="/zh/publications/">论文</a>
  <a href="/zh/team/">团队</a>
  <a href="/zh/news/">新闻</a>
  <a href="/">EN</a>
</nav>

<div class="research-hero">
  <p class="eyebrow"><a href="https://www.whut.edu.cn/">武汉理工大学</a></p>
  <h1>周俊伟 <span>Junwei Zhou</span></h1>
  <p class="hero-role">教授 · 博士生导师 · 副院长</p>
  <p class="hero-summary"><a href="https://csai.whut.edu.cn/">人工智能学院</a></p>
  <div class="hero-actions">
    <a class="button button--primary" href="/zh/publications/">代表性论文</a>
    <a class="button button--outline" href="/">English</a>
  </div>
</div>

## 个人简介

周俊伟，[武汉理工大学](https://www.whut.edu.cn/)[人工智能学院](https://csai.whut.edu.cn/)教授、博士生导师，现任学院副院长。主要从事系统与软件安全、编码与压缩、计算机视觉、系统日志异常检测与根因分析、工业控制系统安全、数据安全等方面的研究。

## 研究方向

<div class="research-grid">
  <div class="research-card"><strong>系统与软件安全</strong><span>软件监控、故障容错、漏洞分析与可信软件系统。</span></div>
  <div class="research-card"><strong>日志智能分析</strong><span>日志异常检测、跨系统迁移与根因分析。</span></div>
  <div class="research-card"><strong>工业控制系统安全</strong><span>工业协议解析、安全测试与威胁诊断。</span></div>
  <div class="research-card"><strong>数据安全</strong><span>隐私保护计算与安全数据处理。</span></div>
  <div class="research-card"><strong>编码与压缩</strong><span>分布式信源编码、图像与视频压缩、压缩与加密联合设计。</span></div>
  <div class="research-card"><strong>计算机视觉</strong><span>视觉识别、人脸特征点定位与隐私保护视觉智能。</span></div>
</div>

## 代表性论文

- **LogDLR: Unsupervised Cross-System Log Anomaly Detection Through Domain-Invariant Latent Representation.** *IEEE Transactions on Dependable and Secure Computing*, 2025。[DOI](https://doi.org/10.1109/TDSC.2025.3548050)
- **DeepSyslog: Deep Anomaly Detection on Syslog Using Sentence Embedding and Metadata.** *IEEE Transactions on Information Forensics and Security*, 2022。[DOI](https://doi.org/10.1109/TIFS.2022.3201379)
- **Poster: GLog: Self-Evolving Log Anomaly Type Prediction via Instruction-Tuned LLM and Clustering.** *ACM CCS*, 2025。[DOI](https://doi.org/10.1145/3719027.3760727)

[查看论文列表 →](/zh/publications/)

## 在研项目

- 面向复杂场景的触觉—视觉多模态融合具身智能关键技术（2025—2027），主持。
- 基于系统运行日志的智能故障定位与分析关键技术研究（2026—2027），主持。
- 人工智能与因子量化交易系统与策略研发（2026—2028），主持。

## 最新消息

{% assign news_items = site.news | sort: "order" %}
<div class="news-list">
{% for item in news_items limit:3 %}
  <article class="news-item">
    <p class="news-meta">{{ item.category_zh }}</p>
    <h3><a href="{{ item.url }}#zh">{{ item.title_zh }}</a></h3>
    <p>{{ item.summary_zh }}</p>
  </article>
{% endfor %}
</div>

[查看全部新闻 →](/zh/news/)

## 招生与合作

欢迎对系统安全、软件可靠性、日志智能分析和工业控制系统安全感兴趣的博士生、硕士生联系。学术交流请发送邮件至 [junweizhou@whut.edu.cn](mailto:junweizhou@whut.edu.cn)。
