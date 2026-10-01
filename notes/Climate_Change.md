# Climate Change

**Summary**: Notes on climate hazards, extreme events, and the datasets that record them.
**Last updated**: 2026-10-02

---

- [Calculating full-year energy savings with only 6 months of data](https://www.reimagine-energy.ai/p/calculating-full-year-energy-savings): A tutorial by Benedetto Grillone in his *Reimagine Energy* newsletter, 24 November 2024. The problem: an energy conservation measure (ECM) goes in mid-year, and only six months of post-installation data exist, but you need the annual savings. The method trains a LightGBM baseline on pre-ECM consumption to predict what the building would have used without the measure. A second model then projects the rest of the year, and the savings are the gap between the two. The data are hourly electricity readings from the Building Data Genome Project 2 and weather from the National Solar Radiation Database, with hour, day-of-week, week, weather variables and an ECM on/off flag as features. The worked example comes to about 5,350 kWh a year. Grillone names three caveats: *"Seasonality: If savings are seasonal and not all seasons are represented in your post-installation data, this method may not be reliable"*; non-routine events or operational changes can invalidate the projection; and future weather has to come from historical averages or climate models. Code uses pandas, LightGBM and Plotly; no repository is linked. *Keywords: energy savings, measurement and verification, LightGBM, building energy, baseline model, BDG2*
  - The note's link was the author's Substack (`benedettogrillone.substack.com`), which now redirects permanently to `reimagine-energy.ai`.
  - BDG2 comes from Clayton Miller's BUDS Lab at NUS, the same group behind the data science for buildings course on [[Learning_Resources]].
  - Related: [[Machine_Learning]], [[Urban_Planning]], [[Python]], [[Data]]

- [CarbonSIG: Carbon Resources Management platform - CaRMa](https://www.youtube.com/watch?v=ni9eN16-BiM): A one-minute product video from the CarbonSIG YouTube channel, posted 18 September 2024. CaRMa, the Carbon Resources Management platform, is described as *"a comprehensive solution allowing to record, model, and manage any process, environment, or supply chain, with a focus on carbon"*. It produces carbon-flow reports aimed at managers, sales teams and executives. The video is a vendor pitch, not a technical walkthrough. *Keywords: carbon accounting, carbon management, supply chain emissions, CaRMa, CarbonSIG, software platform*
  - Related: [[Data]]

- [Multisource Remote Sensing data for glacial lakes in the Himalayas](https://zenodo.org/records/16986936): Multisource Remote Sensing data for training and evluating deep learning models in Himalayas. Produced by Saurabh Kaushik, University of Wisconsin-Madison, version 0.1 published 28 August 2025. Ten multispectral and ancillary bands — Sentinel-2 optical, Sentinel-1 SAR coherence, Landsat 8 thermal, plus slope and elevation — paired with annotated lake boundary labels across the Himalaya, for training and validating deep learning models that detect glacial lakes across varied topography and climate zones. CC BY 4.0 and Apache 2.0. *Keywords: glacial lakes, Himalaya, GLOF hazard, multisource, Sentinel-1 coherence, deep learning labels*
  - Related: [[Benchmark_Datasets]], [[Remote_Sensing]]

- [FloodPlanet Inundation Dataset](https://zenodo.org/records/15238572): FloodPlanet Inundation Dataset. Zhang, Melancon, Giezendanner, Tellman & Mukherjee, published 18 April 2025, CC BY 4.0. 366 manual 1024×1024 flood labels drawn on PlanetScope imagery across 19 flood events between 2017 and 2020, with temporally aligned Sentinel-1, Sentinel-2 and Landsat-8 scenes for each, 1.9 GB with a STAC catalog. The value is the cross-sensor alignment: high resolution labels that transfer to the coarser sensors people actually have global archives of. *Keywords: flood inundation, PlanetScope, manual labels, multi-sensor alignment, STAC, 19 flood events*
  - Related: [[Benchmark_Datasets]], [[Remote_Sensing]], [[Data]]

- [MONITRS: Multimodal Observations of Natural Incidents Through Remote Sensing](https://arxiv.org/abs/2507.16228): MONITRS: Multimodal Observations of Natural Incidents Through Remote Sensing. Revankar, Mall, Phoo, Bala & Hariharan, arXiv 2507.16228, submitted 22 July 2025. Pairs temporal satellite imagery with news article annotations and geolocation for more than 10,000 FEMA disaster events, so models can track how a natural disaster develops over time and space; fine-tuning on it improves automated disaster monitoring. Pairs naturally with the Groundsource flood dataset below — both mine news text for hazard events, one for labels on imagery, the other as the record itself. *Keywords: disaster monitoring, FEMA events, multimodal, news annotations, temporal imagery, hazard tracking*
  - Related: [[Remote_Sensing]], [[Benchmark_Datasets]], [[Data]]

- [Groundsource: A Dataset of Flood Events from News](https://zenodo.org/records/18647054): An open global dataset of 2.6 million historical flood events extracted from news articles across more than 150 countries, published February 2026 by Mayo, Zlydenko, Nearing, Kratzert and colleagues. Distributed as a single 667 MB Parquet file under CC BY 4.0. *Keywords: floods, hazard dataset, news extraction, parquet, global coverage, open data*
  - Related: [[Data]]

On extreme heat: a widely shared critique of using satellite land surface temperature as a proxy for heat hazard, with five supporting papers, is filed under [[Urban_Planning]].

Two paid climate courses are on [[Learning_Resources]]: Skill Up for Earth's Oxford Certificate in Climate Solutions & Strategies, and Nina Benoit's course on AI's own carbon and water footprint and on using AI for ESG and GHG reporting.

## Related topics

[[Data]] · [[Remote_Sensing]] · [[Urban_Planning]] · [[Benchmark_Datasets]] · [[Forestry]] · [[Vegetation_Phenology]]
