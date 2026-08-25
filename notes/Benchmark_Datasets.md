# Benchmark Datasets

**Summary**: Hub page for labeled datasets and benchmarks collected across the knowledge base, grouped by what they are built to test.
**Last updated**: 2026-08-25

---

Datasets are filed on their subject pages; this page gathers the pointers.

- **S2GAIA** — 34,030 seasonally structured Sentinel-2 patches over Greece, 2017–2024, 22 LULC classes, 92.1 GB on Zenodo under CC-BY-4.0. Tests seasonal, national-scale land cover mapping. On [[Land_Cover]].

**Pretraining corpora (unlabeled or weakly labeled)**
- TerraMesh — 9M+ globally distributed samples, seven co-registered modalities at 10 m, trained TerraMind-B. See [[Remote_Sensing]].
- SSL4EO-L — Landsat pretraining dataset built by rejection-sampled non-overlapping tiles; NeurIPS 2023. See [[Foundation_Models]].
- OlmoEarth — 285,288 global samples of 2.56 km², Sentinel-1/2 and Landsat plus six derived map layers. See [[Foundation_Models]].
- M3DRS — ~400,000 five-channel images at 10–25 cm over Switzerland, France and Italy, released unlabeled for self-supervised work. See [[Remote_Sensing]].

**Vision-language**
- RSVLM-QA — 13,820 images, 162,373 VQA pairs, GPT-4.1 assisted. See [[Vision_Language_Models]].
- Landsat30-AU — 196,262 captions and 17,725 VQA samples over 36+ years of Australian Landsat. See [[Vision_Language_Models]].

**Segmentation and land cover**
- OpenEarthMap-SAR — 1.5M segments, eight classes, all-weather SAR; 2025 IEEE GRSS Data Fusion Contest Track 1. See [[Land_Cover]].
- HieraRS / MM-5B — hierarchical multi-granularity LCLU labels. See [[Land_Cover]].
- RS4P-1M — 1M-image curated pretraining corpus behind S5. See [[Land_Cover]].

**Object and boundary extraction**
- SelvaBox — 83,000+ manually labeled tropical tree crowns in 3–10 cm drone imagery. See [[Forestry]].
- Fields of the World — 1.6M labeled parcels across 24 countries, plus a 3.17B-polygon global product. See [[Agriculture]].
- GTPBD — 200,000+ terraced parcels with boundaries, masks and labels. See [[Agriculture]].
- VHRV — 10,158 annotated vessels in very high resolution imagery, with baseline weights. See [[Remote_Sensing]].
- GlobalBuildingAtlas — 2.75B building polygons with heights and LoD1 3D models. See [[Urban_Planning]].

**Multimodal and time series**
- UAVScenes — ~120,000 labeled image and LiDAR pairs with 6-DoF poses. See [[Remote_Sensing]].
- MONITRS — 10,000+ FEMA disaster events pairing temporal imagery with news annotations. See [[Climate_Change]].
- Groundsource — 2.6M flood events mined from news across 150+ countries. See [[Climate_Change]].
- FloodPlanet — 366 manual flood labels on PlanetScope with aligned Sentinel-1/2 and Landsat-8. See [[Climate_Change]].
- Himalayan glacial lakes — 10 bands plus lake boundary labels for glacial lake detection. See [[Climate_Change]].

**Competitions and funded data**
- Zindi Côte d'Ivoire Byte-Sized Agriculture Challenge — geometry-free cocoa, palm and rubber classification. See [[Agriculture]].
- Lacuna Fund agricultural datasets — funded labeling for sub-Saharan Africa. See [[Agriculture]].
- HarvestStat-Africa — harmonized subnational crop statistics for 33 countries. See [[Agriculture]].

## Related topics

[[Code_Repositories]] · [[Community_Resources]] · [[Remote_Sensing]] · [[Vision_Language_Models]] · [[Land_Cover]] · [[Urban_Planning]] · [[Agriculture]] · [[Forestry]] · [[Climate_Change]] · [[Foundation_Models]] · [[Data]]
