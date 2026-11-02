# DINOv2 DrawPaper scientific and layout specification

Source: arXiv 2304.07193v2 (2024-02-02), TMLR 01/2024 author manuscript, 32 pages. Core sources: §3 pp4–5, §4 pp5–6, §5 pp6–7, §6 pp8–10, §7 pp11–18, Appendix A/B pp29–31.

Regions A–D follow data curation, joint self-supervised pretraining, distillation, frozen downstream use. No language encoder, text-target loss, robot action head, 3D world model, or closed-loop control is implied.

- A: image seeds and raw pool; dedup, similarity retrieval and balancing to LVD-142M. Figure avoids incompatible raw-pool-count descriptions between body and appendix. Retrieval encoder is their self-supervised ViT-H/16; visual labels/captions are not pretraining targets.
- B: student masked global images and local crops; teacher intact global crops. Two independent DINO/iBOT projection heads. DINO matches image-level CLS distributions across different views. iBOT matches same-position masked patches. Teacher gets SK targets (3 normalization iterations); student softmax. Student updated by gradients; teacher updated by EMA. KoLeo acts on normalized CLS and encourages feature spread, not class separation labels.
- C: trained ViT-g teacher is frozen. Small S/B/L students train; another EMA of each student is the final model. No masking/stochastic depth; iBOT on both global crops. This frozen teacher is distinct from B's moving teacher.
- D: image produces global z and local f_i. Classification/retrieval and dense prediction consume those features; downstream supervised heads are trained, backbone remains frozen. Linear depth head includes CLS. 224/14→256 patch and ViT-g d1536 are source-backed shape illustrations, not a claim that every evaluation uses224.

Built-in imagegen provides bird/scene photo-card illustrations, transformer tower material, feature-spread sphere and encoder-family symbols. The draft contains illustrative arrows, therefore the final TeX uses only cropped illustration viewports and replaces the complete dataflow, labels and math with vector drawing. The final is mixed raster/vector, not an all-vector redraw. All four regions visibly retain draft artwork. Output PNG is rendered from the checked PDF, not the unedited draft.

The diagram supports the explanation rather than asserting robot ability. On mobile, the text provides the detailed equations and task conditions; the full-resolution diagram remains available for enlargement.
