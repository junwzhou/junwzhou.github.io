---
title: "DeepSyslog: Deep Anomaly Detection on Syslog Using Sentence Embedding and Metadata"
collection: publications
permalink: /publication/2022-08-20-DeepSyslog-Deep-Anomaly-Detection-on-Syslog-Using-Sentence-Embedding-and-Metadata
excerpt: 'In this paper, we propose DeepSyslog, a deep anomaly detection method for Syslog that integrates unsupervised sentence embedding with event metadata to capture contextual semantics and improve detection accuracy, outperforming existing log-based approaches.'
date: 2022-08-20
venue: 'IEEE Transactions on Information Forensics and Security'
paperurl: 'https://ieeexplore.ieee.org/document/9865986'
citation: 'J. Zhou, Y. Qian, Q. Zou, P. Liu and J. Xiang, "DeepSyslog: Deep Anomaly Detection on Syslog Using Sentence Embedding and Metadata," in IEEE Transactions on Information Forensics and Security, vol. 17, pp. 3051-3061, 2022, doi: 10.1109/TIFS.2022.3201379.
keywords: {Metadata;Anomaly detection;Feature extraction;Semantics;Indexes;History;Event detection;Anomaly detection;sentence embedding;event metadata},'
---

## Abstract
Anomaly events indicating the unhealthy status of the computer system are recorded in the system log (Syslog). Therefore, Syslog-based anomaly event detection is crucial for diagnosing system issues and problems. However, existing log-based anomaly detection approaches use raw and unstructured log entries independently and incompletely, i.e., without considering the context of each event and event metadata in the logs. They employ incomplete representation of unstructured log data, limiting the deep learning model’s capacity in the early stage, which tends to omit anomaly events and cause false alarms. In this work, we propose DeepSyslog, which represents Syslog with the context of log events and event metadata in the logs. Inspired by the sequence nature of the log stream, we employ unsupervised sentence embedding to extract the semantic and context information hidden in the log stream, rather than word embedding or one-hot embedding, which only capture the similarities between log words. The sentence embedding is further integrated with event metadata to form complete representations of Syslog, which can distinguish the anomaly caused by the correlated log entries and exceptional event metadata in the log. The simulation results on widely used log datasets show that DeepSyslog achieves high performance compared with the existing log-based anomaly event detection approaches.

## Key words

Metadata;Anomaly detection;Feature extraction;Semantics;Indexes;History;Event detection

[Download paper here](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9865986)

Recommended citation: J. Zhou, Y. Qian, Q. Zou, P. Liu and J. Xiang, "DeepSyslog: Deep Anomaly Detection on Syslog Using Sentence Embedding and Metadata," in IEEE Transactions on Information Forensics and Security, vol. 17, pp. 3051-3061, 2022, doi: 10.1109/TIFS.2022.3201379.
keywords: {Metadata;Anomaly detection;Feature extraction;Semantics;Indexes;History;Event detection;Anomaly detection;sentence embedding;event metadata},

<!-- Recommended citation（in Chinese）: 陈蔚燕, 张扶桑, 刘俊杰, 包鹏, 张大庆. 基于IR-UWB雷达的多视角融合动态目标追踪. 软件学报, 2023, 34(12):
5457–5476. http://www.jos.org.cn/1000-9825/6760.htm -->
