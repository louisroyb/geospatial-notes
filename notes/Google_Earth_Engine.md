# Google Earth Engine

**Summary**: Notes on the Google Earth Engine platform — its data catalog, hosted models, and tutorials.
**Last updated**: 2026-08-24

---

- [Empowering the Google Earth Engine Community with Example ADK Agents](https://medium.com/google-earth/empowering-the-google-earth-engine-community-with-example-adk-agents-4afa22dab855): Empowering the Google Earth Engine Community with Example ADK Agents. Google open-sourced two reference agents built on its Agent Development Kit, hosted in the earth-engine-community repository with the tool-calling, orchestration and Earth Engine integration logic included. The EUDR agent automates deforestation due diligence by pulling historical imagery and land-cover data, analysing it for forest loss and generating structured reports flagging high-risk areas for human review. The ForestWise agent acts as a virtual forest analyst, reasoning about land-use transitions with Dynamic World, estimating biomass stocking trends from ESA and GEDI data, and describing the disturbance history of an arbitrary region. *Keywords: ADK, AI agents, EUDR, ForestWise, Dynamic World, GEDI biomass*
  - Related: [[Agentic_Coding]], [[Forestry]]

- [QGIS Earth Engine Plugin tutorials](https://gee-community.github.io/qgis-earthengine-plugin/tutorials/): QGIS Earth Engine Plugin. Brings Earth Engine into QGIS so its catalogue can be used from the desktop. Three community tutorials: building a Sentinel-2 median composite for a region and downloading it as GeoTIFF; using the QGIS Model Designer to download and analyse cocoa plantation data from the Earth Engine catalogue; and loading CMIP6 climate projections to display on a globe through the Earth Engine Python API. Maintained by the gee-community organisation, copyright Antony Barja. *Keywords: QGIS, Earth Engine plugin, Model Designer, Sentinel-2 composite, CMIP6, tutorials*
  - Related: [[Learning_Resources]], [[Climate_Change]]

Earth Engine turns up across most of the geospatial notes here. The Satellite Embedding (AlphaEarth) tutorial series and the LandTrendr port — both the [LT-GEE guide](https://emapr.github.io/LT-GEE/introduction.html) and the Kennedy et al. 2018 paper — are filed under [[Remote_Sensing]]. The Forest Data Partnership publishes its commodity probability and forest persistence datasets through the Earth Engine catalog, with TensorFlow models hosted externally and called from Earth Engine; see [[Forestry]]. The `agribound` package in [[Agriculture]] pulls its imagery through Earth Engine as well.

Two FAO tools wrap Earth Engine for people who do not want to write code — SEPAL and Earth Map — both on [[Geospatial_Platforms]]. The Satellite Embedding Deep Dive workshop is worked entirely in the Earth Engine editor; see [[Learning_Resources]].

## Related topics

[[Geospatial_Platforms]] · [[Remote_Sensing]] · [[Forestry]] · [[Agriculture]] · [[Agentic_Coding]] · [[Learning_Resources]] · [[Embeddings]]
