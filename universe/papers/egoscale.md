# EgoScale 星系

EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/egoscale.md) · [原文](https://arxiv.org/abs/2602.16710) · [评分卡](../../leaderboard/papers/egoscale/README.md)

从第一视角human videos提取相对SE(3)腕部轨迹与重定向22DoF手关节，pretrain flow-based VLA；少量paired human/robot play midtraining对齐视觉和motor接口，再任务posttrain。统一腕部action、embodiment-specific hand/state adapters迁移至G1 7DoF手，下肢独立Homie。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

## 本篇行星与卫星

- [Flow Matching](egoscale/flow.md) · 初读挂点
- [运动重定向](egoscale/retarget.md) · 初读挂点
- [跨本体数据](egoscale/cross-body.md) · 初读挂点
- [本篇方法链路](egoscale/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
