# Isaac Gym: High Performance GPU Based Physics Simulation For Robot Learning

**Isaac Gym** · NeurIPS D&B 2021 · 本版排名 48 · 综合分 **86.3 / 100**

[原文](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/28dd2c7955ce926456240b2ff0100bde-Abstract-round2.html) · [PDF](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/file/28dd2c7955ce926456240b2ff0100bde-Paper-round2.pdf) · [阅读卡片](../../../library/isaac-gym.md)

## 机制简析

GPU PhysX 缓冲包装为 PyTorch tensor；观测、奖励、动作、并行 rollout 与 PPO 保持 GPU，省去 CPU↔GPU 往返。

带着这个问题读：GPU 仿真、奖励和策略更新怎样连成一条流水线，改变机器人 RL 的试错速度？

初读判断：八类环境和资源/训练时间有证据，公开流程复用价值极高；不同旧系统资源配置按各自条件讲。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 90.0 | 30% |
| 创新性 | 92 | 20% |
| 实验与证据 | 94 | 20% |
| 学术影响 | 50.9 | 10% |
| 近期关注 | 49.0 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[NeurIPS D&B 2021](../../../venues/NeurIPS-Datasets-Benchmarks/README.md)，正式出处见[出版/原文记录](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/28dd2c7955ce926456240b2ff0100bde-Abstract-round2.html)；采用2026-10-10刊会快照。


编辑深度：原文方法与实验选题初读；非全文精读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Isaac Gym: High Performance GPU-Based Physics Simulation For Robot Learning。累计被引 58，2025–2026 被引 20；快照：2026-10-10T11:44:51+08:00。

[指标记录](https://api.openalex.org/works/W3193576605) · [文献计量条目](https://openalex.org/W3193576605)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
