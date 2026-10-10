# Consistency Models

**Consistency Models** · ICML 2023 · 本版排名 51 · 综合分 **86.1 / 100**

[解读导读](../../../library/consistency-models.md) · [Diffusion / Transformer 基础](../../../paper-map/README.md#track-diffusion-transformer) · [ICML集锦](../../../venues/ICML/README.md)

[原文](https://proceedings.mlr.press/v202/song23a.html) · [PDF](https://proceedings.mlr.press/v202/song23a/song23a.pdf) · [阅读卡片](../../../library/consistency-models.md)

## 机制简析

学习一个映射，使概率流 ODE 同一轨迹上的不同噪声点都输出同一个干净样本。蒸馏版由教师扩散模型和求解器产生相邻轨迹点，训练版则直接通过相邻噪声尺度的一致性约束学习。原文在标准图像数据集比较一步、少步生成和编辑，机器人策略将同类映射用于压缩动作采样延迟。

带着这个问题读：沿同一条去噪轨迹的不同点，怎样被一个模型直接映射回同一样本？

初读判断：一条轨迹的自一致性定义清楚，蒸馏与独立训练都有对照，官方实现公开；与 Consistency Policy 的知识链紧密。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 39.2 | 10% |
| 近期关注 | 37.0 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[ICML 2023](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v202/song23a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Consistency Models。累计被引 22，2025–2026 被引 9；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4323076585) · [文献计量条目](https://openalex.org/W4323076585)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
