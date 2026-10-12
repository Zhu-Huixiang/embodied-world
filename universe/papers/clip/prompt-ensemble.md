# 提示模板集成 · CLIP

同一类别放进多种句子模板，编码后平均并归一化，减少单一表述对分类权重的影响。

CLIP 的模板集成先缓存类别向量，推理不必逐图重算所有文字。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#25-使用一句话怎样变成分类器)

[跨论文技术入口](../../concepts/prompt-ensemble.md)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
