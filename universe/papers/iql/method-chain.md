# 本篇方法链路 · IQL

IQL 在数据动作的 Q 值上做非对称 expectile 回归，拟合偏向较好动作的状态值 V。Q 用奖励加下一状态 V 做 Bellman 更新，策略再按优势加权回归数据中的动作。这个过程把值学习与策略提取拆开，实验用 D4RL 与在线微调检查拼接和改善能力。

IQL 在数据动作的 Q 值上做非对称 expectile 回归，拟合偏向较好动作的状态值 V。Q 用奖励加下一状态 V 做 Bellman 更新，策略再按优势加权回归数据中的动作。这个过程把值学习与策略提取拆开，实验用 D4RL 与在线微调检查拼接和改善能力。

[本篇星系](../iql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/iql.md) · [原文依据](https://iclr.cc/virtual/2022/poster/5941)
