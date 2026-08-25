# Embeddings

**Summary**: Notes on vector embeddings, including Earth observation embedding products and their use in downstream tasks.
**Last updated**: 2026-08-25

---

- [Earth Embeddings as Products: Taxonomy, Ecosystem, and Standardized Access](https://www.linkedin.com/posts/isaaccorley_igarss2026-ieeegrss-remotesensing-share-7493330381442535424-pzzo/): LinkedIn post by Isaac Corley presenting the work at IGARSS 2026 in Washington, D.C. *"We take a look at the rapidly growing ecosystem of Earth observation embeddings: how they differ, how they're distributed, and what's needed to make them easier to discover, compare, and use."* The paper argues that geospatial foundation models are fragmenting, that pre-computed embedding products are a practical *"frozen"* alternative to running the models yourself, and that this ecosystem is fragmented in turn — so it proposes a three-layer taxonomy and extends TorchGeo with a unified API so embeddings can be treated as ordinary standardized geospatial datasets. Fang, Stewart, Corley, Zhu & Azizpour, arXiv [2601.13134](https://arxiv.org/abs/2601.13134), submitted 19 January 2026, revised 24 February 2026. Companion book chapter "Earth Embeddings" (Stewart, Fang, Corley & Zhu, arXiv [2608.03410](https://arxiv.org/abs/2608.03410), 4 August 2026) covers embedding types, coverage and resolution characteristics, applications to land cover, ecological and socioeconomic modelling, and guidance on evaluating and publishing embeddings. [Slides](https://isaac.earth/presentation-igarss-2026-earth-embeddings/). *Keywords: Earth embeddings, taxonomy, TorchGeo API, standardized access, IGARSS 2026, embedding products*
  - This is the constructive counterpart to the "technical debt of Earth embedding products" article on [[Remote_Sensing]] — same diagnosis of a fragmented snowflake ecosystem, but proposing a taxonomy and a concrete TorchGeo API rather than only naming the problem.
  - In the replies, George Percivall asks for a further family of *"explicit feature embeddings"* supporting unsupervised feature identification, pointing at a World2Vec write-up at `georoundtable.xyz`.
  - Adam Stewart and Isaac Corley both appear elsewhere in these notes — the SSL4EO-L sampling note on [[Foundation_Models]], the GeoAI lecture on [[Learning_Resources]], and Corley's own site on [[Community_Resources]].
  - Related: [[Foundation_Models]], [[Remote_Sensing]], [[Deep_Learning]], [[Community_Resources]], [[LinkedIn]]

Earth observation embedding products (Clay, Major TOM, Presto, Tessera, AlphaEarth and others) are discussed in [[Remote_Sensing]], where fragmentation across formats and the pixel-vs-patch cost tradeoff are the main open problems. Embedding-based clustering is one of the field delineation methods used by the `agribound` package noted in [[Agriculture]]. Google's AlphaEarth Foundations embeddings — 64 bands per pixel per year — are available in Earth Engine and introduced by the tutorial series filed under [[Remote_Sensing]]; see [[Google_Earth_Engine]].

## Related topics

[[Remote_Sensing]] · [[Foundation_Models]] · [[Google_Earth_Engine]] · [[Agriculture]] · [[Deep_Learning]] · [[Data]]
