# Flow Matching for Generative Modeling

出处：ICLR 2023。研究范围：生成/表征基础，π₀ 类连续动作专家的条件流匹配。

[原文入口](https://iclr.cc/virtual/2023/poster/11309) · [原文 PDF](https://arxiv.org/pdf/2210.02747) · [作者项目 / 代码入口](https://github.com/facebookresearch/flow_matching)

ICLR 2023 正式论文；官方会场确认题名和录用，原始论文用图像任务评估。

阅读问题：**不模拟整条生成轨迹就能训练速度场，π₀ 里的 Flow Matching 损失怎样读？**

收录理由：π₀ 的连续动作生成采用 flow matching 路线，这篇给出路径、目标速度与回归训练的数学基础，具身联系直接。

证据入口：目标等价关系与路径选择构成明确创新，图像对照和通用实现完善；连续动作流匹配教程需要先把这套对象定义清楚。

具身关联：π₀ 的连续动作生成采用 flow matching 路线，这篇给出路径、目标速度与回归训练的数学基础，具身联系直接。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/flow-matching/README.md)

机制简析：给噪声与数据之间指定一个条件概率路径，直接回归该路径的目标速度场，训练时不用数值模拟完整 ODE。条件流匹配的目标在梯度层面对应难直接计算的边缘流目标；生成时才用求解器沿学习的速度场从噪声走向数据。原文比较扩散型路径与最优传输型插值，在 ImageNet 检查样本质量、似然和速度。
<!-- discovery:end -->
