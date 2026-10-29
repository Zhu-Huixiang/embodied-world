# softmax 与温度 · DINO

对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。

温度改变概率集中程度；候选集合也会改变概率分母。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#33-c-区把分数变分布再跨视图对答案)

[跨论文技术入口](../../concepts/softmax.md)

[本篇星系](../dino.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md) · [原文依据](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
