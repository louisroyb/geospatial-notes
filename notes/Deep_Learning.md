# Deep Learning

**Summary**: Notes on neural network architectures and models, particularly for imagery and geospatial tasks.
**Last updated**: 2026-10-03

---

- [Train custom deep learning models without code — QGIS Deepness workflow](https://youtu.be/HIsheKG-lE4): LinkedIn post by Hans van der Kwast, 5 April 2026, on a video tutorial: export training tiles with the QGIS Deepness plugin, annotate in Roboflow, train YOLO with Ultralytics, export to ONNX, and run inference back in Deepness. The example detects wind turbines in aerial photos. *"Personally, I still prefer training people over training models…"* *Keywords: YOLO, QGIS Deepness, Roboflow, ONNX, object detection, no-code*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/jvdkwast_train-custom-deep-learning-models-without-share-7446559794037014528-3gLS); see [[LinkedIn]].
  - Related: [[Learning_Resources]], [[Remote_Sensing]]

- [seapig — area of applicability for EO deep learning](https://www.seapig.dev): LinkedIn post by Darius Görgen, 3 May 2026 (presented at EGU2026): *"{seapig} lets your model abstain from predicting when it encounters unreliable inputs."* A lightweight library for selective inference. It scores inputs by KNN distance in embedding space (Euclidean, cosine, Mahalanobis) or by logit, PCA or PyOD methods, then calibrates thresholds on validation data to hit a target coverage. Integrates with PyTorch Lightning. `pip install seapig`; MIT; Zenodo DOI 10.5281/zenodo.20005134; funded by DFG TRR 391. *Keywords: area of applicability, out-of-distribution, selective inference, uncertainty, PyTorch Lightning, EO*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/darius-goergen_egu2026-share-7456670440292249600-_YMY); see [[LinkedIn]].
  - The deep-learning counterpart to Nowosad's "Where Your Models Can Be Trusted" workshop and to spatial cross-validation on [[Machine_Learning]]. Related: [[Machine_Learning]], [[Remote_Sensing]], [[Code_Repositories]]

- [TorchGeo](https://docs.torchgeo.org/en/stable/): Torchgeo by the GOAT. "A PyTorch domain library, similar to torchvision, providing datasets, samplers, transforms, and pre-trained models specific to geospatial data", aiming both to let ML people work with geospatial data and to let remote sensing people reach for ML. Handles coordinate reference systems automatically when combining datasets, ships benchmark datasets for classification, segmentation and detection, pre-trained weights for multispectral imagery such as Sentinel-2, Lightning datamodules and tasks for reproducible experiments, and a LightningCLI-based command line for training. MIT, ~4.2k stars. Paper: "TorchGeo: Deep Learning With Geospatial Data", *ACM Transactions on Spatial Algorithms and Systems*, August 2025, [10.1145/3707459](https://doi.org/10.1145/3707459). Repository: [microsoft/torchgeo](https://github.com/microsoft/torchgeo). *Keywords: TorchGeo, PyTorch, geospatial datasets, pretrained weights, Lightning, CRS handling*
  - Related: [[Python]], [[Foundation_Models]], [[Benchmark_Datasets]]

- [GeoAI plugin for QGIS](https://plugins.qgis.org/plugins/geoai/#plugin-about): GeoAI plugin for QGIS providing AI-powered geospatial analysis including tree segmentation (DeepForest), water segmentation (OmniWaterMask), Moondream vision-language model, Segment Anything (SAM1/SAM2/SAM3), semantic segmentation, and instance segmentation (Mask R-CNN). Created by Qiusheng Wu and maintained as giswqs, version 1.7.0 released July 2026, for QGIS 3.28 through 4.99. DeepForest covers tree crowns and also birds, livestock, nests and dead trees; SAM supports text, point and box prompts; semantic segmentation takes custom U-Net, DeepLabV3+ or FPN models. Needs the geoai-py package and PyTorch, with a built-in dependency installer that detects NVIDIA CUDA or Apple MPS. Repository: [opengeos/geoai](https://github.com/opengeos/geoai). *Keywords: QGIS plugin, DeepForest, Segment Anything, Moondream, Mask R-CNN, Qiusheng Wu*
  - Related: [[Foundation_Models]], [[Vision_Language_Models]], [[Land_Cover]]

Segmentation and detection models for field boundary delineation — YOLO, Mask R-CNN, FTW, DINOv3, Prithvi — are covered by the `agribound` package in [[Agriculture]]. Vision Transformer architectures underpin the Earth observation embedding products discussed in [[Remote_Sensing]] and [[Embeddings]]. The Forest Data Partnership ships TensorFlow commodity probability models, hosted for Earth Engine — see [[Forestry]].

Three free books cover deep learning on satellite imagery: Qiusheng Wu's *GeoAI with Python*, Caleb Robinson's *Geospatial Machine Learning*, and Isaac Corley's *First Principles of Geospatial Computer Vision*. All three are on [[Learning_Resources]].

From this batch, other pages hold the deep learning applications: tree counting with optimal-transport losses (TreeMatch) and U-Net stand delineation on [[Forestry]], InSAR coherence from GRD with a ResUNet on [[Remote_Sensing]], and Trazo field boundaries on [[Agriculture]]. A semester of reinforcement learning lectures is on [[Learning_Resources]].

## Related topics

A head-to-head of Transformers, LSTM–Transformer hybrids, 1D CNNs and LSTMs against Random Forest and XGBoost on Sentinel time series, including how they transfer to an unseen season, is on [[Agriculture]].

[[Machine_Learning]] · [[Foundation_Models]] · [[Land_Cover]] · [[Agriculture]] · [[Forestry]] · [[Remote_Sensing]] · [[Benchmark_Datasets]] · [[Vision_Language_Models]] · [[Embeddings]] · [[Python]] · [[LinkedIn]] · [[Code_Repositories]]
