# Foundation Models

**Summary**: Notes on large pretrained models for Earth observation and agriculture — general-purpose backbones, domain-specific alternatives, and the self-supervised training behind them.
**Last updated**: 2026-08-24

---

- [ssl4eo-l — `sample_conus.py`](https://github.com/torchgeo/ssl4eo-l/blob/main/sample_conus.py#L105,L122): *Basically generate 1 random box at a time and check if it overlaps with any existing boxes until you hit your target*. The sampling routine used to lay out non-overlapping tiles when building the SSL4EO-L pretraining dataset — rejection sampling rather than a grid, which is why coverage looks scattered rather than regular. SSL4EO-L is the Landsat counterpart to SSL4EO-S12, providing "datasets and foundation models for Landsat imagery"; the repo holds the configs and scripts to reproduce the dataset and the paper's experiments, split out of TorchGeo into its own project. Paper: Stewart, Lehmann, Corley, Wang et al., NeurIPS 2023, *Advances in Neural Information Processing Systems* 36:59787–59807. *Keywords: SSL4EO-L, rejection sampling, tile layout, Landsat pretraining, TorchGeo, NeurIPS 2023*
  - Related: [[Code_Repositories]], [[Benchmark_Datasets]], [[Learning_Resources]]

- [Detecting Objects From Text Prompts with RasterFlow and Segment Anything 3](https://wherobots.com/blog/sam3-earth-observation-rasterflow/): Wherebots blog. Wherobots ran Meta's Segment Anything 3 over NAIP aerial imagery at county scale through RasterFlow, their serverless "planetary scale inference engine for Earth Intelligence", detecting roofs, containers and tractors from text prompts alone with no training or ad hoc labeling. RasterFlow builds mosaics from multiple raster sources, runs PyTorch vision models over them and vectorises the output into spatial features, supporting semantic segmentation, instance segmentation, object detection and regression at scale. *Keywords: SAM3, RasterFlow, text-prompted detection, NAIP, zero-shot, planetary scale inference*
  - Related: [[Vision_Language_Models]], [[Geospatial_Platforms]], [[Deep_Learning]], [[LinkedIn]]

- [OlmoEarth](https://github.com/allenai/olmoearth_pretrain): OlmoEarth's impact: IFPRI/CGIAR. AI2's "flexible, multi-modal, spatio-temporal family of foundation models for Earth Observations", pretrained on 285,288 global samples of 2.56 × 2.56 km. Inputs span Sentinel-2, Sentinel-1 and Landsat imagery plus six derived map layers — OpenStreetMap, WorldCover, USDA Cropland Data Layer, SRTM DEM, WRI Canopy Height, and WorldCereal. Three versions (v1, v1.1, v1.2) ship at sizes from Nano (~1.7M encoder parameters) through Tiny, Small and Base to Large (308M). Released under the custom OlmoEarth Artifact License rather than a standard open license. *Keywords: OlmoEarth, AI2, multi-modal, spatio-temporal, model family, Earth observation foundation model*
  - Companion link from the note: [OlmoEarth's impact: IFPRI/CGIAR](https://allenai.org/olmoearth-testimonial-ifpri-cgiar) — IFPRI used OlmoEarth to build crop-type maps for Nandi County, Kenya and for Mozambique, combining ground observations with the models to cover the current year plus five prior years. Claimed outcomes are maps in days rather than longer, accuracy "exceeding initial expectations" per IFPRI Senior GIS Coordinator Zhe Guo, and evidence for tracking shifts such as sugarcane and coffee expansion to support food security planning.
  - Related: [[Agriculture]], [[Remote_Sensing]], [[Code_Repositories]]

## Where the argument sits

A running theme across these notes is whether general-purpose geospatial backbones are enough, or whether domains need their own.

- **The case for specialisation** — Nedungadi et al. argue agriculture is under-served by general models and propose a dedicated CropFM; see [[Agriculture]].
- **Domain-specific models** — AgriFM (Video Swin backbone, 25M+ samples across MODIS / Landsat / Sentinel-2) and Time2Agri (seasonality-driven self-supervised pretext tasks) are both on [[Agriculture]], and both report beating general remote sensing foundation models.
- **Multi-modal pretraining** — the M3DRS dataset and the `proj-vit` Scale-MAE work on 5-band imagery sit under [[Remote_Sensing]].
- **Embedding products as frozen foundations** — AlphaEarth, Clay, Presto, Tessera and others ship model outputs rather than weights; see [[Embeddings]] and the interoperability critique on [[Remote_Sensing]].
- **Pretraining corpora** — TerraMesh (IBM/ESA, 9M+ multimodal samples) trained TerraMind-B; see [[Remote_Sensing]] and [[Benchmark_Datasets]].
- **Applied backbones** — Prithvi, DINOv3 and FTW appear as segmentation options in the `agribound` package on [[Agriculture]].

## Related topics

[[Remote_Sensing]] · [[Agriculture]] · [[Vision_Language_Models]] · [[Benchmark_Datasets]] · [[Code_Repositories]] · [[Embeddings]] · [[Deep_Learning]] · [[Machine_Learning]]
