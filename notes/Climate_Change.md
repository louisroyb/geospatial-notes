# Climate Change

**Summary**: Notes on climate hazards, extreme events, and the datasets that record them.
**Last updated**: 2026-08-24

---

- [Multisource Remote Sensing data for glacial lakes in the Himalayas](https://zenodo.org/records/16986936): Multisource Remote Sensing data for training and evluating deep learning models in Himalayas. Produced by Saurabh Kaushik, University of Wisconsin-Madison, version 0.1 published 28 August 2025. Ten multispectral and ancillary bands — Sentinel-2 optical, Sentinel-1 SAR coherence, Landsat 8 thermal, plus slope and elevation — paired with annotated lake boundary labels across the Himalaya, for training and validating deep learning models that detect glacial lakes across varied topography and climate zones. CC BY 4.0 and Apache 2.0. *Keywords: glacial lakes, Himalaya, GLOF hazard, multisource, Sentinel-1 coherence, deep learning labels*
  - Related: [[Benchmark_Datasets]], [[Remote_Sensing]]

- [FloodPlanet Inundation Dataset](https://zenodo.org/records/15238572): FloodPlanet Inundation Dataset. Zhang, Melancon, Giezendanner, Tellman & Mukherjee, published 18 April 2025, CC BY 4.0. 366 manual 1024×1024 flood labels drawn on PlanetScope imagery across 19 flood events between 2017 and 2020, with temporally aligned Sentinel-1, Sentinel-2 and Landsat-8 scenes for each, 1.9 GB with a STAC catalog. The value is the cross-sensor alignment: high resolution labels that transfer to the coarser sensors people actually have global archives of. *Keywords: flood inundation, PlanetScope, manual labels, multi-sensor alignment, STAC, 19 flood events*
  - Related: [[Benchmark_Datasets]], [[Remote_Sensing]], [[Data]]

- [MONITRS: Multimodal Observations of Natural Incidents Through Remote Sensing](https://arxiv.org/abs/2507.16228): MONITRS: Multimodal Observations of Natural Incidents Through Remote Sensing. Revankar, Mall, Phoo, Bala & Hariharan, arXiv 2507.16228, submitted 22 July 2025. Pairs temporal satellite imagery with news article annotations and geolocation for more than 10,000 FEMA disaster events, so models can track how a natural disaster develops over time and space; fine-tuning on it improves automated disaster monitoring. Pairs naturally with the Groundsource flood dataset below — both mine news text for hazard events, one for labels on imagery, the other as the record itself. *Keywords: disaster monitoring, FEMA events, multimodal, news annotations, temporal imagery, hazard tracking*
  - Related: [[Remote_Sensing]], [[Benchmark_Datasets]], [[Data]]

- [Groundsource: A Dataset of Flood Events from News](https://zenodo.org/records/18647054): An open global dataset of 2.6 million historical flood events extracted from news articles across more than 150 countries, published February 2026 by Mayo, Zlydenko, Nearing, Kratzert and colleagues. Distributed as a single 667 MB Parquet file under CC BY 4.0. *Keywords: floods, hazard dataset, news extraction, parquet, global coverage, open data*
  - Related: [[Data]]

On extreme heat: a widely shared critique of using satellite land surface temperature as a proxy for heat hazard, with five supporting papers, is filed under [[Urban_Planning]].

## Related topics

[[Data]] · [[Remote_Sensing]] · [[Urban_Planning]] · [[Benchmark_Datasets]] · [[Forestry]] · [[Vegetation_Phenology]]
