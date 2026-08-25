# Agentic Coding

**Summary**: Notes on AI agents that write code or drive tools, and the ecosystems built around them.
**Last updated**: 2026-08-25

---

- [Geospatial Kiro Power Pack](https://www.linkedin.com/posts/johndspence_github-aws-samplessample-geospatial-kiro-power-pack-share-7493481273798127616-Q8Rs/): LinkedIn post by John D. Spence, a Geospatial Data Engineer at Amazon Logistics, opening with the claim that *"Amazon is a #geospatial first company."* Most of the post describes the work — automated pipelines built on AWS services alongside Esri ArcGIS platforms and Apache Sedona, ingesting parcel boundaries, zoning constraints, drive-time coverage, shipping lanes and transport connectivity, then publishing refined layers across AWS, ArcGIS Online, ArcGIS Enterprise and ArcGIS Location Platform for real estate and site-planning teams — and notes a *"small but mighty army"* of geospatial practitioners across AWS, Amazon Leo, Worldwide Operations Security and Whole Foods Market. The reusable artefact is the pointer at the end: [kiro.gis.dev](https://kiro.gis.dev), a geospatial power pack for Kiro, AWS's agentic IDE. Repository: [aws-samples/sample-geospatial-kiro-power-pack](https://github.com/aws-samples/sample-geospatial-kiro-power-pack), Python, MIT-0, last pushed July 2026. *Keywords: Kiro, agentic IDE, AWS, geospatial power pack, Esri ArcGIS, Apache Sedona*
  - Same shape as the skills.sh directory below — packaged domain knowledge dropped into a coding agent — but specific to geospatial work rather than general-purpose.
  - Mostly a first-person account of a role at Amazon; the durable part is the power pack and the AWS-plus-Esri-plus-Sedona stack it targets.
  - Related: [[Geospatial_Platforms]], [[Code_Repositories]], [[Data]], [[LinkedIn]]

- [skills.sh](https://www.skills.sh/): Skill repository. "The Open Agent Skills Directory", made by Vercel. Skills are described as "reusable capabilities for AI agents. Install them with a single command to enhance your agents with access to procedural knowledge" — installed via `npx skills add <owner/repo>` and supported across Claude Code, Cursor, GitHub Copilot, Gemini and a dozen-plus other agents. Carries a leaderboard tracking over 1.3 million skill installs, with Vercel Labs, Matt Pocock, Microsoft Azure and Anthropic among top contributors, plus docs, security audits and topic browsing. Open source on GitHub. *Keywords: agent skills, Vercel, directory, Claude Code, procedural knowledge, npx install*
  - Related: [[Code_Repositories]]

## Related topics

Google's Agent Development Kit example agents for Earth Engine — the EUDR and ForestWise agents — are on [[Google_Earth_Engine]].

[[Google_Earth_Engine]] · [[Code_Repositories]] · [[Machine_Learning]]
