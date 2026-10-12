# BridgeData V2 星系

BridgeData V2: A Dataset for Robot Learning at Scale

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/bridge-v2.md) · [原文](https://proceedings.mlr.press/v229/walke23a.html) · [评分卡](../../leaderboard/papers/bridge-v2/README.md)

统一低成本机械臂平台收集语言标注轨迹，同时主动变化物体、相机、场景和工作台位置。策略可按目标图或自然语言训练，测试再拆开已见任务的视觉变化与新物体、新环境泛化。不同离线学习方法、数据规模和模型容量在同一数据上比较，让数据多样性的作用有可检查的落点。

## 技术挂点

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [行为克隆](bridge-v2/bc.md) · 初读挂点
- [跨本体数据](bridge-v2/cross-body.md) · 初读挂点
- [泛化评测与遗忘](bridge-v2/benchmark.md) · 初读挂点
- [本篇方法链路](bridge-v2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
