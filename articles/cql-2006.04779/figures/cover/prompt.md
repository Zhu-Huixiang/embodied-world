# Built-in imagegen cover prompt (exact original call)

```javascript
// @exec: {"yield_time_ms": 120000, "max_output_tokens": 500}
const prompt="Use case: illustration-story. Create a premium Chinese science editorial cover for CQL conservative offline reinforcement learning, wide aspect 2.35:1. Cream background, navy typography, teal and coral visual accents. Main title exact Chinese: “没试过的动作凭什么高分” (large centered upper). Subtitle “CQL · NeurIPS 2020”. Visual metaphor below title: a small teal solid stack of archived action cards beside a wildly tall coral score pillar with a faint cloud-shaped top; a mechanical calibration press gently compresses the inflated top while the archive remains intact. Elegant dimensional paper and brushed metal illustration, restrained warm studio lighting. This is an abstract conceptual illustration, no realistic robot experiment, no graphs with fabricated results, no people, no logos. Essential title and two subjects inside center square safe area so square crop remains readable; outer width contains only soft decorative breathing space. No AI/DrawPaper/generated labels, no watermark. Chinese text spelled exactly. Clear hierarchy at phone size, do not include extra text or equations.";
const r=await tools.image_gen__imagegen({prompt,transparent_background:false});store("cql_covergen",r);generatedImage(r);

```
