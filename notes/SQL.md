# SQL

**Summary**: Notes on SQL for spatial work — query engines, spatial joins, indexing, and the performance tradeoffs between them.
**Last updated**: 2026-10-03

---

- [Learn spatial databases with PostGIS and QGIS — GIS Schools](https://www.youtube.com/playlist?list=PLumZ7YQFbxIw5WJFXFgL-rCoDCE8O9mmw): A free 21-video playlist covering PostgreSQL/PostGIS installation, shapefile import and export, SQL basics through JOINs and CASE, SRIDs and geometry vs geography, spatial joins and indexes, and editing from QGIS. *Keywords: PostGIS, spatial SQL, QGIS DB Manager, indexes, spatial joins, YouTube*
  - Related: [[Learning_Resources]]

- [Spatial Data Management with DuckDB — Qiusheng Wu's book](https://duckdb.gishub.org): LinkedIn post, 3 November 2025, announcing *Spatial Data Management with DuckDB: From SQL Basics to Advanced Geospatial Analytics*, based on his University of Tennessee course ([geog-414](https://geog-414.gishub.org)). It is aimed at GIS analysts, data scientists and spatial developers, and *"all code examples will be freely available on GitHub"*: [giswqs/duckdb-spatial](https://github.com/giswqs/duckdb-spatial) (CC0). *Keywords: DuckDB, spatial SQL, book, GeoParquet, Qiusheng Wu, course*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/giswqs_table-of-contents-ugcPost-7391097247792263169-vEO4); see [[LinkedIn]].
  - Related: [[Learning_Resources]], [[Data]], [[Code_Repositories]]

- [GeoSQL — learn PostgreSQL & PostGIS with geoscience data](https://siddhi1991.github.io/GeoSQL-learning/): LinkedIn post by Siddhi Garg, 14 February 2026, on a free interactive tutorial that swaps the usual employee tables for earthquakes, rock samples, mineral deposits, seismic stations and geological formations. It runs from SELECT and joins to PostGIS spatial queries, with an in-browser editor and solutions at each step: *"It is the resource I wish I had when I was learning spatial SQL."* [siddhi1991/GeoSQL-learning](https://github.com/siddhi1991/GeoSQL-learning), no license. *Keywords: PostGIS, spatial SQL, interactive tutorial, geoscience, PostgreSQL, beginners*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/activity-7428585125812174848-h871); see [[LinkedIn]].
  - Related: [[Learning_Resources]]

- [Complete Microsoft SQL Server Database Administration (Udemy)](https://www.udemy.com/course/complete-microsoft-sql-server-database-administration-course/): A learner's review on LinkedIn by Céphas Mwimangire (1 Apr 2026) of a 32-hour paid course covering RDBMS basics, indexing, performance tuning, security, high availability and backups, with AI-assisted query writing: *"a solid foundation for a long-term career in database administration."* Not spatial, but the database-admin side of running PostGIS or SQL Server spatial in production. *Keywords: SQL Server, database administration, indexing, performance, Udemy, career*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/c%C3%A9phas-mwimangire-543302133_sql-databaseadministration-learningjourney-share-7445193430374277120-R8JC); see [[LinkedIn]].
  - Related: [[Careers_and_Research]], [[Learning_Resources]]

- [PostGIS spatial joins in DuckDB](https://www.geomermaids.com/cookbook/duckdb-spatial/): Optimizing DuckDB Spatial Queries. Geomermaids cookbook entry, written from 25 years of PostGIS experience, translating PostGIS spatial join patterns to DuckDB's spatial extension. The argument is that PostGIS is "twenty years mature" with integrated spatial indexes that the planner picks automatically, while DuckDB's spatial extension is "bolted onto a columnar core" — both return identical results, but DuckDB pushes the optimization choice onto you. Practical rules it gives: R-tree indexes only fire for constant-geometry predicates via `RTREE_INDEX_SCAN`, so joins ignore persistent indexes and build a runtime R-tree in `SPATIAL_JOIN` instead; for a handful of probe points run per-point constant queries or `UNION ALL` them rather than a join; for millions of points let `SPATIAL_JOIN` stream; when clipping to a region, resolve the clip geometry once and inline it as literal bbox and polygon constants so [[Data]]'s GeoParquet row-group statistics can prune. Also warns that exactly one spatial predicate per join is allowed — a second one in `WHERE` falls back to `BLOCKWISE_NL_JOIN` and a full scan — and that `SPATIAL_JOIN` is non-spilling, so a large build side is killed by OOM rather than merely slowed. Distance work needs reprojection to a metric CRS before `ST_DWithin`, there is no `<->` nearest-neighbour operator, and `ORDER BY ST_Distance LIMIT` still evaluates every row (DuckDB issue #20113). *Keywords: DuckDB, PostGIS, spatial join, R-tree index, GeoParquet, query optimization*
  - The worked example is a production case from Hagen Hübel: the same 50M-point Canada clip ran 30 minutes and died at 32 GB as a join, but finished in about 2 seconds with the polygon inlined as literals — the point being that this is a question of feasibility, not just speed.
  - Source note: the accompanying text filed this as "Optimizing DuckDB Spatial Queries"; the page's own title is "PostGIS spatial joins in DuckDB". Both are recorded above.
  - Related: [[Data]], [[Code_Repositories]], [[Python]]

GeoSQL, a coding-agent skill that writes spatial SQL against DuckDB, PostGIS or BigQuery and checks the result on a map, is on [[Agentic_Coding]].

## Related topics

Spatial data formats and the cloud-native storage practices these queries read from are on [[Data]]. The Python side of the same work — reading and manipulating spatial data in code rather than SQL — is on [[Python]].

[[Data]] · [[Python]] · [[Code_Repositories]] · [[Geospatial_Platforms]] · [[Agentic_Coding]]
