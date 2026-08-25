# Land Cover

**Summary**: Notes on land cover and land use mapping — classification schemes, segmentation methods, and the benchmarks that test them.
**Last updated**: 2026-08-24

---

- [S5: Scalable Semi-Supervised Semantic Segmentation in Remote Sensing](https://arxiv.org/abs/2508.12409): S5: Scalable Semi-Supervised Semantic Segmentation in Remote Sensing. Lv, Wang, Zhang & Zhang, arXiv 2508.12409, submitted 17 August 2025 (revised December 2025), AAAI 2026 Oral. Attacks the scalability limits of semi-supervised segmentation with entropy-based data filtering and a pretraining paradigm called S4P, using a curated 1M-image corpus (RS4P-1M) to pretrain backbones, then a Mixture-of-Experts multi-dataset fine-tuning step for adaptation. Reports state of the art across several land cover segmentation and object detection benchmarks. Code: [MiliLab/S5](https://github.com/MiliLab/S5). *Keywords: semi-supervised learning, semantic segmentation, RS4P-1M, mixture of experts, AAAI 2026, pretraining*
  - Related: [[Foundation_Models]], [[Deep_Learning]], [[Code_Repositories]]

- [HieraRS: A Hierarchical Segmentation Paradigm for Remote Sensing](https://github.com/AI-Tianlong/HieraRS): HieraRS: A Hierarchical Segmentation Paradigm for Remote Sensing Enabling Multi-Granularity Interpretation and Cross-Domain Transfer. Tackles two gaps in land cover / land use segmentation: flat classifiers cannot produce end-to-end multi-granularity predictions matching the tree-structured hierarchies practitioners actually use, and models transfer badly across domains with different category structures. Two pieces do the work — BHCCM, a bidirectional hierarchical consistency constraint that drops into standard flat models to yield hierarchical predictions with better semantic consistency, and TransLU, a dual-branch transfer framework combining cross-domain knowledge sharing and semantic alignment. Evaluated on MM-5B (a multi-modal hierarchical LCLU dataset built on Five-Billion-Pixels), Crop10m (Sentinel-2 crop classification in northeastern China), and WHDLD. Accepted to IEEE TGRS March 2026; preprint July 2025. *Keywords: hierarchical segmentation, LCLU, cross-domain transfer, semantic consistency, MM-5B, multi-granularity*
  - Related: [[Deep_Learning]], [[Agriculture]], [[Benchmark_Datasets]]

- [OpenEarthMap-SAR](https://github.com/cliffbb/OpenEarthMap-SAR): OpenEarthMap-SAR. "A high-resolution SAR benchmark dataset for land cover mapping under all-weather conditions" — 1.5 million segments from 5,033 aerial and satellite images across 35 regions in Japan, France and the USA, tiled at 1024×1024 with ground sampling distance of 0.15–0.5 m. Eight land cover classes, with both manual and pseudo labels, supporting semantic segmentation, unsupervised domain adaptation, and image translation. Served as the official dataset for Track 1 of the 2025 IEEE GRSS Data Fusion Contest on all-weather land cover and building damage mapping. MIT licensed; cite Xia et al. 2025, arXiv:2501.10891. *Keywords: SAR, all-weather mapping, land cover, data fusion contest, domain adaptation, benchmark*
  - Related: [[Remote_Sensing]], [[Benchmark_Datasets]], [[Data]]

## Related topics

[[Remote_Sensing]] · [[Agriculture]] · [[Forestry]] · [[Foundation_Models]] · [[Benchmark_Datasets]] · [[Code_Repositories]] · [[Deep_Learning]]
