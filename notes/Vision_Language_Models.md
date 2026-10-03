# Vision Language Models

**Summary**: Notes on vision-language models for Earth observation — captioning, visual question answering, and the datasets that train and test them.
**Last updated**: 2026-10-03

---

- [GroundSet: A Cadastral-Grounded Dataset for Spatial Understanding with Vector Data](https://arxiv.org/abs/2603.14609): LinkedIn post by Roger Ferrod (Université Paris Cité, with Google Research), 28 April 2026. It has 3.8M objects annotated from verified cadastral vector data across 510k high-resolution images and 135 categories, plus an instruction-tuning benchmark of 7 spatial-reasoning tasks. A plain LLaVA baseline trained on it beats remote-sensing-specific and commercial models: *"a standard VLM architecture (like LLaVA) can master complex spatial grounding tasks when trained on dense annotations, without needing complex architectural modifications."* [Data](https://huggingface.co/datasets/RogerFerrod/GroundSet), [model](https://huggingface.co/RogerFerrod/GroundSet-LLaVA-1.6-7B), code at [rogerferrod/GroundSet](https://github.com/rogerferrod/GroundSet) (Apache-2.0). *Keywords: GroundSet, multimodal LLM, spatial grounding, cadastral data, LLaVA, instruction tuning*
  - Source: [LinkedIn post](https://www.linkedin.com/posts/roger-ferrod-926938130_remotesensing-earthobservation-multimodalai-share-7454878375279656960-hwZC); see [[LinkedIn]].
  - Related: [[Benchmark_Datasets]], [[Urban_Planning]], [[Code_Repositories]]

- [RSVLM-QA: A Benchmark Dataset for Remote Sensing Vision Language Model-based Question Answering](https://arxiv.org/abs/2508.07918): RSVLM-QA: A Benchmark Dataset for Remote Sensing Vision Language Model-based Question Answering. Zi, Xiao, Shi, Tao, Li, Braytee & Prasad, arXiv 2508.07918, submitted 11 August 2025. A large VQA benchmark of 13,820 images and 162,373 QA pairs, assembled from WHU, LoveDA, INRIA and iSAID through a dual pipeline — GPT-4.1 prompted to write captions and complex questions, plus automated extraction from segmentation masks to generate object-counting questions. Built to test how well current vision language models actually reason about overhead imagery. *Keywords: VQA benchmark, remote sensing, GPT-4.1 generated, object counting, LoveDA iSAID, model evaluation*
  - Related: [[Benchmark_Datasets]], [[Remote_Sensing]], [[Deep_Learning]]

- [Landsat30-AU: A Vision-Language Dataset for Australian Landsat Imagery](https://arxiv.org/abs/2508.03127): Landsat30-AU: A Vision-Language Dataset for Australian Landsat Imagery. Ma, Li & Taylor, arXiv 2508.03127, submitted 5 August 2025. Pairs 30 m imagery from four Landsat satellites spanning 36+ years over Australia with 196,262 image-caption pairs and 17,725 VQA samples. The point is to bring natural language interaction to long-term, multi-satellite archives at moderate resolution and continental scale, rather than the very high resolution scenes most vision-language work uses. *Keywords: Landsat, image captioning, VQA, Australia, long time series, moderate resolution*
  - Related: [[Benchmark_Datasets]], [[Remote_Sensing]]

## Related topics

[[Remote_Sensing]] · [[Foundation_Models]] · [[Benchmark_Datasets]] · [[Deep_Learning]] · [[Machine_Learning]] · [[LinkedIn]] · [[Code_Repositories]]
