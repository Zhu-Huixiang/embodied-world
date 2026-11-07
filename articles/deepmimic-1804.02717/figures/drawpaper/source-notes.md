# DrawPaper source notes

## Original paper

- URL: https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf
- PDF SHA-256: `c57cdd325b4bb921d95a5feb2742bdf016d48412ed969ea5f4ee2fe05e22db30`
- Source identity: author-hosted TOG2018 final paper,18pages with supplementary material; no claim of arXiv byte equivalence.
- Scientific regions and locators are in `figure-spec.md`.

## Built-in image generation

- Draft: `deepmimic-imagegen-draft.png`,1024×1536, SHA-256 `04974fac12ef073e0b5852cc9cfdffce199dfcfacd1ce525bf1bfe99130b8782`.
- Exact prompt: `imagegen-prompt.md`, SHA-256 `2651e185f502c42511caf7866a27f329f4c3a43b59c4afe24161010727800e4d`.
- Built-in generation artifact: `exec-890c665a-2553-4b4c-844a-b90c73e60a19.png`.
- The generated draft is retained unchanged. No external paid image service was used.
- The incorrect generated E explanation about splitting long skills was cropped out and replaced by the paper's three parallel options. Generated feedback routing was discarded and reconstructed in TikZ. Reference initializes simulation and supplies reward comparison; it does not supply target poses to B at every step.

## Actual draft illustrations retained in final

Coordinates use the unchanged draft's1024×1536pixel top-left system. TeX `art` converts these to graphicx trim coordinates, preserving source aspect ratio. Labels and inter-module arrows are independently typeset.

| x | y | width | height | final x bp | final y bp | final width bp |
| --- | --- | --- | --- | --- | --- | --- |
| 263 | 156 | 742 | 236 | 24 | 107 | 291 |
| 269 | 452 | 137 | 151 | 29 | 334 | 65 |
| 566 | 424 | 223 | 185 | 127 | 329 | 86 |
| 837 | 412 | 165 | 200 | 244 | 330 | 66 |
| 276 | 678 | 166 | 124 | 27 | 668 | 84 |
| 449 | 643 | 344 | 188 | 152 | 661 | 164 |
| 300 | 928 | 175 | 195 | 28 | 919 | 84 |
| 493 | 930 | 264 | 185 | 155 | 922 | 153 |
| 257 | 1335 | 267 | 123 | 30 | 1415 | 99 |
| 548 | 1320 | 202 | 155 | 30 | 1507 | 99 |
| 792 | 1314 | 208 | 185 | 30 | 1613 | 97 |

## Exact layout and rendering

- Main source: `deepmimic-overview.tex`; dependency: `deepmimic-imagegen-draft.png`.
- Final PDF: `deepmimic-overview.pdf`; final PNG: `deepmimic-overview.png`,1020×5220pixels,3pixels per bp.
- Compile from this directory with XeLaTeX; uses Arial, STHeiti Light/Medium from the macOS font directory. These fonts are runtime dependencies and are not redistributed.
- All formulas are TeX. The full diagram is340bp wide, so its13–17bp labels stay readable at typical mobile content width.
- Reviewed latest full mobile-width render and full-resolution details: region headings, state feedback, reference initialization wording, task-only weighting scope, policy/value parameter roles, three skill alternatives, all crop boundaries and no-label-overlap.
- Initial compile failed on malformed single-backslash line breaks; corrected to TeX line breaks. The failure is retained in local review logs, separate from the successful final compile. Final build has no missing glyphs or overfull boxes.
- All sample motions are conceptual illustrations. Original Fig2, performance tables and curves remain source-paper excerpts, separate from this diagram.
