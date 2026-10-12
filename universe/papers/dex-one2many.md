# Dex-One2Many 星系

Dex-One2Many: Learning Dexterous Manipulation from a Single Human Demonstration

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dex-one2many.md) · [原文](https://arxiv.org/abs/2610.12470v1) · [评分卡](../../leaderboard/papers/dex-one2many/README.md)

把单视频压成顺序场景关系图，以图约束重置状态、阶段奖励，指导 RL 搜索更广的抓取与物体配置。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

## 本篇行星与卫星

- [空间表示](dex-one2many/spatial.md) · 初读挂点
- [强化学习](dex-one2many/rl.md) · 初读挂点
- [机器人数据与评测](dex-one2many/data.md) · 初读挂点
- [本篇方法链路](dex-one2many/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
