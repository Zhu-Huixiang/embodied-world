# PaLM-E 星系

PaLM-E: An Embodied Multimodal Language Model

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/palm-e.md) · [原文](https://proceedings.mlr.press/v202/driess23a.html) · [评分卡](../../leaderboard/papers/palm-e/README.md)

视觉和连续状态由编码器变成与语言 token 等维的向量，和文本交错组成多模态句子，再交给 decoder-only 语言模型生成文字。训练同时覆盖机器人任务、视觉问答和图文任务，以检验知识是否产生正迁移。机器人演示中，文字计划交给底层策略执行，后续视觉反馈再进入模型。

## 技术挂点

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

## 本篇行星与卫星

- [表征空间](palm-e/representation.md) · 初读挂点
- [因果序列建模](palm-e/causal.md) · 初读挂点
- [分层技能与计划](palm-e/skills.md) · 初读挂点
- [本篇方法链路](palm-e/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
