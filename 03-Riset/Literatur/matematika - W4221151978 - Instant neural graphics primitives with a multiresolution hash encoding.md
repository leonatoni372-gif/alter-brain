---
tags: [literatur, matematika]
domain: matematika
tahun: 2022
sitasi: 3967
doi: 10.1145/3528223.3530127
core: "[[Core Ilmu]]"
status_baca: belum
---

# Instant neural graphics primitives with a multiresolution hash encoding

- **Penulis:** Thomas Müller, Alex Evans, Christoph Schied, Alexander Keller
- **Jurnal:** ACM Transactions on Graphics
- **Tahun:** 2022 | **Disitasi:** 3967x
- **Link:** https://doi.org/10.1145/3528223.3530127
- **Konsep:** Computer science, Hash function, Speedup, Rendering (computer graphics)
- **Core:** [[Core Ilmu]]

## Abstrak
Neural graphics primitives, parameterized by fully connected neural networks, can be costly to train and evaluate. We reduce this cost with a versatile new input encoding that permits the use of a smaller network without sacrificing quality, thus significantly reducing the number of floating point and memory access operations: a small neural network is augmented by a multiresolution hash table of trainable feature vectors whose values are optimized through stochastic gradient descent. The multiresolution structure allows the network to disambiguate hash collisions, making for a simple architecture that is trivial to parallelize on modern GPUs. We leverage this parallelism by implementing the whole system using fully-fused CUDA kernels with a focus on minimizing wasted bandwidth and compute operations. We achieve a combined speedup of several orders of magnitude, enabling training of high-quality neural graphics primitives in a matter of seconds, and rendering in tens of milliseconds at a resolution of 1920×1080.

## 💡 Insight-ku
-

## 🔗 Terkait
-
