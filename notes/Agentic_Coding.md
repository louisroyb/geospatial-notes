# Agentic Coding

**Summary**: Notes on AI agents that write code or drive tools, and the ecosystems built around them.
**Last updated**: 2026-10-03

---

- [QGIS and AI — automating spatial analysis with the QGIS MCP server](https://courses.spatialthoughts.com/advanced-qgis.html#qgis-and-ai): LinkedIn post by Spatial Thoughts, 29 September 2026. A new free module in the Advanced QGIS course drives QGIS through the QGIS MCP server and AI agents. Its main asset is *"the custom project instructions (CLAUDE .md/AGENTS .md) file that captures the best practices for using QGIS's powerful processing framework and adds guardrails for the agent"*. [Video walkthrough](https://www.youtube.com/watch?v=r-hPfRtgo2U). *Keywords: QGIS MCP, AI agents, CLAUDE.md, guardrails, processing framework, Spatial Thoughts*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/qgis-and-ai-automating-spatial-analysis-share-7510686340418793473-gKW8); see [[LinkedIn]].
  - The same instruction-file pattern this vault uses (`CLAUDE.md`). Related: [[Cartography]], [[Learning_Resources]]

- [ai-job-search — a Claude Code job application pipeline](https://github.com/MadsLorentzen/ai-job-search): LinkedIn post by Linas Beliūnas, 6 July 2026, on an open-source framework by Mads Lorentzen, a data scientist with a geophysics background. `/scrape` searches job boards and ranks postings against your profile. `/apply <url>` writes a tailored LaTeX CV and cover letter, which a second reviewer agent critiques before the first agent revises and compiles the PDFs. *"The entire system lives in plain Markdown files - your profile, writing rules, evaluation criteria, templates, and interview prep notes."* It needs a Claude subscription plus Python, Bun and LaTeX, and has Danish job portals built in. MIT, ~44.7k stars. *Keywords: Claude Code, job applications, agent pipeline, reviewer agent, markdown state, open source*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/linasbeliunas_a-scientist-in-denmark-figured-out-how-to-share-7479975129024888833-bJym); see [[LinkedIn]]. The post itself links only to the author's newsletter; the repo link comes from the comments.
  - Same plain-Markdown-files-plus-agent pattern as this vault. Other career material is on [[Careers_and_Research]].
  - Related: [[Careers_and_Research]], [[Code_Repositories]]

- [50 LLM resources to future-proof your career](https://www.linkedin.com/posts/sairam-sundaresan_the-tech-landscape-just-shifted-again-share-7481642807405760512-dcwM): LinkedIn post by Sairam Sundaresan, 11 July 2026: *"The tech landscape just shifted. Again."* A list of about 50 links on LLMs and AI agents:
  - **Repos**: [NirDiamant/GenAI_Agents](https://github.com/NirDiamant/GenAI_Agents), [microsoft/ai-agents-for-beginners](https://github.com/microsoft/ai-agents-for-beginners), [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide), [AGI-Edgerunners/LLM-Agents-Papers](https://github.com/AGI-Edgerunners/LLM-Agents-Papers).
  - **Guides**: Anthropic's [Building effective agents](https://www.anthropic.com/engineering/building-effective-agents) and [Claude Code best practices](https://www.anthropic.com/engineering/claude-code-best-practices), Google's [agents whitepaper](https://www.kaggle.com/whitepaper-agents), OpenAI's [practical guide to building agents](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf).
  - **Papers**: [ReAct](https://arxiv.org/abs/2210.03629), [Generative Agents](https://arxiv.org/abs/2304.03442), [Chain-of-Thought](https://arxiv.org/pdf/2201.11903), [Tree of Thoughts](https://arxiv.org/pdf/2305.10601), Toolformer, Reflexion, and a [RAG survey](https://arxiv.org/pdf/2312.10997).
  - **Courses and books**: the [Hugging Face Agents Course](https://huggingface.co/learn/agents-course/en/unit0/introduction), 13 DeepLearning.AI short courses (MCP, agent memory, RAG, evaluation, multi-agent systems), and books including [Understanding Deep Learning](https://udlbook.github.io/udlbook/) (free online).
  - Plus 8 videos and 6 newsletters; the full list is in the post.
  - *Keywords: LLM agents, reading list, ReAct, RAG, prompt engineering, courses*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/sairam-sundaresan_the-tech-landscape-just-shifted-again-share-7481642807405760512-dcwM); see [[LinkedIn]].
  - Related: [[Learning_Resources]], [[Code_Repositories]], [[Deep_Learning]]

- [Geospatial Kiro Power Pack](https://www.linkedin.com/posts/johndspence_github-aws-samplessample-geospatial-kiro-power-pack-share-7493481273798127616-Q8Rs/): LinkedIn post by John D. Spence, a Geospatial Data Engineer at Amazon Logistics, opening with the claim that *"Amazon is a #geospatial first company."* Most of the post describes the work — automated pipelines built on AWS services alongside Esri ArcGIS platforms and Apache Sedona, ingesting parcel boundaries, zoning constraints, drive-time coverage, shipping lanes and transport connectivity, then publishing refined layers across AWS, ArcGIS Online, ArcGIS Enterprise and ArcGIS Location Platform for real estate and site-planning teams — and notes a *"small but mighty army"* of geospatial practitioners across AWS, Amazon Leo, Worldwide Operations Security and Whole Foods Market. The reusable artefact is the pointer at the end: [kiro.gis.dev](https://kiro.gis.dev), a geospatial power pack for Kiro, AWS's agentic IDE. Repository: [aws-samples/sample-geospatial-kiro-power-pack](https://github.com/aws-samples/sample-geospatial-kiro-power-pack), Python, MIT-0, last pushed July 2026. *Keywords: Kiro, agentic IDE, AWS, geospatial power pack, Esri ArcGIS, Apache Sedona*
  - **Second announcement** ([LinkedIn, Taylor Teske (AWS), 22 June 2026](https://www.linkedin.com/posts/taylor-teske-b37aaa71_aws-kiro-geoai-share-7474890479772258304-v1qq)), the day the repo was created. Teske built the pack with Chris Stoner. The post describes three areas: data access (STAC, vector, geocoding, terrain, weather, biodiversity), processing (CRS transforms, spatial SQL, raster, point clouds) and GeoAI (foundation-model embeddings, segmentation, vector search), plus agent "Skills & Steering". *"21 modular packages, 46 tools — install only what you need."* The README now lists 56 tools. It was the companion to an "AIDLC in GeoAI" session at Esri UC 2026 (14 July, San Diego), which has now passed. Merged here rather than filed twice; see [[LinkedIn]].
  - Same shape as the skills.sh directory below — packaged domain knowledge dropped into a coding agent — but specific to geospatial work rather than general-purpose.
  - Mostly a first-person account of a role at Amazon; the durable part is the power pack and the AWS-plus-Esri-plus-Sedona stack it targets.
  - Related: [[Geospatial_Platforms]], [[Code_Repositories]], [[Data]], [[LinkedIn]]

- [skills.sh](https://www.skills.sh/): Skill repository. "The Open Agent Skills Directory", made by Vercel. Skills are described as "reusable capabilities for AI agents. Install them with a single command to enhance your agents with access to procedural knowledge" — installed via `npx skills add <owner/repo>` and supported across Claude Code, Cursor, GitHub Copilot, Gemini and a dozen-plus other agents. Carries a leaderboard tracking over 1.3 million skill installs, with Vercel Labs, Matt Pocock, Microsoft Azure and Anthropic among top contributors, plus docs, security audits and topic browsing. Open source on GitHub. *Keywords: agent skills, Vercel, directory, Claude Code, procedural knowledge, npx install*
  - Related: [[Code_Repositories]]

## Related topics

Google's Agent Development Kit example agents for Earth Engine — the EUDR and ForestWise agents — are on [[Google_Earth_Engine]].

[[Google_Earth_Engine]] · [[Code_Repositories]] · [[Machine_Learning]] · [[Careers_and_Research]] · [[Learning_Resources]]
