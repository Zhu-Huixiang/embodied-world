# π₀ 星系

π₀: A Vision-Language-Action Flow Model for General Robot Control

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/pi0.md) · [原文](https://www.roboticsproceedings.org/rss21/p010.html) · [评分卡](../../leaderboard/papers/pi0/README.md)

视觉语言骨干提供语义条件，Flow Matching 动作专家生成连续动作块，再按闭环观测更新。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

## 本篇行星与卫星

- [Flow Matching](pi0/flow.md) · 初读挂点
- [动作块](pi0/chunk.md) · 初读挂点
- [注意力](pi0/attention.md) · 初读挂点
- [本篇方法链路](pi0/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
