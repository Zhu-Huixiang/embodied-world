# EfficientZero V2: Mastering Discrete and Continuous Control with Limited Data

出处：ICML 2024。研究范围：世界模型与连续/离散规划；模拟控制基础。

[原文入口](https://proceedings.mlr.press/v235/wang24at.html) · [原文 PDF](https://raw.githubusercontent.com/mlresearch/v235/main/assets/wang24at/wang24at.pdf)

ICML 2024 Spotlight 的正式会议信息可在官方 virtual 页面交叉核对。

阅读问题：**树搜索怎样跨过离散动作的限制，在连续控制里仍保持样本效率？**

收录理由：把有影响力的 EfficientZero 树搜索路线扩展到连续动作，正式 ICML 论文同时覆盖 Atari、视觉和本体控制，适合与 Dreamer/TD-MPC 对读。

证据入口：正式 ICML Spotlight，原文跨三类基准并比较 DreamerV3；连续树搜索与价值估计分别有消融，初读评分保留为编辑判断。

具身关联：把有影响力的 EfficientZero 树搜索路线扩展到连续动作，正式 ICML 论文同时覆盖 Atari、视觉和本体控制，适合与 Dreamer/TD-MPC 对读。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/efficientzero-v2/README.md)

机制简析：表示函数得到潜状态，动力学函数接收动作并预测潜状态与奖励，策略和值网络为搜索提供先验。连续动作下先采样候选动作，再用基于 Gumbel 的树搜索改善策略，并用搜索产生价值目标以利用旧经验。实验按有限交互预算比较离散和连续、图像和低维输入任务。
<!-- discovery:end -->
