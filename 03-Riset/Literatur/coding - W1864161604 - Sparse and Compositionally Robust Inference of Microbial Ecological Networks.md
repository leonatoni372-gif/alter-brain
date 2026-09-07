---
tags: [literatur, coding]
domain: coding
tahun: 2015
sitasi: 1944
doi: 10.1371/journal.pcbi.1004226
core: "[[Core Ilmu]]"
status_baca: belum
---

# Sparse and Compositionally Robust Inference of Microbial Ecological Networks

- **Penulis:** Zachary Kurtz, Christian L. Müller, Emily R. Miraldi, Dan R. Littman
- **Jurnal:** PLoS Computational Biology
- **Tahun:** 2015 | **Disitasi:** 1944x
- **Link:** https://doi.org/10.1371/journal.pcbi.1004226
- **Konsep:** Inference, Microbial ecology, Statistical inference, Operational taxonomic unit
- **Core:** [[Core Ilmu]]

## Abstrak
16S ribosomal RNA (rRNA) gene and other environmental sequencing techniques provide snapshots of microbial communities, revealing phylogeny and the abundances of microbial populations across diverse ecosystems. While changes in microbial community structure are demonstrably associated with certain environmental conditions (from metabolic and immunological health in mammals to ecological stability in soils and oceans), identification of underlying mechanisms requires new statistical tools, as these datasets present several technical challenges. First, the abundances of microbial operational taxonomic units (OTUs) from amplicon-based datasets are compositional. Counts are normalized to the total number of counts in the sample. Thus, microbial abundances are not independent, and traditional statistical metrics (e.g., correlation) for the detection of OTU-OTU relationships can lead to spurious results. Secondly, microbial sequencing-based studies typically measure hundreds of OTUs on only tens to hundreds of samples; thus, inference of OTU-OTU association networks is severely under-powered, and additional information (or assumptions) are required for accurate inference. Here, we present SPIEC-EASI (SParse InversE Covariance Estimation for Ecological Association Inference), a statistical method for the inference of microbial ecological networks from amplicon sequencing datasets that addresses both of these issues. SPIEC-EASI combines data transformations developed for compositional data analysis with a graphical model inference framework that assumes the underlying ecological association network is sparse. To reconstruct the network, SPIEC-EASI relies on algorithms for sparse neighborhood and inverse covariance selection. To provide a synthetic benchmark in the absence of an experimentally validated gold-standard network, SPIEC-EASI is accompanied by a set of computational tools to generate OTU count data from a set of diverse underlying network topologies. SPIEC-EASI outperforms state-of-the-art methods to recover edges and network properties on synthetic data under a variety of scenarios. SPIEC-EASI also reproducibly predicts previously unknown microbial associations using data from the American Gut project.

## 💡 Insight-ku
-

## 🔗 Terkait
-
