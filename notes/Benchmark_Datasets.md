# Benchmark Datasets

**Summary**: Hub page for labeled datasets and benchmarks collected across the knowledge base, grouped by what they are built to test.
**Last updated**: 2026-10-03

---

Datasets are filed on their subject pages; this page gathers the pointers.

- **S2GAIA** — 34,030 seasonally structured Sentinel-2 patches over Greece, 2017–2024, 22 LULC classes, 92.1 GB on Zenodo under CC-BY-4.0. Tests seasonal, national-scale land cover mapping. On [[Land_Cover]].

**Pretraining corpora (unlabeled or weakly labeled)**
- TerraMesh — 9M+ globally distributed samples, seven co-registered modalities at 10 m, trained TerraMind-B. See [[Remote_Sensing]].
- SSL4EO-L — Landsat pretraining dataset built by rejection-sampled non-overlapping tiles; NeurIPS 2023. See [[Foundation_Models]].
- OlmoEarth — 285,288 global samples of 2.56 km², Sentinel-1/2 and Landsat plus six derived map layers. See [[Foundation_Models]].
- M3DRS — ~400,000 five-channel images at 10–25 cm over Switzerland, France and Italy, released unlabeled for self-supervised work. See [[Remote_Sensing]].

**Location encoding**
- CoordBench — 52 datasets and 78 target variables with random and regional holdouts at several spatial scales, released with MIND. See [[Embeddings]].

**Vision-language**
- GroundSet — 3.8M cadastral-grounded objects across 510k images, 135 categories, plus a 7-task spatial reasoning benchmark. See [[Vision_Language_Models]].
- RSVLM-QA — 13,820 images, 162,373 VQA pairs, GPT-4.1 assisted. See [[Vision_Language_Models]].
- Landsat30-AU — 196,262 captions and 17,725 VQA samples over 36+ years of Australian Landsat. See [[Vision_Language_Models]].

**Segmentation and land cover**
- OpenEarthMap-SAR — 1.5M segments, eight classes, all-weather SAR; 2025 IEEE GRSS Data Fusion Contest Track 1. See [[Land_Cover]].
- LAS (LAnd Segment) — ~150k global sample locations with RGB, Planet, Sentinel-2 and Landsat imagery, mixing precise and weak LULC labels; built to train LandSegmenter. See [[Land_Cover]].
- So2Sat LCZ42 — 400,000+ Sentinel-1/2 patch pairs labelled with 17 Local Climate Zones across 42 cities, now with geolocations. See [[Urban_Planning]].
- S1S2_AI4LCC — co-located Sentinel-1/2 with 5-class AI4LCC land cover labels over Northern Africa, 13.9 GB in Zarr. See [[Land_Cover]].
- HieraRS / MM-5B — hierarchical multi-granularity LCLU labels. See [[Land_Cover]].
- RS4P-1M — 1M-image curated pretraining corpus behind S5. See [[Land_Cover]].

**Object and boundary extraction**
- Trees outside forests (TOFMapper) — hedgerow, individual tree, grove and forest labels on German aerial imagery, CC-BY-4.0 on Zenodo. See [[Forestry]].
- TreeScanPL10K — 10,417 trees segmented in terrestrial laser scans from 272 Polish plots, about 72% labelled across 30 species. See [[Forestry]].
- Infra-Bench CLS — 18,756 Sentinel-1/2 chips, 13 critical-infrastructure classes on 7 continents; benchmarks seven EO foundation models. See [[Foundation_Models]].
- FBIS-22M — the field-boundary instance segmentation dataset behind Delineate Anything. See [[Agriculture]].
- ORBITaL-Net — 128,270 Maxar VHR chips with building labels across 72 countries. See [[Urban_Planning]].
- OpenFACADES — 31,180 annotated street-view building images (plus 1.2M auto-labelled) with type, floors, age and material. See [[Urban_Planning]].
- CropGlobe — 300,000 crop-type samples across 8 countries and 5 continents, for testing transfer. See [[Agriculture]].
- Kenya Helmets Labeling Crops — 4,925 street-level crop-type validation points. See [[Agriculture]].
- MMEarth — 1.2M locations with 12 aligned modalities, for multi-modal pretraining. See [[Foundation_Models]].
- SpectralEarth — 538,974 EnMAP hyperspectral patches for pretraining, plus nine downstream benchmarks. See [[Foundation_Models]].
- TinyTrees — 216M individual trees over 25,890 km² of China, Rwanda and France from 3 sensors, for counting rather than crown delineation; ECCV 2026. See [[Forestry]].
- Trazo — 40,000+ crop field boundaries across 17 South American ecoregions, extending Fields of the World. See [[Agriculture]].
- SelvaBox — 83,000+ manually labeled tropical tree crowns in 3–10 cm drone imagery. See [[Forestry]].
- Fields of the World — 1.6M labeled parcels across 24 countries, plus a 3.17B-polygon global product. See [[Agriculture]].
- GTPBD — 200,000+ terraced parcels with boundaries, masks and labels. See [[Agriculture]].
- VHRV — 10,158 annotated vessels in very high resolution imagery, with baseline weights. See [[Remote_Sensing]].
- GlobalBuildingAtlas — 2.75B building polygons with heights and LoD1 3D models. See [[Urban_Planning]].

**Multimodal and time series**
- UAVScenes — ~120,000 labeled image and LiDAR pairs with 6-DoF poses. See [[Remote_Sensing]].
- MONITRS — 10,000+ FEMA disaster events pairing temporal imagery with news annotations. See [[Climate_Change]].
- HydroPML — datasets and baselines for physics-aware ML in rainfall-runoff, flood and landslide forecasting. See [[Climate_Change]].
- GMIA-NEXT ground truth — nearly 400,000 irrigation ground-truth points behind a global 30 m irrigated-area map. See [[Agriculture]].
- Groundsource — 2.6M flood events mined from news across 150+ countries. See [[Climate_Change]].
- FloodPlanet — 366 manual flood labels on PlanetScope with aligned Sentinel-1/2 and Landsat-8. See [[Climate_Change]].
- Himalayan glacial lakes — 10 bands plus lake boundary labels for glacial lake detection. See [[Climate_Change]].

**Competitions and funded data**
- Zindi Côte d'Ivoire Byte-Sized Agriculture Challenge — geometry-free cocoa, palm and rubber classification. See [[Agriculture]].
- Lacuna Fund agricultural datasets — funded labeling for sub-Saharan Africa. See [[Agriculture]].
- HarvestStat-Africa — harmonized subnational crop statistics for 33 countries. See [[Agriculture]].

## Related topics

[[Code_Repositories]] · [[Community_Resources]] · [[Remote_Sensing]] · [[Vision_Language_Models]] · [[Land_Cover]] · [[Urban_Planning]] · [[Agriculture]] · [[Forestry]] · [[Climate_Change]] · [[Foundation_Models]] · [[Data]]
