# Isaac Gym: High Performance GPU Based Physics Simulation For Robot Learning

**解读导读** · NeurIPS D&B 2021 · [强化学习与离线决策](../paper-map/README.md#track-reinforcement-learning)

研究范围：机器人 RL 的 GPU 物理仿真基础设施。

[原文入口](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/hash/28dd2c7955ce926456240b2ff0100bde-Abstract-round2.html) · [原文 PDF](https://datasets-benchmarks-proceedings.neurips.cc/paper/2021/file/28dd2c7955ce926456240b2ff0100bde-Paper-round2.pdf) · [作者项目 / 代码入口](https://research.nvidia.com/labs/srl/publication/makoviychuk-2021-isaac/)

正式 NeurIPS 2021 Datasets and Benchmarks Track；NVIDIA 官方出版列表 Dec 2021，正式日期在五年窗内。物理仿真工具，不是学习型世界模型。

## 先看它做了什么

GPU PhysX 缓冲包装为 PyTorch tensor；观测、奖励、动作、并行 rollout 与 PPO 保持 GPU，省去 CPU↔GPU 往返。

## 带着什么问题读

**GPU 仿真、奖励和策略更新怎样连成一条流水线，改变机器人 RL 的试错速度？**

## 为什么值得继续读

正式 NeurIPS 2021 D&B track；GPU 全链路物理与训练是腿足、人形、灵巧 RL 的基础设施漏收项。

证据入口：八类机器人环境；A100 条件下 Ant20秒、Humanoid4分钟、ANYmal<2分钟、ShadowHand cube35分钟等。保留硬件/任务条件，不能统一算资源匹配加速。（tensor API / framework 与 benchmark表）

具身关联：机器人 RL 的 GPU 物理仿真基础设施；GPU 仿真、奖励和策略更新怎样连成一条流水线，改变机器人 RL 的试错速度？

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/isaac-gym/README.md) · [NeurIPS D&B集锦](../venues/NeurIPS-Datasets-Benchmarks/README.md) · [地图方向](../paper-map/README.md#track-reinforcement-learning) · [首页](../README.md)

元数据核对：2026-10-10。
