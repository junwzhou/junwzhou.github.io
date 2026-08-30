---
title: "LogDLR: Unsupervised Cross-System Log Anomaly Detection Through Domain-Invariant Latent Representation"
collection: publications
permalink: /publication/2025-03-05-LogDLR-Unsupervised-Cross-System-Log-Anomaly-Detection-Through-Domain-Invariant-Latent-Representation
excerpt: 'In this paper, we propose LogDLR, a novel unsupervised cross-system log anomaly detection method. It uses universal sentence embeddings and a Transformer-based autoencoder to extract domain-invariant latent representations, adapts to heterogeneous log formats, captures semantic dependencies, and achieves efficient and accurate anomaly detection across different systems.'
date: 2025-03-05
venue: 'IEEE Transactions on Dependable and Secure Computing '
paperurl: 'https://doi.org/10.1109/TDSC.2025.3548050'
citation: 'J. Zhou et al., "LogDLR: Unsupervised Cross-System Log Anomaly Detection Through Domain-Invariant Latent Representation," in IEEE Transactions on Dependable and Secure Computing, vol. 22, no. 4, pp. 4456-4471, July-Aug. 2025, doi: 10.1109/TDSC.2025.3548050.
keywords: {Semantics;Anomaly detection;Feature extraction;Transformers;Data models;Training;Autoencoders;Syntactics;Vectors;Long short term memory;Anomaly detection;log analysis;adversarial training},'
---

## Abstract
Log anomaly detection aims to discover abnormal events from massive log data to ensure the security and reliability of software systems. However, due to the heterogeneity of log formats and syntaxes across different systems, existing log anomaly detection methods often need to be designed and trained for specific systems, lacking generalization ability. To address this challenge, we propose LogDLR, a novel unsupervised cross-system log anomaly detection method. The core idea of LogDLR is to use universal sentence embeddings and a Transformer-based autoencoder to extract domain-invariant latent representations from log entries, which can effectively adapt to log format changes and capture semantic information and dependencies in log sequences. To obtain domain-invariant latent representations, we adopt a domain-adversarial training strategy, introducing a domain discriminator that competes with the Transformer-based encoder through a gradient reversal layer, forcing the encoder to learn shared knowledge between different system logs. Finally, the Transformer-based decoder detects anomalies based on the domain-invariant representations obtained by the encoder. We evaluate LogDLR in simulated cross-system scenarios using three publicly available log datasets. The experimental results show that LogDLR can handle heterogeneous logs effectively in cross-system scenarios and achieve efficient and accurate anomaly detection on both source and target systems.

## Key words

Anomaly detection,log analysis,adversarial training

[Publisher page](https://doi.org/10.1109/TDSC.2025.3548050)

Recommended citation: J. Zhou et al., "LogDLR: Unsupervised Cross-System Log Anomaly Detection Through Domain-Invariant Latent Representation," in IEEE Transactions on Dependable and Secure Computing, vol. 22, no. 4, pp. 4456-4471, July-Aug. 2025, doi: 10.1109/TDSC.2025.3548050.
keywords: {Semantics;Anomaly detection;Feature extraction;Transformers;Data models;Training;Autoencoders;Syntactics;Vectors;Long short term memory;Anomaly detection;log analysis;adversarial training},


