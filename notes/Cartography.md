# Cartography

**Summary**: Notes on map projections, map design, and the presentation of spatial information.
**Last updated**: 2026-10-03

---

- [Creating Consistent & Compelling Maps at Mercy Corps — Part 1: The Style Guidelines](https://medium.com/mercy-corps-technology-for-development/creating-consistent-compelling-maps-at-mercy-corps-part-1-the-style-guidelines-640ded396fcf): By Aaron Eubank, Wynnie Gross and Chechi Amah (23 Feb 2026), shared by [Eubank on LinkedIn](https://www.linkedin.com/posts/aaron-eubank-53065b111_creating-consistent-compelling-maps-at-activity-7431770186069815296-wFFR). A humanitarian NGO's cartographic style guide, so that maps by staff and consultants look consistent, on-brand and accessible. It covers boundary styles, label hierarchy, open fonts (Merriweather and League Spartan replacing licensed brand fonts), map-friendly icons, sequential, diverging and qualitative palettes, insets, basemaps and projections, and argues you don't need a north arrow on every map. The challenge was *"making something that was organized and standard enough that the brand shines through on a map made with them, but that is also flexible enough that the person making the map can still make creative decisions."* Importable QGIS and ArcGIS style packages followed ([Part 2](https://medium.com/mercy-corps-technology-for-development/creating-consistent-compelling-maps-at-mercy-corps-part-2-making-the-guide-easy-to-use-for-all-8c13c3fc1bb9)). *Keywords: cartographic style guide, Mercy Corps, colour palettes, typography, QGIS styles, humanitarian maps*
  - See [[LinkedIn]]. Related: [[Geospatial_Platforms]]

- [Cartograms for ecology — R Coding for Ecology chapter](https://doi.org/10.1007/978-3-031-99665-8_14): LinkedIn post by Jakub Nowosad, 15 February 2026, on a chapter by Elisa Marchetto, Sebastian Jeworutzki and Nowosad in Springer's *R Coding for Ecology*, using the `cartogram` package: it *"Demonstrates visualizing sampling bias and ecological variables by resizing regions based on data values."* Code: [RCodingForEcology/cartogram](https://github.com/RCodingForEcology/cartogram), no license. *Keywords: cartogram, R, ecology, sampling bias, thematic mapping, Springer*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/jakub-nowosad-r_rstats-gis-dataviz-activity-7428830757936340992-K_xu); see [[LinkedIn]].
  - Related: [[Learning_Resources]]

- [QTiles 2 — NextGIS raster tiles from QGIS](https://www.linkedin.com/posts/eduard-kazakov-gis_qtiles-20-by-nextgis-ugcPost-7435659871418740736-ZK37): LinkedIn post by Eduard Kazakov (NextGIS), 6 March 2026. The 13-year-old plugin, *"the first (and essentially the only) tool that could generate raster tiles directly from QGIS projects"*, gets a major version: QGIS 4 ready, PMTiles output, extent tools and a zoom-sync button. [nextgis/qgis_qtiles](https://github.com/nextgis/qgis_qtiles) (GPL-2.0; found by lookup, not linked in the post). *Keywords: QTiles, raster tiles, PMTiles, QGIS plugin, NextGIS, web maps*
  - See [[LinkedIn]]. Related: [[Geospatial_Platforms]]

- [Multi-band COGs in deck.gl-raster](https://developmentseed.org/deck.gl-raster/blog/multi-band-cog/): LinkedIn post by Kyle Barron, 16 April 2026: *"Render Sentinel-2 or Landsat COGs directly from your browser, all without a server."* A new MultiCOGLayer combines bands stored as separate COGs, resampling mixed resolutions on the GPU (20 m SWIR to 10 m), with a hosted Sentinel-2 example. [developmentseed/deck.gl-raster](https://github.com/developmentseed/deck.gl-raster), MIT. *Keywords: deck.gl, COG, WebGL, Sentinel-2, client-side rendering, false colour*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/kylebarrongeo_new-in-deckgl-raster-%F0%9D%90%8C%F0%9D%90%AE%F0%9D%90%A5%F0%9D%90%AD%F0%9D%90%A2-%F0%9D%90%9B%F0%9D%90%9A%F0%9D%90%A7%F0%9D%90%9D-ugcPost-7450596515884224512-k57l); see [[LinkedIn]].
  - Related: [[Remote_Sensing]], [[Python]], [[Code_Repositories]]

- [Prompting your way to vectors — locator globes with Claude and D3](https://www.linkedin.com/posts/evan-applegate_maps-cartography-ugcPost-7450582000056401923-pTkN): LinkedIn post by Evan Applegate, 16 April 2026: *"Since Claude knows javascript, it can use D3 to make little locator globes, which can be kicked out to SVG, which I can cute up in Illustrator."* Much faster than building them in QGIS; he asks whether other cartographers are working the same way. *Keywords: locator maps, D3, SVG, Claude, Illustrator, cartographic workflow*
  - See [[LinkedIn]]. Related: [[Agentic_Coding]]

- [BellTopo Sans — a free map font by Sarah Bell](https://sarahbellmaps.com): A free sans-serif map-label typeface (Regular, Italic, Bold, Bold Italic), released in 2020 for personal and commercial use and modelled on the lettering of early USGS topographic maps. In her words, *"the beauty of this typeface that I see on old USGS maps exists within its subtle differences."* It is also available in ArcGIS Online's Map Viewer. The original page now 404s (the site moved to Shopify), so details come from [Lat × Long](https://latlong.blog/2022/10/belltopo-sans.html) and [Esri](https://www.esri.com/arcgis-blog/products/arcgis-online/mapping/the-belltopo-sans-font-is-available-in-arcgis-online-map-viewer-beta). *Keywords: typography, map fonts, BellTopo Sans, USGS, labelling, free font*

- [Interactive story maps with GeoLibre — maritime piracy hotspots](https://www.youtube.com/watch?v=fMXg-y4wg_8): LinkedIn post by Spatial Thoughts, 27 June 2026, on a video tutorial: *"This video covers the full workflow to import, style and analyze a dataset to find maritime piracy hotspots,"* then turns it into an interactive [story map](https://spatialthoughts.github.io/geolibre-maps/maritime-piracy-web.html) exported as standalone HTML. *Keywords: GeoLibre, story maps, hotspot analysis, web maps, tutorial, maritime piracy*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/new-video-tutorial-creating-interactive-share-7476693255422861312-3gPs); see [[LinkedIn]].
  - Related: [[Geospatial_Platforms]], [[Learning_Resources]]

- [GeoProfiler Web App — DEM line and swath profiles](https://geoprofiler.streamlit.app): Reshared on LinkedIn by Somdeep Kundu (17 Jun 2026) from Chandni Verma: *"What started as a Python tool has now evolved into GeoProfiler Web App—an open-source platform for extracting and visualizing topographic profiles from DEMs."* A Streamlit app for line and swath profiles, with hillshade, GeoJSON/Shapefile input with auto-reprojection, and PNG/PDF/CSV export. For river long profiles, cross-sections, faults and watersheds. [chandnivermageo/GeoProfiler-WebApp](https://github.com/chandnivermageo/GeoProfiler-WebApp), MIT. *Keywords: DEM, topographic profile, swath profile, Streamlit, geomorphology, hillshade*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/somdeep-kundu_great-pwa-must-give-it-a-try-ugcPost-7473088709224165377-hF0x); see [[LinkedIn]].
  - Related: [[Python]]

- [Open-source mapping tools from State of the Map 2026](https://2026.stateofthemap.org/programme/): LinkedIn post by Venkanna Babu Guthula, 31 August 2026, listing tools he picked up at the OSM community's Paris conference: [Panoramax](https://panoramax.fr/) (open street-level imagery), [GeoDesk](https://www.geodesk.com/) (OSM toolkit), [OpenHistoricalMap](https://www.openhistoricalmap.org/), [Mapterhorn](https://mapterhorn.com/) (*"Public terrain tiles for interactive web map visualisations"*), [OSM for Cities](https://osmforcities.org/), MapLibre, and routing engines MOTIS ([motis-project/motis](https://github.com/motis-project/motis), MIT, 598 stars), Transitous and OSRM. The next State of the Map is in Bogotá. *Keywords: OpenStreetMap, State of the Map, Panoramax, Mapterhorn, MapLibre, routing*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/venkanna37_i-would-like-to-share-a-few-open-source-mapping-share-7500228539795800064-l3nd); see [[LinkedIn]].
  - Related: [[Data]], [[Urban_Planning]], [[Community_Resources]]

- [Top ten QGIS plugins I can't live without](https://www.linkedin.com/posts/helenmckenzie003_qgis-gis-geospatial-share-7511015796303765504-3xRj): LinkedIn post by Helen McKenzie (CARTO), 30 September 2026: *"QGIS out of the box is already a ridiculous piece of software for £0... it would actually be ridiculous for £5,000."* Her ten:
  - QuickOSM (OSM data without Overpass queries)
  - QuickMapServices (one-click basemaps)
  - Chainage (points at intervals along a line)
  - cartogram3
  - CARTO (live cloud editing; she discloses she works there)
  - qgis2web (no-code Leaflet/OpenLayers maps)
  - DataPlotly (charts linked to the map selection)
  - H3 Toolkit (pairs with the Density Analysis plugin)
  - Bivariate Renderer
  - Terrain Shading (ambient occlusion, texture shading)
  - *Keywords: QGIS plugins, QuickOSM, qgis2web, DataPlotly, H3, terrain shading*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/helenmckenzie003_qgis-gis-geospatial-share-7511015796303765504-3xRj); see [[LinkedIn]]. The note arrived as an `lnkd.in/p/` share link.
  - Related: [[Geospatial_Platforms]], [[Data]]

- [GIS & Cartography student portfolios — University College Utrecht](https://jakub8markech-gif.github.io/GIS_web/elevation.html): LinkedIn post by Britta Ricker, 19 July 2026. In a two-week GIS summer course, *"students built personal websites to showcase the six assignments they completed throughout the course"*, using open data and mostly open-source tools, though *"Most of them had little or no prior web design experience"*. The examples are all GitHub Pages sites: a 3D flood model of Utrecht (linked above, built from Hans van der Kwast's tutorials), an [animated Amsterdam map](https://beatrizdapsoares24.github.io/page2.html), an [interactive DEM](https://21annaw.github.io/100annaw/elevation_map.html), [vegetation change in Beirut](https://alice772.github.io/maps-gallery.html) and [land-use classification](https://jakub8markech-gif.github.io/GIS_web/classification.html). *Keywords: GIS teaching, student portfolios, GitHub Pages, web maps, open data, Utrecht*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/brittaricker_one-of-my-favorite-parts-of-teaching-gis-share-7484495600315506688-DlGn); see [[LinkedIn]]. LinkedIn served an unrelated post at the slug URL; the real post was read from its `feed/update` URL.
  - Related: [[Learning_Resources]]

- [Styling QGIS legends with Claude Design](https://www.linkedin.com/posts/gopangokul_qgis-claude-qgis-ugcPost-7477656983580540928-YA5T): LinkedIn post by Gokul Gopan, 30 June 2026. Default QGIS legends look plain, and styling them meant writing CSS inside an HTML frame. *"Used #Claude Design instead this time — described what I wanted, got a few options, picked one and pasted the html into QGIS. No CSS needed."* *Keywords: QGIS legend, map layout, HTML frame, Claude Design, AI-assisted design, cartography*
  - See [[LinkedIn]]. The post has no outbound links.
  - Related: [[Agentic_Coding]]

- [QGIS specialist module for cadastral surveying](https://spatialists.ch/posts/2026/07/21-qgis-specialist-module-for-cadastral-surveying/): A Spatialists post by Ralph Straumann, 21 July 2026. A consortium of 60 Swiss firms has funded AV-QGIS, a QGIS extension for official Swiss cadastral surveying (*amtliche Vermessung*) built on the DMAV 1.0 data model, and the project is now being implemented. Basic data updating is due in January 2028 and the full rollout by mid-2028. New members can still join the committee on favourable terms until September 2026 (contact info@av-qgis.ch). Straumann calls it a sign of *"competition and sovereign solutions"* and *"a welcome sign"* for open-source alternatives in surveying software. *Keywords: QGIS, cadastral surveying, Switzerland, DMAV, open source, AV-QGIS*
  - Related: [[Urban_Planning]], [[Data]]

- [Equal Earth map](https://equal-earth.com/index.html): Equal earth map. Tom Patterson's equal-area world projection and the map series built on it, made because conventional projections distort relative size — the site's example is that Africa is 14 times larger than Greenland, which common projections hide. The projection keeps areas true while staying visually agreeable, and the maps are designed with readable type and clear hierarchy. Free digital maps come in three regional centrings (Africa/Europe, the Americas, East Asia/Australia) at 55" × 29" and 350 DPI, plus layered Adobe Illustrator files, outline variants and 20+ language versions, all released to the public domain; printed wall maps are sold through Longitude Maps. *Keywords: equal-area projection, Tom Patterson, map design, public domain, world map, area distortion*
  - Related: [[Data]]

## Related topics

[[Data]] · [[Remote_Sensing]] · [[Geospatial_Platforms]] · [[Urban_Planning]] · [[LinkedIn]] · [[Agentic_Coding]] · [[Learning_Resources]]
