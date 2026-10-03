# Urban Planning

**Summary**: Notes on cities — urban data, urban heat, transport and housing analysis, and the methods planners use on them.
**Last updated**: 2026-10-03

---

- [The changing surface of the world's roads](https://www.nature.com/articles/s41467-026-76234-8): LinkedIn post by Sukanya Randhawa (HeiGIT), 1 September 2026, on the *Nature Communications* paper (DOI 10.1038/s41467-026-76234-8) by S. Randhawa, G. Randhawa, Langer, Andorful, Herfort, Kwakye, Olchik and colleagues. A deep learning model reads road pavedness and width from PlanetScope imagery, covering 95.5% of 9.2 million km of critical arterial roads for 2020 and 2024; nearly half had no prior classification. It also produces a global Humanitarian Passability Score, with case studies in Ghana (governance) and Pakistan (climate vulnerability). Pavedness is offered as *"a high-resolution proxy for economic activity (when compared to traditional proxies such as nightime lights)"*. The data is on OCHA's HDX. *Keywords: road surface, pavedness, PlanetScope, humanitarian passability, HeiGIT, Nature Communications*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/sukanya-randhawa_the-changing-surface-of-the-worlds-roads-share-7500579169467043840-bE8M); see [[LinkedIn]].
  - Related: [[Remote_Sensing]], [[Deep_Learning]], [[Climate_Change]], [[Data]]

- [641 buildings detected in less than 1 minute — AI Segmentation QGIS plugin](https://plugins.qgis.org/plugins/AI_Segmentation/): LinkedIn post by Lilien Auger, co-founder of TerraLab (Paris), 16 July 2026, launching the automatic mode of TerraLab's *AI Segmentation* QGIS plugin. Detection needs no clicks, covers up to 5 km² per run, and *"runs in the cloud"*, so no local models are installed. The demo extracted 600+ buildings on the outskirts of Paris. Install it from the QGIS Plugin Manager by searching "AI Segmentation". According to TerraLab's [docs](https://terra-lab.ai/docs/ai-segmentation), it also extracts trees and vegetation as polygons, supports QGIS 3.22–4, and is free to start. *Keywords: building extraction, QGIS plugin, TerraLab, cloud inference, segmentation, Paris*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/lilien-auger_641-buildings-detected-in-less-than-1-minute-ugcPost-7483547339945791488-V8qW); see [[LinkedIn]]. The post put its how-to guide in the comments, which need a login; the plugin and docs links come from web search.
  - Related: [[Deep_Learning]], [[Machine_Learning]]

- [GlobalBuildingAtlas: An Open Global and Complete Dataset of Building Polygons, Heights and LoD1 3D Models](https://arxiv.org/abs/2506.04106): GlobalBuildingAtlas: An Open Global and Complete Dataset of Building Polygons, Heights and LoD1 3D Models. Zhu, Chen, Zhang, Shi & Wang, arXiv 2506.04106, submitted 4 June 2025. More than 2.75 billion buildings worldwide with polygon boundaries, heights and LoD1 3D models, produced by machine learning pipelines that extract footprints and elevation from PlanetScope imagery, then fused with existing open building datasets under a quality-based strategy. Heights come at 3×3 m against the 90 m of previous global products, with 1.5–8.9 m RMSE depending on continent. *Keywords: building footprints, building height, LoD1 3D, global coverage, PlanetScope, 2.75 billion buildings*
  - Related: [[Data]], [[Remote_Sensing]], [[Benchmark_Datasets]]

- [LinkedIn post: stop using LST to quantify urban heat hazard](https://www.linkedin.com/feed/update/urn:li:activity:7478690057026207745/): Tirthankar "TC" Chakraborty argues that every summer's crop of satellite land surface temperature (LST) maps actively misleads the public about heat hazard. Verbatim from the post: *"The problem is that LST values are almost never equivalent to the temperature of the air around us. LST represents the bulk radiometric 'skin' temperature of whatever a satellite sees, which, in #urban settings, includes an amalgamation of rooftops, tops of tree canopies, asphalt roads, parking lots, etc."* — and, on tree cooling, *"when we use satellites to estimate cooling efficiency of trees, we don't even see the ground underneath the tree. We are basically comparing the LST of tops of tree canopies, which are actively transpiring, against heated #asphalt roads & #parkinglots."* He notes that "this is surface temperature, not air temperature, but…" disclaimers still create an anchoring effect, and that when lived experience fails to match a headline 50°C, trust in the data and the science erodes. Replies push back usefully: Justine Kojo argues the fix is data declaration and stated limitations rather than abandoning LST, especially in data-scarce regions; Chakraborty responds that sparse urban weather stations are by design, that many research sensor networks break meteorological siting protocols, and that city-scale agreement between LST and air temperature patterns does not follow from the aggregate. *Keywords: land surface temperature, urban heat island, air temperature, science communication, tree cooling, heat hazard*
  - Sources cited in the post:
    - [Crowdsourced air temperatures contrast satellite measures of the urban heat island and its mechanisms](https://doi.org/10.1126/sciadv.abb9569) — Venter et al., *Science Advances* 7(22), 2021.
    - [Lower Urban Humidity Moderates Outdoor Heat Stress](https://doi.org/10.1029/2022AV000729) — Chakraborty et al., *AGU Advances* 3(5), 2022.
    - [Daytime cooling efficiencies of urban trees derived from land surface temperature are much higher than those for air temperature](https://doi.org/10.1088/1748-9326/ad30a3) — Du et al., *Environmental Research Letters* 19(4), 2024.
    - [Residential segregation and outdoor urban moist heat stress disparities in the United States](https://doi.org/10.1016/j.oneear.2023.05.016) — Chakraborty et al., *One Earth* 6(6):738–750, 2023.
    - [Satellite-derived Land Surface Temperatures Strongly Mischaracterise Urban Heat Hazard](https://doi.org/10.48550/arXiv.2509.16568) — Zhan, Bechtel, Du, Chakraborty et al., arXiv preprint, 20 September 2025.
  - Related: [[Climate_Change]], [[Remote_Sensing]], [[Data]], [[LinkedIn]]

- [Urban Data Science](https://urbandatascience.its.ucla.edu/): Urban Data Science Course. A hands-on course from UCLA's Luskin School of Public Affairs on scraping, processing, and managing urban data with open-source tools, mainly Python and SQL. Ten modules cover APIs, web scraping, data wrangling, spatial relations, classification, clustering, text parsing, natural language processing, and big data, drawing examples from transit, housing, and equity planning, and it also treats the limits of data science and the biases "big data" can carry. Materials are public as Jupyter notebooks for the video lectures and in-class exercises. *Keywords: urban data, UCLA Luskin, python, jupyter notebooks, transit housing equity, data bias*
  - Related: [[Python]], [[Data]], [[Learning_Resources]], [[Machine_Learning]]

Clayton Miller's NUS course on data science for the built environment (Python, Pandas, data cleaning, visualisation and intro ML) is on [[Learning_Resources]].

AV-QGIS, a QGIS module for Swiss cadastral surveying funded by 60 firms, is on [[Cartography]].

Agent-driven flood exposure of electricity substations (GeoSQL with Overture and DuckDB) is on [[Agentic_Coding]]. Local routing on Overture data is on [[Data]].

## Related topics

Whether Google and Microsoft building footprints actually agree with each other, measured per-polygon with IoU rather than assumed, is on [[Machine_Learning]].

[[Climate_Change]] · [[LinkedIn]] · [[Remote_Sensing]] · [[Land_Cover]] · [[Data]] · [[Benchmark_Datasets]] · [[Python]] · [[Learning_Resources]]
