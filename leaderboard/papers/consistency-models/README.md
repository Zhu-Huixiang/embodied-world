# Consistency Models

**Consistency Models** · ICML 2023 · 本版排名 45 · 综合分 **86.1 / 100**

[解读导读](../../../library/consistency-models.md) · [Diffusion / Transformer 基础](../../../paper-map/README.md#track-diffusion-transformer) · [ICML集锦](../../../venues/ICML/README.md)

[原文](https://proceedings.mlr.press/v202/song23a.html) · [PDF](https://proceedings.mlr.press/v202/song23a/song23a.pdf) · [阅读卡片](../../../library/consistency-models.md)

论文出处：[Yang Song · OpenAI](../../origins/papers/consistency-models.md)

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
| 公开与评审 | 95.0 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 39.2 | 10% |
| 近期关注 | 38.4 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[ICML 2023](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v202/song23a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Consistency Models。累计被引 **22**，2025–2026 被引 **9**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4323076585) · [文献计量条目](https://openalex.org/W4323076585)

### 影响与关注的计算依据

- **学术影响 39.2**：身份匹配的累计引用C=22，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4323076585)
- **近期关注 38.4**：huggingface 的论文专属入口：HF 最近30天下载=82；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/openai/diffusers-cd_imagenet64_l2) · [依据2](https://huggingface.co/openai/diffusers-cd_imagenet64_l2/raw/main/README.md) · [依据3](https://huggingface.co/openai/diffusers-cd_imagenet64_l2)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/openai/consistency_models) | GitHub Star 6484；GitHub Watch订阅 59；GitHub Fork 433 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/openai/diffusers-cd_imagenet64_l2) | HF 最近30天下载 82；HF 仓库累计点赞 7 | 单篇原研究权重的HF转换版，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2303.01469) | HF 论文累计点赞 9 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
