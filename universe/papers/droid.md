# DROID 星系

DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/droid.md) · [原文](https://www.roboticsproceedings.org/rss20/p120.html) · [评分卡](../../leaderboard/papers/droid/README.md)

不同机构使用一致的机械臂、相机与遥操作平台，把设备移到大量真实场景收集示范，保存同步视觉、动作、语言及相机标定。训练时混入这些跨场景经验，再测试任务性能、鲁棒性与泛化。可迁移的核心不只是轨迹数量，而是场景、相机与交互位置覆盖。

## 技术挂点

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [机器人数据与评测](droid/data.md) · 初读挂点
- [跨本体数据](droid/cross-body.md) · 初读挂点
- [行为克隆](droid/bc.md) · 初读挂点
- [本篇方法链路](droid/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
