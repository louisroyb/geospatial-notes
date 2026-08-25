# Deep Learning

**Summary**: Notes on neural network architectures and models, particularly for imagery and geospatial tasks.
**Last updated**: 2026-08-24

---

- [TorchGeo](https://docs.torchgeo.org/en/stable/): Torchgeo by the GOAT. "A PyTorch domain library, similar to torchvision, providing datasets, samplers, transforms, and pre-trained models specific to geospatial data", aiming both to let ML people work with geospatial data and to let remote sensing people reach for ML. Handles coordinate reference systems automatically when combining datasets, ships benchmark datasets for classification, segmentation and detection, pre-trained weights for multispectral imagery such as Sentinel-2, Lightning datamodules and tasks for reproducible experiments, and a LightningCLI-based command line for training. MIT, ~4.2k stars. Paper: "TorchGeo: Deep Learning With Geospatial Data", *ACM Transactions on Spatial Algorithms and Systems*, August 2025, [10.1145/3707459](https://doi.org/10.1145/3707459). Repository: [microsoft/torchgeo](https://github.com/microsoft/torchgeo). *Keywords: TorchGeo, PyTorch, geospatial datasets, pretrained weights, Lightning, CRS handling*
  - Related: [[Python]], [[Foundation_Models]], [[Benchmark_Datasets]]

- [GeoAI plugin for QGIS](https://plugins.qgis.org/plugins/geoai/#plugin-about): GeoAI plugin for QGIS providing AI-powered geospatial analysis including tree segmentation (DeepForest), water segmentation (OmniWaterMask), Moondream vision-language model, Segment Anything (SAM1/SAM2/SAM3), semantic segmentation, and instance segmentation (Mask R-CNN). Created by Qiusheng Wu and maintained as giswqs, version 1.7.0 released July 2026, for QGIS 3.28 through 4.99. DeepForest covers tree crowns and also birds, livestock, nests and dead trees; SAM supports text, point and box prompts; semantic segmentation takes custom U-Net, DeepLabV3+ or FPN models. Needs the geoai-py package and PyTorch, with a built-in dependency installer that detects NVIDIA CUDA or Apple MPS. Repository: [opengeos/geoai](https://github.com/opengeos/geoai). *Keywords: QGIS plugin, DeepForest, Segment Anything, Moondream, Mask R-CNN, Qiusheng Wu*
  - Related: [[Foundation_Models]], [[Vision_Language_Models]], [[Land_Cover]]

Segmentation and detection models for field boundary delineation — YOLO, Mask R-CNN, FTW, DINOv3, Prithvi — are covered by the `agribound` package in [[Agriculture]]. Vision Transformer architectures underpin the Earth observation embedding products discussed in [[Remote_Sensing]] and [[Embeddings]]. The Forest Data Partnership ships TensorFlow commodity probability models, hosted for Earth Engine — see [[Forestry]].

## Related topics

[[Machine_Learning]] · [[Foundation_Models]] · [[Land_Cover]] · [[Agriculture]] · [[Forestry]] · [[Remote_Sensing]] · [[Benchmark_Datasets]] · [[Vision_Language_Models]] · [[Embeddings]] · [[Python]]
