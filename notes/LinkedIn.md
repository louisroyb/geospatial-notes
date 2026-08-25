# LinkedIn

**Summary**: Tracking page for everything in these notes that came from LinkedIn — posts, and articles found through the feed.
**Last updated**: 2026-08-25

---

LinkedIn links rot and usually demand a login, so each entry records the author, what the item argued, and where the full note lives. Where a post was clipped, the raw text is kept in `processed/`.

| Item | Author | Kind | Filed under |
|---|---|---|---|
| [Stop using LST to quantify urban heat hazard](https://www.linkedin.com/feed/update/urn:li:activity:7478690057026207745/) | Tirthankar "TC" Chakraborty | Feed post, clipped | [[Urban_Planning]] |
| [S2GAIA: seasonally aware Sentinel-2 LULC dataset for Greece](https://www.linkedin.com/posts/anastasios-temenos-9849a9208_remotesensing-earthobservation-geoai-share-7495512241295867905-4KIl/) | Anastasios Temenos | Feed post, clipped | [[Land_Cover]] |
| [Earth Embeddings as Products (IGARSS 2026)](https://www.linkedin.com/posts/isaaccorley_igarss2026-ieeegrss-remotesensing-share-7493330381442535424-pzzo/) | Isaac Corley | Feed post, clipped | [[Embeddings]] |
| [NDVI Tree Crown Detection](https://www.linkedin.com/posts/amir-sharifi-313a0160_remotesensing-python-computervision-share-7490188575767154688-zCgy/) | Amir Sharifi | Feed post, clipped | [[Forestry]] |
| [Geospatial Kiro Power Pack](https://www.linkedin.com/posts/johndspence_github-aws-samplessample-geospatial-kiro-power-pack-share-7493481273798127616-Q8Rs/) | John D. Spence | Feed post, clipped | [[Agentic_Coding]] |
| [Open data in GeoLibre — Chrome extension](https://www.linkedin.com/posts/giswqs_geolibre-gis-geospatial-ugcPost-7495471245816430593-HN3T/) | Qiusheng Wu | Feed post, clipped | [[Geospatial_Platforms]] |
| [Use cases for the IoU Calculator QGIS Plugin](https://www.linkedin.com/posts/reut-keller_gis-qgis-remotesensing-ugcPost-7497220741818540033-139y/) | Reut Keller Azulay | Feed post, clipped | [[Machine_Learning]] |
| [Mid-season parcel-based crop type mapping](https://www.linkedin.com/posts/hazhir-bahrami-ab7723104_github-tenor-inrscropmappingproject-share-7497636823557550080-JnDZ/) | Hazhir Bahrami | Feed post, clipped | [[Agriculture]] |
| [Detecting Objects From Text Prompts with RasterFlow and SAM 3](https://wherobots.com/blog/sam3-earth-observation-rasterflow/) | Wherobots | Article shared to the feed | [[Foundation_Models]] |

## Posts

- **[Stop using LST to quantify urban heat hazard](https://www.linkedin.com/feed/update/urn:li:activity:7478690057026207745/)** — Chakraborty's argument that satellite land surface temperature is not air temperature, that headline "55°C in Madrid" maps anchor people into overestimating heat hazard, and that LST also overstates how much trees cool the air. The reply thread is substantive: Justine Kojo pushes for data declaration and stated limitations rather than abandoning LST in data-scarce regions, and Chakraborty answers on weather station siting and on why city-scale agreement does not follow from cross-city aggregates. Five supporting papers are cited in the replies, all verified against Crossref and arXiv — see the full note on [[Urban_Planning]]. The complete clipping is preserved at `processed/Post_LinkedIn_2026-08-24.md`.

- **[S2GAIA: seasonally aware Sentinel-2 LULC dataset for Greece](https://www.linkedin.com/posts/anastasios-temenos-9849a9208_remotesensing-earthobservation-geoai-share-7495512241295867905-4KIl/)** — Temenos announcing the dataset and its paper: 34,030 patches, four seasons a year over 2017–2024, 22 classes, positioned as training data for the Greek National Microsatellite Programme. Note on [[Land_Cover]].
- **[Earth Embeddings as Products (IGARSS 2026)](https://www.linkedin.com/posts/isaaccorley_igarss2026-ieeegrss-remotesensing-share-7493330381442535424-pzzo/)** — Corley presenting a three-layer taxonomy for Earth embedding products and a TorchGeo API for standardized access, plus a companion book chapter. Note on [[Embeddings]].
- **[NDVI Tree Crown Detection](https://www.linkedin.com/posts/amir-sharifi-313a0160_remotesensing-python-computervision-share-7490188575767154688-zCgy/)** — Sharifi open-sourcing a classical NDVI-plus-watershed desktop tool that pre-generates tree crown masks to cut manual labeling time. Note on [[Forestry]].
- **[Geospatial Kiro Power Pack](https://www.linkedin.com/posts/johndspence_github-aws-samplessample-geospatial-kiro-power-pack-share-7493481273798127616-Q8Rs/)** — Spence on geospatial engineering at Amazon Logistics, pointing at kiro.gis.dev, a geospatial pack for AWS's agentic IDE. Note on [[Agentic_Coding]].
- **[Open data in GeoLibre — Chrome extension](https://www.linkedin.com/posts/giswqs_geolibre-gis-geospatial-ugcPost-7495471245816430593-HN3T/)** — Qiusheng Wu announcing the extension on the Chrome Web Store. It scans the page you are on for GeoJSON, GeoParquet, PMTiles, COG and ZIP-wrapped GeoJSON, and opens several at once in GeoLibre; it reads Source Cooperative's embedded inventory so lazy-loaded file listings still enumerate fully. Note on [[Geospatial_Platforms]]. Clipping at `processed/Post_LinkedIn_2026-08-25_b.md`.
- **[Use cases for the IoU Calculator QGIS Plugin](https://www.linkedin.com/posts/reut-keller_gis-qgis-remotesensing-ugcPost-7497220741818540033-139y/)** — Reut Keller Azulay on mapping evaluation metrics instead of tabulating them, using Google vs Microsoft building footprints as the example, and on the distinction between agreement and accuracy when neither dataset is ground truth. Note on [[Machine_Learning]]. Clipping at `processed/Post_LinkedIn_2026-08-25_c.md`.
- **[Mid-season parcel-based crop type mapping](https://www.linkedin.com/posts/hazhir-bahrami-ab7723104_github-tenor-inrscropmappingproject-share-7497636823557550080-JnDZ/)** — Bahrami announcing his *Big Earth Data* paper (DOI 10.1080/20964471.2026.2705616, verified via Crossref). Transformers on Sentinel-1/2 over Quebec hit 0.97 validation accuracy, and — the claim he leads with — transferred to an entirely unseen 2025 season at ~92% with no in-year training data. He also reports AlphaEarth embeddings with plain RF/XGB matching the deep learning models, while noting AlphaEarth is annual and so not a mid-season equivalent. Full note on [[Agriculture]]; the complete clipping is preserved at `processed/Post_LinkedIn_2026-08-25.md`.

## Found through the feed

Items whose note URL carries LinkedIn campaign tracking, meaning they were picked up from the feed rather than posted there.

- **[Detecting Objects From Text Prompts with RasterFlow and SAM 3](https://wherobots.com/blog/sam3-earth-observation-rasterflow/)** — Wherobots running Meta's SAM 3 over NAIP imagery at county scale to detect roofs, containers and tractors from text prompts alone. The original link carried `utm_source=linkedin`; the tracking parameters were stripped when filing. Note on [[Foundation_Models]].

## Related topics

[[Agriculture]] · [[Land_Cover]] · [[Embeddings]] · [[Forestry]] · [[Agentic_Coding]] · [[Geospatial_Platforms]] · [[Machine_Learning]] · [[Urban_Planning]] · [[Foundation_Models]] · [[Community_Resources]] · [[Code_Repositories]]
