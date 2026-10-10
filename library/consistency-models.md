# Consistency Models

出处：ICML 2023。研究范围：生成/表征基础，Consistency Policy 的少步动作生成与蒸馏。

[原文入口](https://proceedings.mlr.press/v202/song23a.html) · [原文 PDF](https://proceedings.mlr.press/v202/song23a/song23a.pdf) · [作者项目 / 代码入口](https://github.com/openai/consistency_models)

ICML 2023，PMLR 202；一致性生成基础与 RSS 2024 Consistency Policy 的操作实验证据分开。

阅读问题：**沿同一条去噪轨迹的不同点，怎样被一个模型直接映射回同一样本？**

收录理由：已收录的 Consistency Policy 把一致性蒸馏用于动作扩散加速，这篇给出轨迹自一致性与一步/少步采样的核心定义。

证据入口：一条轨迹的自一致性定义清楚，蒸馏与独立训练都有对照，官方实现公开；与 Consistency Policy 的知识链紧密。

具身关联：已收录的 Consistency Policy 把一致性蒸馏用于动作扩散加速，这篇给出轨迹自一致性与一步/少步采样的核心定义。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/consistency-models/README.md)

机制简析：学习一个映射，使概率流 ODE 同一轨迹上的不同噪声点都输出同一个干净样本。蒸馏版由教师扩散模型和求解器产生相邻轨迹点，训练版则直接通过相邻噪声尺度的一致性约束学习。原文在标准图像数据集比较一步、少步生成和编辑，机器人策略将同类映射用于压缩动作采样延迟。
<!-- discovery:end -->
