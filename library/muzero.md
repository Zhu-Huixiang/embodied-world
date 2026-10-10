# Mastering Atari, Go, chess and shogi by planning with a learned model

出处：Nature 2020。研究范围：任务导向世界模型与树搜索基础；非实机实验。

[原文入口](https://www.nature.com/articles/s41586-020-03051-4) · [原文 PDF](https://arxiv.org/pdf/1911.08265)

经典例外；期刊正式公开日期为 2020-12-23，arXiv 首稿为 2019。

阅读问题：**用于规划的世界模型，为什么可以只预测奖励、价值和策略，而不重建下一帧？**

收录理由：学习潜动力学再树搜索的基础路线，EfficientZero 正式论文直接以它为起点；为世界模型的任务充分表示提供高价值讨论。

证据入口：Nature 正式论文、跨棋类和 Atari 的完整实验、公开伪代码；EfficientZero 的直接继承为路线影响提供可核实依据。

具身关联：学习潜动力学再树搜索的基础路线，EfficientZero 正式论文直接以它为起点；为世界模型的任务充分表示提供高价值讨论。

经典保留理由：放宽年限：MuZero 是任务导向潜动力学与模型内树搜索的公认基础路线，EfficientZero 系列直接继承；不是为凑数新增旧论文。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/muzero/README.md)

机制简析：表示网络从观测历史得到潜状态，动力学网络在动作条件下预测下一潜状态和奖励，预测网络给出策略先验和值。MCTS 在这些潜状态里展开候选动作，搜索产生的策略和值再监督网络。Nature 论文比较棋类与 Atari；这里关注的是规划表征，而不是实机机器人结论。
<!-- discovery:end -->
