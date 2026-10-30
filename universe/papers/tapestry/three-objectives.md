# 三种训练目标共用一个骨干 · TAPESTRY

视频生成、联合生成和动作独立去噪分别承担迁移、耦合和部署匹配。

无动作视频只做视频扩散；有动作样本以0.5概率做联合模式，否则同时做视频与动作独立模式。视频/动作损失权重0.1/1。

继续拆：[动作看视频，视频不看动作](asymmetric-mask.md) · [把去视频部署路径也练到](deployment-match.md) · [固定5epoch的组件比较](ablation-budget.md)。

[本篇星系](../tapestry.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tapestry.md) · [原文依据](https://arxiv.org/pdf/2610.36823v1)
