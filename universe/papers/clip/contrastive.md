# 对比学习 · CLIP

给相关样本较高相似度，让它们在候选竞争中被找回来。图文配对是 CLIP 的监督来源。

CLIP 同批 N 对样本组成 N×N 相似度表，对角线是配对答案。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

继续拆：[向量归一化](normalization.md) · [余弦相似度](cosine.md) · [交叉熵](cross-entropy.md)。

[跨论文技术入口](../../concepts/contrastive.md)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
