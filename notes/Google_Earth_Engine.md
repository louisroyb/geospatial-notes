# Google Earth Engine

**Summary**: Notes on the Google Earth Engine platform — its data catalog, hosted models, and tutorials.
**Last updated**: 2026-10-03

---

- [20-Day Google Earth Engine Mastery](https://github.com/BlueGIS760404/20-Day-Google-Earth-Engine-Course): LinkedIn post by Reza Hosseini, 4 June 2026, sharing a *"free 20-day Google Earth Engine Mastery, designed for students, researchers, GIS professionals, environmental scientists"*. One lesson a day (theory, script, exercises, extension challenge): fundamentals, Sentinel-2 processing, ML land-cover classification, time series, environmental monitoring and web apps. Requires basic JavaScript. No license declared. *Keywords: Earth Engine, self-paced course, JavaScript, land cover classification, time series, GitHub*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/reza-hosseini-a337a51b9_googleearthengine-remotesensing-gis-share-7468304348570234882-Ca6G); see [[LinkedIn]].
  - Related: [[Learning_Resources]]

- [PlotToSat](https://github.com/MiltoMiltiadou/PlotToSat): LinkedIn post by Milto Miltiadou (University of Exeter), 26 June 2026, after running a PlotToSat workshop at the 4th ML4EO Conference. *"PlotToSat efficiently generates time-series signatures from Sentinel-1 and Sentinel-2 imagery across multiple regions (e.g., thousands of field-based plots) for machine learning applications."* It runs in Earth Engine. In one run it processed about 18.3 TB of Sentinel-1/2 data for 15,962 plots in under 24 hours. New spectral-index support was introduced at the workshop; slides are in the repo and a recording is "coming soon". GPL-3.0, so the license is copyleft. The 5th ML4EO conference is 14–16 June 2027 at Exeter. *Keywords: PlotToSat, Earth Engine, Sentinel-1/2 time series, field plots, ML4EO, feature extraction*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/milto-miltiadou_earthobservation-remotesensing-machinelearning-ugcPost-7476263083292884993-3Ab2); see [[LinkedIn]].
  - Related: [[Remote_Sensing]], [[Machine_Learning]], [[Forestry]], [[Code_Repositories]]

- [Empowering the Google Earth Engine Community with Example ADK Agents](https://medium.com/google-earth/empowering-the-google-earth-engine-community-with-example-adk-agents-4afa22dab855): Empowering the Google Earth Engine Community with Example ADK Agents. Google open-sourced two reference agents built on its Agent Development Kit, hosted in the earth-engine-community repository with the tool-calling, orchestration and Earth Engine integration logic included. The EUDR agent automates deforestation due diligence by pulling historical imagery and land-cover data, analysing it for forest loss and generating structured reports flagging high-risk areas for human review. The ForestWise agent acts as a virtual forest analyst, reasoning about land-use transitions with Dynamic World, estimating biomass stocking trends from ESA and GEDI data, and describing the disturbance history of an arbitrary region. *Keywords: ADK, AI agents, EUDR, ForestWise, Dynamic World, GEDI biomass*
  - **Second take** ([LinkedIn, Vikas Kumar, 18 Jun 2026](https://www.linkedin.com/posts/vikknikk_googleearthengine-geospatialai-sustainability-share-7473380345783074816-Z3i-)): *"Instead of writing complex code, users can now interact with Earth Engine using natural language."* The two reference agents are the Sustainable Sourcing Agent (EUDR due diligence and deforestation risk) and the ForestWise Agent (land-use transitions and biomass trends from ESA and GEDI). Both are in [google/earthengine-community](https://github.com/google/earthengine-community) (Apache-2.0, 825 stars).
  - Related: [[Agentic_Coding]], [[Forestry]]

- [QGIS Earth Engine Plugin tutorials](https://gee-community.github.io/qgis-earthengine-plugin/tutorials/): QGIS Earth Engine Plugin. Brings Earth Engine into QGIS so its catalogue can be used from the desktop. Three community tutorials: building a Sentinel-2 median composite for a region and downloading it as GeoTIFF; using the QGIS Model Designer to download and analyse cocoa plantation data from the Earth Engine catalogue; and loading CMIP6 climate projections to display on a globe through the Earth Engine Python API. Maintained by the gee-community organisation, copyright Antony Barja. *Keywords: QGIS, Earth Engine plugin, Model Designer, Sentinel-2 composite, CMIP6, tutorials*
  - Related: [[Learning_Resources]], [[Climate_Change]]

Earth Engine turns up across most of the geospatial notes here. The Satellite Embedding (AlphaEarth) tutorial series and the LandTrendr port — both the [LT-GEE guide](https://emapr.github.io/LT-GEE/introduction.html) and the Kennedy et al. 2018 paper — are filed under [[Remote_Sensing]]. The Forest Data Partnership publishes its commodity probability and forest persistence datasets through the Earth Engine catalog, with TensorFlow models hosted externally and called from Earth Engine; see [[Forestry]]. The `agribound` package in [[Agriculture]] pulls its imagery through Earth Engine as well.

Two FAO tools wrap Earth Engine for people who do not want to write code — SEPAL and Earth Map — both on [[Geospatial_Platforms]]. The Satellite Embedding Deep Dive workshop is worked entirely in the Earth Engine editor; see [[Learning_Resources]].

The open-access EEFA textbook, *Cloud-Based Remote Sensing with Google Earth Engine* (Cardille et al., Springer 2024), covers Earth Engine from JavaScript basics through to applications. It is on [[Learning_Resources]].

Google Earth's no-code Classify tool, which trains a random forest on AlphaEarth embeddings in Earth Engine behind the scenes, is on [[Geospatial_Platforms]]. The GFSM flood-susceptibility Earth Engine app is on [[Climate_Change]].

## Related topics

[[Geospatial_Platforms]] · [[Remote_Sensing]] · [[Forestry]] · [[Agriculture]] · [[Agentic_Coding]] · [[Learning_Resources]] · [[Embeddings]]
