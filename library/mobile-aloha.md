# Mobile ALOHA: Learning Bimanual Mobile Manipulation using Low-Cost Whole-Body Teleoperation

**解读导读** · CoRL 2024 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：双臂移动操作、全身遥操作与静态/移动数据联合训练。

[原文入口](https://proceedings.mlr.press/v270/fu25b.html) · [原文 PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/fu25b/fu25b.pdf) · [作者项目 / 代码入口](https://mobile-aloha.github.io/) · [作者与团队](../leaderboard/origins/papers/mobile-aloha.md)

CoRL 2024；PMLR 270 于 2025 出版。正式题目 using 与项目/首版 with 为同一工作。

## 先看它做了什么

把双臂关节位置与底盘线/角速度拼成统一动作，遥操作同时记录手臂与底盘；行为克隆直接预测整套动作。训练混入已有静态 ALOHA 示范，检验不同任务、臂安装位置和场景之间的正迁移。原文把自治策略执行与人类遥操作采集分开，比较联合训练和只用移动数据的任务表现。

## 带着什么问题读

**桌面双臂经验为什么能帮会移动的机器人做饭、开柜子和坐电梯？**

## 为什么值得继续读

双臂移动操作的高关注代表项目，任务直观、硬件与训练路线开放，适合以科学机制解释公众常见的机器人演示。

证据入口：CoRL 正式稿与首版方法给出真实长程移动任务和联合训练对照，开放软硬件便于复用；视觉演示具有传播价值，评分仍以自治任务评估而非视频震撼程度为依据。

具身关联：双臂移动操作的高关注代表项目，任务直观、硬件与训练路线开放，适合以科学机制解释公众常见的机器人演示。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/mobile-aloha/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-10。
