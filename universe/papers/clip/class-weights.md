# 文本生成类别权重 · CLIP

把类别句子编码成分类器的权重行。

B/32的K类权重表形状K×512，新图只编码一次，与K个单位文本向量比较。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#25-使用一句话怎样变成分类器)

继续拆：[类别向量缓存](cache.md) · [提示上下文与歧义](ambiguity.md) · [候选集合与拒识](closed-set.md)。

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
