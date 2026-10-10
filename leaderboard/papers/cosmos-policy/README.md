# Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning

**Cosmos Policy** · ICLR 2026 · 本版排名 103 · 综合分 **78.5 / 100**

[解读导读](../../../library/cosmos-policy.md) · [世界动作模型](../../../paper-map/README.md#track-world-action-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://openreview.net/forum?id=wPEIStHxYH) · [PDF](https://arxiv.org/pdf/2601.16163) · [阅读卡片](../../../library/cosmos-policy.md)

论文出处：[Moo Jin Kim · NVIDIA / Stanford University](../../origins/papers/cosmos-policy.md)

## 机制简析

微调视频基础模型，把动作、未来视觉状态和规划信号放进共同生成过程。

带着这个问题读：视频生成序列怎样容纳动作、未来状态与规划信号？

初读判断：视频先验到控制的接口值得看；精读需追训练条件和规划/策略消融。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 82 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 54.8 | 5% |
| 复用价值 | 82 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[ICLR 2026](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://openreview.net/forum?id=wPEIStHxYH)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本；匹配题目：Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W7125496427) · [文献计量条目](https://openalex.org/W7125496427)

### 影响与关注的计算依据

- **学术影响 0.0**：身份匹配的累计引用C=0，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7125496427)
- **近期关注 54.8**：huggingface 的论文专属入口：HF 最近30天下载=551；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/nvidia/Cosmos-Policy-LIBERO-Predict2-2B) · [依据2](https://huggingface.co/nvidia/Cosmos-Policy-LIBERO-Predict2-2B/raw/main/README.md) · [依据3](https://huggingface.co/nvidia/Cosmos-Policy-LIBERO-Predict2-2B)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/nvidia/Cosmos-Policy-ALOHA-Planning-Model-Predict2-2B) | HF 最近30天下载 228；HF 仓库累计点赞 9 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/nvidia/Cosmos-Policy-LIBERO-Predict2-2B) | HF 最近30天下载 551；HF 仓库累计点赞 8 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2601.16163) | HF 论文累计点赞 15 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
