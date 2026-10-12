# RoboCasa 星系

RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/robocasa.md) · [原文](https://roboticsproceedings.org/rss20/p050.html) · [评分卡](../../leaderboard/papers/robocasa/README.md)

在厨房仿真中同时扩展可交互家具、物体、布局与视觉纹理，再把基础技能组合成长任务。人类示范与自动轨迹生成共同提供训练数据，模型在不同数据规模和任务条件下学习。原文的重点是模拟多样性和合成数据是否形成可测的性能增长，并探索向真实任务迁移。

## 技术挂点

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [泛化评测与遗忘](robocasa/benchmark.md) · 初读挂点
- [机器人数据与评测](robocasa/data.md) · 初读挂点
- [行为克隆](robocasa/bc.md) · 初读挂点
- [本篇方法链路](robocasa/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
