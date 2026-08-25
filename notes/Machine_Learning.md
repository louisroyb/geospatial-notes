# Machine Learning

**Summary**: Notes on machine learning methods and their application to geospatial and urban problems.
**Last updated**: 2026-08-25

---

- [What are the use cases for the IoU Calculator QGIS Plugin?](https://www.linkedin.com/posts/reut-keller_gis-qgis-remotesensing-ugcPost-7497220741818540033-139y/): LinkedIn post by Reut Keller Azulay on why spatial-agreement metrics belong on a map rather than in a table. IoU is defined as *"IoU = Intersection / Union"*, scored 0 to 1, where *"1 -> perfect overlap"* and *"0 -> no overlap"*. The stated main use case is evaluating feature extraction models: *"I was already calculating these metrics with Python, but I wanted to go beyond the numbers. I wanted to see the results spatially. Where does the model perform well? Where does it struggle? Is there a spatial pattern?"* The worked example compares Google and Microsoft open building footprints over the same area — blue for Microsoft, orange for Google, black for overlap, then each polygon recoloured by its own IoU score from blue for high agreement to red for low. She is careful about what that does and does not show: *"Neither is ground truth. We don't know whether they were generated from the same imagery, acquisition date, or methodology. So this comparison cannot tell us which dataset is more accurate. But it can tell us how much they agree."* The closing point is the general one — *"Don't just calculate the score. See where it comes from."* — and where one side genuinely is ground truth, the same view exposes which building types a model fails on. The plugin also carries area-based and object-based metrics beyond IoU. *Keywords: IoU, model evaluation, QGIS plugin, building footprints, spatial agreement, error analysis*
  - Agreement is not accuracy: two independent models agreeing tells you about shared method or shared imagery as much as about correctness. Worth holding next to the global building datasets on [[Urban_Planning]], where the same Google and Microsoft footprints get used as though interchangeable.
  - The post carries no link to the plugin, and as of 2026-08-25 no "IoU Calculator" plugin appears in the QGIS plugin repository or in a GitHub search, so no repository is recorded on [[Code_Repositories]].
  - Related: [[Urban_Planning]], [[Deep_Learning]], [[Benchmark_Datasets]], [[LinkedIn]]

Machine learning shows up throughout these notes rather than on its own. EO College's "Introduction to Machine Learning for Earth Observation" and the Copernicus "AI for Earth Monitoring" MOOC are listed under [[Remote_Sensing]]; classification, clustering and NLP modules make up much of the UCLA course on [[Urban_Planning]]. For architecture-level notes see [[Deep_Learning]], for pretrained backbones see [[Foundation_Models]], and for representation learning see [[Embeddings]]. Benchmark competitions such as the Zindi Côte d'Ivoire crop classification challenge, and the labeled datasets the Lacuna Fund pays for, are both on [[Agriculture]]. The Forest Data Partnership's commodity probability models in [[Forestry]] are a worked example of ML products published as map layers.

Microsoft's 26-lesson classic ML curriculum and the free Earth Lab courses are on [[Learning_Resources]]; the GeoSpatial ML newsletter is on [[Community_Resources]].

## Related topics

[[Deep_Learning]] · [[Foundation_Models]] · [[Community_Resources]] · [[Embeddings]] · [[Remote_Sensing]] · [[Urban_Planning]] · [[Agriculture]] · [[Forestry]] · [[Learning_Resources]]
