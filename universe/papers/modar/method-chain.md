# 本篇方法链路 · ModAR

共享DiT把当前DINO/深度/RGB和配置/任务条件融合，按点轨迹→DINO→深度→RGB块自回归去噪，动作最后生成；上下文加噪避免前一模态误差层层放大。实机去掉收益最小的未来RGB。

共享DiT把当前DINO/深度/RGB和配置/任务条件融合，按点轨迹→DINO→深度→RGB块自回归去噪，动作最后生成；上下文加噪避免前一模态误差层层放大。实机去掉收益最小的未来RGB。

[本篇星系](../modar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/modar.md) · [原文依据](https://arxiv.org/abs/2609.17524v1)
