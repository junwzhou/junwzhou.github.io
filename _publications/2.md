---
title: "Poster: GLog: Self-Evolving Log Anomaly Type Prediction via Instruction-Tuned LLM and Clustering"
collection: publications
permalink: /publication/2025-11-22-GLog-Self-Evolving-Log-Anomaly-Type-Prediction-via-Instruction-Tuned-LLM-and-Clustering
excerpt: 'In this paper, we propose GLog, an end-to-end self-evolving log anomaly prediction framework. It fine-tunes instruction-tuned LLMs to achieve high-accuracy anomaly detection on raw unparsed logs, clusters anomalies for automatic pseudo label generation, and supports continuous self-evolving model optimization, which greatly reduces manual annotation cost and adapts to evolving system behaviors.'
date: 2025-11-22
venue: 'Proceedings of the 2025 ACM SIGSAC Conference on Computer and Communications Security'
paperurl: 'https://dl.acm.org/doi/10.1145/3719027.3760727'
citation: 'JunWei Zhou, Yuyang Gao, Cheng Tan, Yanchao Yang, and Jianwen Xiang. 2025. Poster: GLog: Self-Evolving Log Anomaly Type Prediction via Instruction-Tuned LLM and Clustering. In Proceedings of the 2025 ACM SIGSAC Conference on Computer and Communications Security (CCS 25). Association for Computing Machinery, New York, NY, USA, 4791–4793.'
keywords: 'Log anomaly detection; Self-evolving prediction; Instruction-tuned LLM; Log clustering; Anomaly type classification'
---

## Abstract
Log anomaly detection is critical for maintaining system reliability and observability in complex cloud and microservice environments. However, existing methods often remain limited to binary classification, struggle to adapt to dynamic log patterns, and suffer from semantic loss due to log parsing. To address these challenges, we propose GLog, an end-to-end framework that enables dynamic anomaly type prediction without requiring manual type labels. GLog first fine-tunes instruction-tuned large language models using normal/abnormal labels to achieve high-accuracy anomaly detection on raw, unparsed log sequences. It then clusters the detected anomalies to automatically generate pseudo anomaly type labels and descriptions, which are further used for second-stage fine-tuning, enabling the model to predict specific anomaly types with interpretable outputs. By leveraging full log semantics and dynamically updating its anomaly type repository, GLog reduces manual annotation costs and adapts to evolving system behaviors in large-scale environments.

## Key words
Log anomaly type prediction; self-evolving model; instruction-tuned LLM; log clustering; log semantic understanding

[Download paper here](https://dl.acm.org/doi/pdf/10.1145/3719027.3760727)

Recommended citation: JunWei Zhou, Yuyang Gao, Cheng Tan, Yanchao Yang, and Jianwen Xiang. 2025. Poster: GLog: Self-Evolving Log Anomaly Type Prediction via Instruction-Tuned LLM and Clustering. In Proceedings of the 2025 ACM SIGSAC Conference on Computer and Communications Security (CCS '25). Association for Computing Machinery, New York, NY, USA, 4791–4793. https://doi.org/10.1145/3719027.3760727
