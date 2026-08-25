# Geospatial Platforms

**Summary**: Notes on hosted platforms for accessing and analysing Earth observation data without local infrastructure.
**Last updated**: 2026-08-24

---

- [GeoLibre](https://geolibre.app/getting-started/): Geo Libre from the Goat. An open-source geospatial information system from the opengeos community for visualising, exploring and analysing geospatial data, processing client-side so data stays private. Runs as a lightweight cloud-native GIS in the browser, on desktop, mobile and inside Jupyter, reading vector (GeoJSON, Shapefile), raster (GeoTIFF, COG) and services (WMS, ArcGIS, vector tiles). Features layer styling, a spatial SQL and Python console, processing tools, AI segmentation, story maps and plugins, and works offline. Install paths cover browser, desktop for Windows/macOS/Linux, pip/conda, an R package, mobile apps and self-hosting via Docker with optional Clerk or Auth0 auth. Web app: [web.geolibre.app](https://web.geolibre.app/). *Keywords: GeoLibre, opengeos, client-side GIS, cloud-native, offline, self-hosting*
  - Related: [[Python]], [[Data]]

- [Digital Earth Africa User Guide](https://docs.digitalearthafrica.org/en/latest/index.html): Digital Earth Africa User Guide. Documentation for Digital Earth Africa, "a repository of Earth Observation data and a set of tools to view and analyse the data". The guide splits into technical specifications for every DE Africa dataset, product and service, documentation for the platform tools used to visualise and analyse them, and instructions for reaching the data directly from outside the platform. *Keywords: Digital Earth Africa, EO data repository, user guide, datasets and products, Africa, data access*
  - Related: [[Data]], [[Remote_Sensing]], [[Land_Cover]]

- [GeoLab cloud compute hub now open to all users](https://www.earthscope.org/news/geolab-cloud-compute-hub-now-open-to-all-users/): GeoLab cloud compute hub now open to all users. GeoLab is a cloud JupyterHub from the EarthScope Consortium, run with 2i2c, letting users "explore and analyze data without downloading" and prototype heavy processing workflows, with shareable notebooks that need no local setup. Free to anyone with an EarthScope User Account, subject to a rolling 30-day quota, with 50 GB personal storage plus scratch space. The 9 June 2026 announcement opened it to the whole community, launched at the NSF National Geophysical Facility Community Science Conference, alongside a help desk, community forum, docs and a Cloud Foundations course. *Keywords: GeoLab, EarthScope, JupyterHub, 2i2c, free cloud compute, geophysical data*
  - Related: [[Data]], [[Learning_Resources]]

- [SEPAL](https://docs.sepal.io/en/latest/index.html): *Note: this URL was labelled "Earthmap" in the source table, but it is the SEPAL documentation; the two labels in that row were swapped.* SEPAL — System for Earth Observation Data Access, Processing and Analysis for Land Monitoring — is "a cloud computing-based platform for autonomous land monitoring using remotely sensed data", letting users query and process satellite data, tailor products to local needs, and build geospatial analyses without coding expertise. Part of the Open Foris suite, funded by the Government of Norway through the FAO Forestry Department. Bundles Google Earth Engine for data access with GDAL, Python, R and R Shiny Server, Jupyter, SNAP Toolkit, ORFEO Toolbox and RStudio Server. *Keywords: SEPAL, FAO, Open Foris, cloud processing, land monitoring, no-code analysis*
  - Related: [[Forestry]], [[Google_Earth_Engine]], [[Land_Cover]]

- [Earth Map](https://www.openforis.org/earth-map/#community_section): *Note: this URL was labelled "Sepal" in the source table; the labels in that row were swapped.* A web tool from FAO built with Google that "transforms vast amounts of satellite and climate data into maps and analyses that anyone can use", giving instant visualisation and statistics on forest dynamics, rainfall, temperature and land use without GIS expertise or heavy compute. Runs on Google Earth Engine with Firebase hosting, organises data thematically into Forestry, Climate, Vegetation, Land Degradation and Biodiversity, and works in any browser for registered and anonymous users alike. Aimed at policymakers, researchers, land managers and farmers. *Keywords: Earth Map, FAO, Open Foris, no-code, thematic analysis, climate and forest data*
  - Related: [[Forestry]], [[Google_Earth_Engine]], [[Climate_Change]]

## Platforms filed elsewhere

- **Google Earth Engine** — the planetary-scale analysis platform underpinning both tools above, with its own page: [[Google_Earth_Engine]].
- **Africa GeoPortal** — Esri's free ArcGIS Online access and community data for Africa; see [[Data]].

## Related topics

[[Google_Earth_Engine]] · [[Remote_Sensing]] · [[Forestry]] · [[Data]] · [[Learning_Resources]]
