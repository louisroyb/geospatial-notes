# Vegetation Phenology

**Summary**: Notes on seasonal vegetation dynamics — growing season timing, productivity metrics, and the software and products that derive them from satellite time series.
**Last updated**: 2026-08-24

---

- [Welcome to the TIMESAT pages!](https://web.nateko.lu.se/timesat/timesat.asp): A software package to analyse time-series of satellite sensor data. Developed at Lund University and Malmö University, TIMESAT extracts vegetation seasonality from satellite time series (AVHRR NDVI, Terra/MODIS and others) by smoothing and curve fitting — Savitzky-Golay filters, asymmetric Gaussians, and double logistic functions — then deriving phenological parameters from the fitted curves. Version 3.3 is current and free for non-commercial academic research; version 4 is in development to handle irregular time steps such as Sentinel-2. *Keywords: TIMESAT, phenology, curve fitting, Savitzky-Golay, NDVI time series, seasonality metrics*
  - Related: [[Remote_Sensing]], [[Agriculture]]

- [Global Land Surface Phenology 2024 product available](https://land.copernicus.eu/en/news/global-land-surface-phenology-2024-product-available): Copernicus Land Monitoring Service's Vegetation suite. The 2024 edition of the global Land Surface Phenology suite, at 300 m resolution, giving vegetation phenology and productivity for up to two growing seasons per year. Each season carries 13 parameters — start, peak and end dates, duration, values at those points, amplitude, productivity, and rates of change. Data for 2023 and 2024 are available through the CLMS catalogue and data viewer. *Keywords: land surface phenology, Copernicus, CLMS, 300m global, growing season, productivity metrics*
  - Related: [[Remote_Sensing]], [[Data]]

Seasonality is also the training signal behind agricultural foundation models — Time2Agri builds its self-supervised pretext tasks on it, and phenology estimation is one of the tasks CropFM is proposed for; see [[Agriculture]] and [[Foundation_Models]].

## Related topics

[[Remote_Sensing]] · [[Agriculture]] · [[Foundation_Models]] · [[Climate_Change]] · [[Data]]
