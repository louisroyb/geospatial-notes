# Python

**Summary**: Notes on Python packages and libraries, especially for geospatial and scientific work.
**Last updated**: 2026-10-03

---

- [Smoothify — smooth staircase polygons from rasters](https://github.com/DPIRD-DMA/Smoothify): LinkedIn post by Nicholas Wright, 2 June 2026: *"Vectorise a raster and you get staircases."* Smoothify smooths polygons and lines (holes included) and whole GeoDataFrames, preserving area, using an optimised Chaikin corner-cutting algorithm. `pip install smoothify`; MIT, 213 stars. *Keywords: polygon smoothing, vectorisation, Chaikin, GeoPandas, segmentation masks, cartography*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/nicholas-wright-92205985_python-gis-remotesensing-ugcPost-7467432960795832321-1QWQ); see [[LinkedIn]].
  - Related: [[Cartography]], [[Deep_Learning]], [[Code_Repositories]]

- [PyGStat — geostatistics for modern Python](https://zia207.github.io/PyGStat/): LinkedIn post by Zia Ahmed, 11 September 2026: *"PyGStat brings together classical geostatistics, kriging, variogram modeling, simulation, spatial/spatiotemporal methods, machine learning, deep learning, and GPU-accelerated computing in a modern Python framework."* Kriging: ordinary, simple, universal, indicator, co-, regression, Poisson, Empirical Bayesian and spatiotemporal, plus GSLIB-style 3-D. Simulation: SGSIM/SISIM. ML: deep-learning regression kriging, GNNs, spatiotemporal graph transformers, ConvLSTM. `pip install pygstat` (v0.1.1). Repo: [zia207/PyGStat](https://github.com/zia207/PyGStat), MIT. *Keywords: geostatistics, kriging, variogram, spatial simulation, GPU, Python package*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/zia-ahmed207_pygstat-share-7504241259574681600-pWKA); see [[LinkedIn]].
  - Related: [[Machine_Learning]], [[Code_Repositories]]

- [Easy-EO — EO analysis in a few lines](https://github.com/Tommy-Burns/easy-eo): Reshared on LinkedIn by EM CDE (10 Aug 2026) from Thomas Burns Botchwey, an EM CDE student: *"Give me 20 minutes, and I'll show you why."* An 18-minute [video walkthrough](https://youtu.be/rQJByMOTAaA) of his lightweight library for chainable raster processing, raster algebra and visualisation without the usual boilerplate. [Docs](https://easy-eo.readthedocs.io/en/latest/), MIT. *Keywords: Easy-EO, raster processing, Python library, raster algebra, beginners, EO*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/em-cde-b55780171_learn-eo-python-share-7492466531419955201-cGlf); see [[LinkedIn]].
  - Related: [[Remote_Sensing]], [[Code_Repositories]]

- [fundayao — a remote sensing library written entirely by AI](https://gitee.com/timobalz/fundayao): LinkedIn post by Timo Balz, 1 September 2026: *"Every line of code, every test, every docstring was written by AI."* A teaching library for his courses on the basic principles of remote sensing, released under The Unlicense, `pip install fundayao` (v0.2.0). Hosted on Gitee, not GitHub, so it isn't in the repository tracker. *Keywords: remote sensing teaching, AI-written code, Python library, Gitee, Unlicense, education*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/timo-balz-a9b03936_remotesensing-python-opensource-ugcPost-7500468325676711936-AXiU); see [[LinkedIn]].
  - Related: [[Agentic_Coding]], [[Remote_Sensing]], [[Learning_Resources]]

- [Announcing jupyter-tiler](https://geojupyter.org/blog/20260622-jupyter-tiler/): LinkedIn post by Matt Fisher (Schmidt Center for Data Science & Environment, UC Berkeley), 22 June 2026. jupyter-tiler is a GeoJupyter server extension that runs a dynamic tile server (TiTiler or Xpublish-tiles) inside Jupyter or JupyterHub, so *"You can directly visualize your xarray DataArray on a slippy map widget without the typical intermediate step of writing out a file."* It is integrated into JupyterGIS, still in alpha: `pip install --pre jupytergis[tiler]==0.16.0a4`. [Docs](https://jupyter-tiler.readthedocs.io/). Code: [geojupyter/jupyter-tiler](https://github.com/geojupyter/jupyter-tiler), BSD-3-Clause. *Keywords: jupyter-tiler, xarray, TiTiler, JupyterGIS, dynamic tiles, GeoJupyter*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/mattfisher8_announcing-jupyter-tiler-share-7474852181972631552-vleV); see [[LinkedIn]]. LinkedIn served an unrelated post at the slug URL; the real post was read from its `feed/update` URL.
  - Related: [[Cartography]], [[Data]], [[Code_Repositories]]

- [Pete Gadomski — High-performance Cloud-Native Geospatial Python packages using Rust](https://www.youtube.com/watch?v=zRV-ANGZgzU): A talk from the *Scientific Computing in Rust* 2026 online workshop, published 10 July 2026. The premise: *"While Python is the traditional language for geospatial processing and analytics, most high-performance tools require non-Python components to get acceptable performance (think numpy)."* It argues for writing those components in Rust (via pyo3) and walks through two Development Seed / stac-utils libraries. [obstore](https://github.com/developmentseed/obstore) (MIT) is *"the simplest, highest-throughput Python interface to Amazon S3, Google Cloud Storage, Azure Storage"*. [rustac](https://github.com/stac-utils/rustac) (Apache-2.0) is STAC in Rust, with stac-geoparquet and async API queries. The same Rust code can also be compiled to WebAssembly for the browser. *Keywords: Rust, pyo3, obstore, rustac, cloud-native geospatial, STAC*
  - The same Rust-plus-WASM approach is behind geolibre-rust on [[Geospatial_Platforms]]. STAC Browser and STAC Index are on [[Data]].
  - Related: [[Data]], [[Geospatial_Platforms]]

- [PyGeoFetch](https://github.com/EOCoreINT/pygeofetch): LinkedIn post by Samuel Appiah Kubi, 22 July 2026, introducing an open-source package for one problem: *"Every provider has different auth, queries, and formats and every project means re-learning"*, which he says hits institutions in Africa and the Global South hardest. One CLI and Python API searches and downloads from 20+ providers (USGS, Copernicus, NASA, Planet, Maxar and others). It also does optical preprocessing (cloud masking, pan-sharpening, mosaicking), computes 17+ spectral indices (NDVI, NDWI, EVI, NBR, dNBR, LST) and runs a full Sentinel-1 SLC InSAR pipeline in pure Python. Workflows can be scheduled from YAML. Install with `pip install pygeofetch`; [docs](https://appiahkubis14.github.io/pygeofetch-docs/); MIT. Free tutorials are at eocoreint.com. *Keywords: satellite data access, multi-provider download, InSAR, spectral indices, Python package, Global South*
  - **Citable release** ([LinkedIn, 25 Aug 2026](https://www.linkedin.com/posts/samuel-appiah-kubi-b52633333_openscience-reproducibleresearch-insar-share-7497996802344935424-v9H8)): v2.6.2.1 is archived on Zenodo with DOI [10.5281/zenodo.22087230](https://doi.org/10.5281/zenodo.22087230), and the repo now has a `CITATION.cff`. *"Open science requires more than just public code; it requires permanent, citable, and versioned archives."* A JOSS paper on the architecture, the "Preflight Gate" and a validated InSAR chain is in preparation.
  - Source: [LinkedIn post](https://www.linkedin.com/posts/samuel-appiah-kubi-b52633333_pygeofetch-earthobservation-remotesensing-ugcPost-7485712214419464192-4Mqz); see [[LinkedIn]]. All three `lnkd.in` links (PyPI, docs, GitHub) were resolved.
  - Related: [[Remote_Sensing]], [[Data]], [[Code_Repositories]]

- [PDAL Python for Beginners: Working with LAS/LAZ LiDAR Data](https://www.geowgs84.ai/post/pdal-python-for-beginners-working-with-las-laz-lidar-data): A short tutorial from GeoWGS84.ai on PDAL, *"an open-source software library used to read, write, filter, translate, and process point cloud data."* It covers installing with conda or pip, how JSON pipelines are built (reader → filters → writer), reading LAS into NumPy arrays, compressing LAS to LAZ, ground classification with the SMRF filter, cropping to a bounding box, reprojecting, and writing a DTM to GeoTIFF. It ends with NumPy statistics and a mention of GeoPandas, Rasterio and Shapely. The page carries the year-less date "July 10" and doubles as marketing for GeoWGS84.ai's GeoAI services. *Keywords: PDAL, LiDAR, LAS/LAZ, point cloud, SMRF ground filter, DTM*
  - Related: [[Remote_Sensing]], [[Data]], [[Forestry]]

- [PySTAC](https://github.com/stac-utils/pystac): Python library for working with any SpatioTemporal Asset Catalog (STAC). The reference Python implementation of the STAC specification, covering reading, creating and manipulating catalogs and items, with optional jsonschema validation, orjson for speed, urllib3 retries, Jupyter display of STAC objects, and an extension system where each STAC extension is its own independently versioned package. Documented at pystac.readthedocs.io. *Keywords: PySTAC, STAC, catalog manipulation, extensions, validation, python library*
  - Related: [[Data]], [[Code_Repositories]]

- [Introducing eo-learn](https://medium.com/sentinel-hub/introducing-eo-learn-ab37f2869f5c): Introducing eo-learn / Bridging the gap between Earth Observation and Machine Learning. Sentinel Hub's Python framework for EO processing, built to lower the entry barrier to remote sensing for data scientists while bringing Python's computer vision and ML tooling to remote sensing experts. Work is organised around three abstractions: an EOPatch holding all data for a bounding box (raster time series, vector data, one-off masks such as land cover), EOTasks that transform patches (cloud masking, spectral indices, feature extraction, classification), and EOWorkflows that chain tasks into computational graphs with parallelisation and record keeping. Repository: [sentinel-hub/eo-learn](https://github.com/sentinel-hub/eo-learn). *Keywords: eo-learn, Sentinel Hub, EOPatch, EOTask, workflow graphs, EO processing framework*
  - Related: [[Machine_Learning]], [[Remote_Sensing]], [[Data]]

- [Extracting Time Series at Multiple Points with Xarray](https://www.geopythontutorials.com/notebooks/xarray_extracting_time_series_multiple.html): Extracting Time Series at Multiple Points with Xarray. Ujaval Gandhi's tutorial taking "12 individual Cloud-Optimized GeoTIFF (COG) files representing Soil Moisture for each month of a year", building an Xarray Dataset from them, and extracting values at many point locations at once. Uses Xarray with rioxarray for raster I/O, GeoPandas for the points, Dask for parallelism and Pandas to pivot the result into a wide table with months as columns; the core trick is interpolation and nearest-neighbour selection to sample a gridded dataset at points. CC BY 4.0. *Keywords: Xarray, time series extraction, COG, rioxarray, Dask, point sampling*
  - Related: [[Data]], [[Learning_Resources]]

- [Thresholding - scikit-image](https://scikit-image.org/docs/0.25.x/auto_examples/segmentation/plot_thresholding.html): Thresholding. The scikit-image example on turning grayscale images into binary ones. Covers Otsu's method, which finds an optimal threshold "by maximizing the variance between two classes of pixels", and `try_all_threshold`, which runs several algorithms at once (Isodata, Li, Mean, Minimum, Triangle, Yen) so you can "select the best algorithm for your data without a deep understanding of their mechanisms". Thresholding is the cheap first step before segmentation and object detection. *Keywords: scikit-image, Otsu, thresholding, binary segmentation, try_all_threshold, preprocessing*
  - Related: [[Land_Cover]], [[Deep_Learning]]

The `agribound` package for agricultural field boundary delineation (Python 3.10+, built on GDAL, Rasterio, GeoPandas and PyTorch) is noted in [[Agriculture]]. Related geospatial tooling — GDAL, Rasterio, TorchGeo — also appears in [[Remote_Sensing]]. The UCLA Urban Data Science course on [[Urban_Planning]] teaches Python and SQL for scraping and analysing city data, with public Jupyter notebooks.

Two courses here teach programming for spatial work: the Spatial Thoughts Python Foundation course and the MIT OpenCourseWare R and GIS course (R rather than Python, but the same audience); both on [[Learning_Resources]]. Pipeline tooling — STAC, Xarray, Zarr, xbatcher — is covered in the cloud pipeline note on [[Data]].

The NUS Data Science for Construction, Architecture and Engineering course covers Python and Pandas from scratch using building data. It is now on YouTube and filed on [[Learning_Resources]].

The ESA CCI Toolbox (`esa-climate-toolbox`) opens about 500 satellite climate data records as xarray and geopandas objects. It is on [[Climate_Change]].

SuperSTAC (multi-catalog STAC search with a GeoParquet cache) is on [[Data]]. Ahrari's PySTAC NDVI and phenology video tutorials are on [[Vegetation_Phenology]]. InSAR.dev is on [[Remote_Sensing]].

## Related topics

Querying the same spatial data in SQL rather than Python — DuckDB spatial joins, indexing and their tradeoffs against PostGIS — is on [[SQL]].

[[Code_Repositories]] · [[Learning_Resources]] · [[Agriculture]] · [[Remote_Sensing]] · [[Urban_Planning]] · [[Deep_Learning]] · [[Learning_Resources]]
