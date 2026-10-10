# Modality-Autoregressive World-Action Models

出处：arXiv 2026。研究范围：多模态世界动作模型；双臂操作。

[原文入口](https://arxiv.org/abs/2609.17524v1) · [原文 PDF](https://arxiv.org/pdf/2609.17524v1) · [作者项目 / 代码入口](https://adamhung60.github.io/ModAR/)

arXiv v1；官方项目和原文未核到正式会刊。

阅读问题：**为什么先预测点轨迹、语义与几何，再给动作，可能比视频动作一起去噪更有效？**

收录理由：控制WAM组织形式、模态和计算预算的比较较完整，外加三项实机。

证据入口：6项RoboTwin，每项50个held-out初始条件；固定50条有动作demo，其余actionless，总250时ModAR平均75%、Unified67%；总1250时76% vs64%。（§IV-A/B; Table I）；同一独立IDM仍保留优势；匹配40Eulersteps后Unified59%、Disjoint54%、Independent-noise37%，ModAR75%。（Fig.5 / sampling-step comparison）；去context-noise75%→63%，反序65%；实机3任务每模型每任务30rollouts，ModAR83.3%、Unified66.7%、Action-only52.2%；增加human actionless数据70.0%→81.1%→83.3%。（Fig.6-7 / §IV-C/D）

具身关联：多模态世界动作模型；双臂操作；为什么先预测点轨迹、语义与几何，再给动作，可能比视频动作一起去噪更有效？

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/modar/README.md)

机制简析：共享DiT把当前DINO/深度/RGB和配置/任务条件融合，按点轨迹→DINO→深度→RGB块自回归去噪，动作最后生成；上下文加噪避免前一模态误差层层放大。实机去掉收益最小的未来RGB。
<!-- discovery:end -->
