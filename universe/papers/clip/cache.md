# 类别向量缓存 · CLIP

预先计算类别文字，推理时直接比较。

换类别或模板就重算对应文字向量；每张新图不用让文本网络陪所有候选重跑。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#25-使用一句话怎样变成分类器)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
