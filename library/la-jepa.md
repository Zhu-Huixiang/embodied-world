# La-JEPA: Compact Robot Policies with Latent World Modeling

**解读导读** · arXiv 2026 · [世界动作模型](../paper-map/README.md#track-world-action-model)

研究范围：目标示范训练的紧凑世界动作模型；LIBERO/Plus、50任务RoboTwin 2.0与单台Franka的四种桌面操作。

[原文入口](https://arxiv.org/abs/2611.08156v1) · [原文 PDF](https://arxiv.org/pdf/2611.08156v1) · [作者与团队](../leaderboard/origins/papers/la-jepa.md)

所读v1。无机器人预训练仍使用预训练视觉与语言编码器；主结果按三训练seed报告，原发布指令与校正指令分别比较。专属代码入口当前为空库。

## 先看它做了什么

La-JEPA以预训练V-JEPA 2.1 ViT-L编码当前两帧和32帧范围内的未来16帧，FLAN-T5-large编码语言，本体投影为条件token。在该表征空间从头训练World DiT和Action DiT，分别对未来特征与32步动作块做独立时间的流匹配。观测只读观测、未来读观测和未来、动作只读观测和动作；未来损失通过共享World参数影响观测表示。部署删除未来token，固定World时间0并缓存观测K/V，仅对动作做10步Euler积分，LIBERO执行10步、RoboTwin执行24步后重规划。最终观测编码器用LoRA和增强，未来目标保持原冻结编码器的干净特征；无需像素解码。

## 带着什么问题读

**要借用预训练视觉知识，就得把大视频生成器整套搬上机器人吗？如果只保留JEPA表征并训练小型动作模型，未来预测在部署被删除后还剩下什么价值？**

## 为什么值得继续读

从控制架构与感知预训练的耦合提出具体问题，注意力路径和联合目标可核；多seed模拟、未来监督/表征/鲁棒性设计研究与有限实机证据足以支持预印本收录。代码空库、校正文本协议和跨论文比较边界公开保留。

证据入口：RoboTwin 50任务clean训练、各条件各seed 5000回合、3训练seed：S/B/L的clean为85.5/86.2/86.0%，randomized为33.9/35.4/32.1%，B平均60.8%；Fast-WAM77.8/1.9来自官方榜。LIBERO-Plus修正文本10030变体（部分基线10029）下S/B/L86.3/87.3/88.0%，NowWAM86.2；原文本S/B/L80.0/82.5/84.1%，须分开。原始管线三seed未来监督76.47%对action-only74.35%，不能与主表跨管线比较。单Franka四任务各20次：La-JEPA70/80对π0.5 69/80，近似而非显著超越。10步优化S17.78ms/B25.16ms对Fast-WAM88.09ms是单次policy-call，不是控制周期，GPU型号未列。

具身关联：直接讨论视觉世界表征如何帮助示范学习动作，以及推理时不预测未来能否保留控制收益；包含闭环模拟、跨扰动和有限真实接触操作。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/la-jepa.md) · [七维评分与雷达](../leaderboard/papers/la-jepa/README.md) · [arXiv集锦](../arxiv/README.md#paper-la-jepa) · [地图方向](../paper-map/README.md#track-world-action-model) · [首页](../README.md)

元数据核对：2026-11-07。
