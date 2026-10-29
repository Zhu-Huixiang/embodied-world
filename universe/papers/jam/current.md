# 当前观测到动作上下文 · JAM

骨干编码当前帧与指令，动作专家另接本体状态。

Wan当前视觉token为98×3072，Ovis为392×1536；动作专家读取骨干上下文，在flow-matching中预测动作块。

继续拆：[冻结未来目标分支](anchor.md)。

[本篇星系](../jam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jam.md) · [原文依据](https://arxiv.org/html/2610.37219v1)
