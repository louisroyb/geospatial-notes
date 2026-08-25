# Forestry

**Summary**: Notes on forest mapping, deforestation and degradation monitoring, and commodity-driven forest loss.
**Last updated**: 2026-08-24

---

- [SelvaBox: A high-resolution dataset for tropical tree crown detection](https://arxiv.org/abs/2507.00170): SelvaBox: A high-resolution dataset for tropical tree crown detection. Baudchon, Ouaknine, Weiss, Teng, Walla, Caron-Guay, Pal & Laliberté, arXiv 2507.00170, submitted 30 June 2025 (v2 February 2026). More than 83,000 manually labeled tree crowns in drone imagery at 3–10 cm per pixel across three countries, an order of magnitude larger than earlier tropical forest datasets, aimed at individual tree crown detection that generalises across tropical forest types. *Keywords: tree crown detection, drone imagery, tropical forest, instance annotation, 83000 crowns, benchmark*
  - Related: [[Benchmark_Datasets]], [[Deep_Learning]], [[Data]]

- [Forest Data Partnership on Earth Engine](https://developers.google.com/earth-engine/datasets/publisher/forestdatapartnership): Forest Data Partnership. Publisher page for datasets supporting "global monitoring of commodity-driven deforestation, forest degradation and restoration efforts". Includes per-pixel commodity probability models for cocoa, coffee, palm and rubber at 10 m (2025a and 2025b versions), and Forest Persistence v0, a 30 m score in [0, 1] for whether a pixel held undisturbed forest in 2020, built by convergence of evidence across sources. Several versions are tagged for EUDR compliance; the datasets are not yet peer-reviewed. *Keywords: deforestation, EUDR, commodity mapping, forest persistence, Google Earth Engine, cocoa palm rubber coffee*
  - Related: [[Google_Earth_Engine]], [[Remote_Sensing]], [[Agriculture]]

- [google/forest-data-partnership — models](https://github.com/google/forest-data-partnership/tree/main/models): Forest Data Partnership. The code and artifact repository behind the datasets above, holding downloadable TensorFlow models in versioned folders (`model_20240312/palm`, `model_2024a`, `model_2025a`, `model_2025b`). A companion notebook, `Forest_Data_Partnership_model_hosting.ipynb`, shows how to host a model and call it from Earth Engine. *Keywords: tensorflow models, model hosting, commodity probability, open source, Google Earth Engine, deforestation*
  - Related: [[Google_Earth_Engine]], [[Deep_Learning]]

- [TanDEM-X Forest/Non-Forest Map (FNF50)](https://download.geoservice.dlr.de/FNF50/#details): TanDEM-X Forest/Non-Forest Map - Global. A global forest / non-forest classification at 50 m derived from more than 500,000 TanDEM-X bistatic InSAR images (Stripmap single-polarization HH) acquired 2011–2015, produced by the Microwaves and Radar Institute at DLR. Distributed without warranty and restricted to scientific use under DLR's license terms. *Keywords: TanDEM-X, InSAR, radar, forest non-forest, 50m global, DLR*
  - Related: [[Remote_Sensing]], [[Data]]

## Related topics

[[Remote_Sensing]] · [[Land_Cover]] · [[Code_Repositories]] · [[Geospatial_Platforms]] · [[Google_Earth_Engine]] · [[Agriculture]] · [[Vegetation_Phenology]] · [[Benchmark_Datasets]] · [[Climate_Change]]
