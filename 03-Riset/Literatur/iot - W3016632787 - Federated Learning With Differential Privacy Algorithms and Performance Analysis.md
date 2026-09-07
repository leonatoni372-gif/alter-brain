---
tags: [literatur, iot]
domain: iot
tahun: 2020
sitasi: 2362
doi: 10.1109/tifs.2020.2988575
core: "[[Core Ilmu]]"
status_baca: belum
---

# Federated Learning With Differential Privacy: Algorithms and Performance Analysis

- **Penulis:** Kang Wei, Jun Li, Ming Ding, Chuan Ma
- **Jurnal:** IEEE Transactions on Information Forensics and Security
- **Tahun:** 2020 | **Disitasi:** 2362x
- **Link:** https://doi.org/10.1109/tifs.2020.2988575
- **Konsep:** Computer science, Differential privacy, Algorithm, Theoretical computer science
- **Core:** [[Core Ilmu]]

## Abstrak
Federated learning (FL), as a type of distributed machine learning, is capable of significantly preserving clients’ private data from being exposed to adversaries. Nevertheless, private information can still be divulged by analyzing uploaded parameters from clients, e.g., weights trained in deep neural networks. In this paper, to effectively prevent information leakage, we propose a novel framework based on the concept of differential privacy (DP), in which artificial noise is added to parameters at the clients’ side before aggregating, namely, noising before model aggregation FL (NbAFL). First, we prove that the NbAFL can satisfy DP under distinct protection levels by properly adapting different variances of artificial noise. Then we develop a theoretical convergence bound on the loss function of the trained FL model in the NbAFL. Specifically, the theoretical bound reveals the following three key properties: 1) there is a tradeoff between convergence performance and privacy protection levels, i.e., better convergence performance leads to a lower protection level; 2) given a fixed privacy protection level, increasing the number$N$of overall clients participating in FL can improve the convergence performance; and 3) there is an optimal number aggregation times (communication rounds) in terms of convergence performance for a given protection level. Furthermore, we propose a$K$-client random scheduling strategy, where$K$($1\leq K< N$) clients are randomly selected from the$N$overall clients to participate in each aggregation. We also develop a corresponding convergence bound for the loss function in this case and the$K$-client random scheduling strategy also retains the above three properties. Moreover, we find that there is an optimal$K$that achieves the best convergence performance at a fixed privacy level. Evaluations demonstrate that our theoretical results are consistent with simulations, thereby facilitating the design of various privacy-preserving FL algorithms with different tradeoff requirements on convergence performance and privacy levels.

## Insight-ku
-

## Terkait
-
