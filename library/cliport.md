# CLIPort: What and Where Pathways for Robotic Manipulation

**解读导读** · CoRL 2021 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：语言条件桌面操作、语义与空间双流结构。

[原文入口](https://proceedings.mlr.press/v164/shridhar22a.html) · [原文 PDF](https://proceedings.mlr.press/v164/shridhar22a/shridhar22a.pdf) · [作者项目 / 代码入口](https://cliport.github.io/) · [作者与团队](../leaderboard/origins/papers/cliport.md)

CoRL 2021 主会在五年窗内，PMLR 164 于 2022 出版；首次 arXiv 在 2021 年 9 月，作为边界基础工作记录。

## 先看它做了什么

语义支路用 CLIP 提取 RGB 与指令概念，空间支路从 RGB-D 学习保持位置结构的特征；两路信息进入 Transporter 的拾取与放置预测。拾取位置先决定裁出哪块特征，再用互相关找到合适的放置区域。原文在多任务仿真和真实桌面上检验新物体、语义概念与少量示范。

## 带着什么问题读

**CLIP 知道是什么，但不知道手该落在哪里；语义和几何怎样配合？**

## 为什么值得继续读

语义预训练与空间等变操作结合的代表作，是理解语言操作路线从 Transporter 到 PerAct 的重要节点。

证据入口：PMLR 正式版与作者项目提供双流结构、语义泛化以及真实多任务评估，公开代码支持复用；主题冲突具体且容易讲清。

具身关联：语义预训练与空间等变操作结合的代表作，是理解语言操作路线从 Transporter 到 PerAct 的重要节点。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/cliport/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-10。
