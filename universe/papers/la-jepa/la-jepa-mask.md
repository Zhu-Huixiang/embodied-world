# 动作看观测，不直接看未来token · La-JEPA

三类token的可见关系决定训练与部署能否分开。

观测只读观测；未来读观测和未来；动作读观测和动作。动作查询读取World DiT观测K/V，未来损失通过共享World参数塑造观测表征，并非推理时把预测视频喂给动作。

继续拆：[两个独立流时间，两个速度目标](la-jepa-flow.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
