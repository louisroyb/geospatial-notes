# Python

**Summary**: Notes on Python packages and libraries, especially for geospatial and scientific work.
**Last updated**: 2026-08-24

---

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

## Related topics

[[Code_Repositories]] · [[Learning_Resources]] · [[Agriculture]] · [[Remote_Sensing]] · [[Urban_Planning]] · [[Deep_Learning]] · [[Learning_Resources]]
