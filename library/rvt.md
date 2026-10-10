# RVT: Robotic View Transformer for 3D Object Manipulation

**解读导读** · CoRL 2023 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：多视图三维操作策略与高效空间表示。

[原文入口](https://proceedings.mlr.press/v229/goyal23a.html) · [原文 PDF](https://proceedings.mlr.press/v229/goyal23a/goyal23a.pdf) · [作者项目 / 代码入口](https://robotic-view-transformer.github.io/) · [作者与团队](../leaderboard/origins/papers/rvt.md)

CoRL 2023。论文的 26% 是相对成功率提升，不能写成 26 个百分点。

## 先看它做了什么

RGB-D 先变成点云，再从机器人工作区周围的虚拟相机重渲染多张视图；Transformer 在视图内及视图间聚合信息。多视图动作热图反投影得到夹爪位置，其他头预测姿态与夹爪状态。原文把成功率、训练达到相同性能所需时间和推理速度分别与 PerAct 对比，并展示真实少示范操作。

## 带着什么问题读

**体素太贵，重渲染几张虚拟视图能保住 3D 信息吗？**

## 为什么值得继续读

对 PerAct 计算瓶颈给出具体替代，兼顾 3D 几何结构、训练效率与真实操作，是高价值方法系列节点。

证据入口：PMLR 正式页给出 RLBench 与实机证据、PerAct 速度及成功率对照，代码和模型开放；新增表示的作用可通过直接对照讲清。

具身关联：对 PerAct 计算瓶颈给出具体替代，兼顾 3D 几何结构、训练效率与真实操作，是高价值方法系列节点。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/rvt/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-10。
