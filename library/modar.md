# Modality-Autoregressive World-Action Models

**解读导读** · arXiv 2026 · [世界动作模型](../paper-map/README.md#track-world-action-model)

研究范围：多模态世界动作模型；双臂操作。

[原文入口](https://arxiv.org/abs/2609.17524v1) · [原文 PDF](https://arxiv.org/pdf/2609.17524v1) · [作者项目 / 代码入口](https://adamhung60.github.io/ModAR/)

arXiv v1；官方项目和原文未核到正式会刊。

## 先看它做了什么

共享DiT把当前DINO/深度/RGB和配置/任务条件融合，按点轨迹→DINO→深度→RGB块自回归去噪，动作最后生成；上下文加噪避免前一模态误差层层放大。实机去掉收益最小的未来RGB。

## 带着什么问题读

**为什么先预测点轨迹、语义与几何，再给动作，可能比视频动作一起去噪更有效？**

## 为什么值得继续读

控制WAM组织形式、模态和计算预算的比较较完整，外加三项实机。

证据入口：6项RoboTwin，每项50个held-out初始条件；固定50条有动作demo，其余actionless，总250时ModAR平均75%、Unified67%；总1250时76% vs64%。（§IV-A/B; Table I）；同一独立IDM仍保留优势；匹配40Eulersteps后Unified59%、Disjoint54%、Independent-noise37%，ModAR75%。（Fig.5 / sampling-step comparison）；去context-noise75%→63%，反序65%；实机3任务每模型每任务30rollouts，ModAR83.3%、Unified66.7%、Action-only52.2%；增加human actionless数据70.0%→81.1%→83.3%。（Fig.6-7 / §IV-C/D）

具身关联：多模态世界动作模型；双臂操作；为什么先预测点轨迹、语义与几何，再给动作，可能比视频动作一起去噪更有效？

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/modar/README.md) · [arXiv集锦](../arxiv/README.md#paper-modar) · [地图方向](../paper-map/README.md#track-world-action-model) · [首页](../README.md)

元数据核对：2026-10-10。
