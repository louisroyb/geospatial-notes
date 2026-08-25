# SQL

**Summary**: Notes on SQL for spatial work — query engines, spatial joins, indexing, and the performance tradeoffs between them.
**Last updated**: 2026-08-25

---

- [PostGIS spatial joins in DuckDB](https://www.geomermaids.com/cookbook/duckdb-spatial/): Optimizing DuckDB Spatial Queries. Geomermaids cookbook entry, written from 25 years of PostGIS experience, translating PostGIS spatial join patterns to DuckDB's spatial extension. The argument is that PostGIS is "twenty years mature" with integrated spatial indexes that the planner picks automatically, while DuckDB's spatial extension is "bolted onto a columnar core" — both return identical results, but DuckDB pushes the optimization choice onto you. Practical rules it gives: R-tree indexes only fire for constant-geometry predicates via `RTREE_INDEX_SCAN`, so joins ignore persistent indexes and build a runtime R-tree in `SPATIAL_JOIN` instead; for a handful of probe points run per-point constant queries or `UNION ALL` them rather than a join; for millions of points let `SPATIAL_JOIN` stream; when clipping to a region, resolve the clip geometry once and inline it as literal bbox and polygon constants so [[Data]]'s GeoParquet row-group statistics can prune. Also warns that exactly one spatial predicate per join is allowed — a second one in `WHERE` falls back to `BLOCKWISE_NL_JOIN` and a full scan — and that `SPATIAL_JOIN` is non-spilling, so a large build side is killed by OOM rather than merely slowed. Distance work needs reprojection to a metric CRS before `ST_DWithin`, there is no `<->` nearest-neighbour operator, and `ORDER BY ST_Distance LIMIT` still evaluates every row (DuckDB issue #20113). *Keywords: DuckDB, PostGIS, spatial join, R-tree index, GeoParquet, query optimization*
  - The worked example is a production case from Hagen Hübel: the same 50M-point Canada clip ran 30 minutes and died at 32 GB as a join, but finished in about 2 seconds with the polygon inlined as literals — the point being that this is a question of feasibility, not just speed.
  - Source note: the accompanying text filed this as "Optimizing DuckDB Spatial Queries"; the page's own title is "PostGIS spatial joins in DuckDB". Both are recorded above.
  - Related: [[Data]], [[Code_Repositories]], [[Python]]

## Related topics

Spatial data formats and the cloud-native storage practices these queries read from are on [[Data]]. The Python side of the same work — reading and manipulating spatial data in code rather than SQL — is on [[Python]].

[[Data]] · [[Python]] · [[Code_Repositories]] · [[Geospatial_Platforms]]
