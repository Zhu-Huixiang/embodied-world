# Where are we in the search for an Artificial Visual Cortex for Embodied Intelligence?

**VC-1** · NeurIPS 2023 · 本版排名 71 · 综合分 **83.9 / 100**

[解读导读](../../../library/vc1.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/022ca1bed6b574b962c48a2856eb207b-Paper-Conference.pdf) · [阅读卡片](../../../library/vc1.md)

论文出处：[Arjun Majumdar · Georgia Institute of Technology / Meta FAIR 等5个出处](../../origins/papers/vc1.md)

## 机制简析

先把导航、移动操作、灵巧操作和运动控制纳入 CortexBench，统一比较不同预训练视觉模型。固定 MAE 目标后变化视频来源、数据规模和 ViT 容量，再检验同一编码器能否处处占优。VC-1 的平均提升和任务适配提升分别报告，暴露视觉预训练的任务差异。

带着这个问题读：有没有一套视觉编码器在所有具身任务上都强？扩大人类视频数据就够了吗？

初读判断：NeurIPS 正式版明确是系统评估而非新算法，跨领域任务、数据/容量研究、硬件实验和公开模型构成强证据；榜单应奖励研究设计而非包装新模块。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 38.6 | 10% |
| 近期关注 | 24.6 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[NeurIPS 2023](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Where are we in the search for an Artificial Visual Cortex for Embodied Intelligence?。累计被引 **21**，2025–2026 被引 **5**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4362514550) · [文献计量条目](https://openalex.org/W4362514550)

### 影响与关注的计算依据

- **学术影响 38.6**：身份匹配的累计引用C=21，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4362514550)
- **近期关注 24.6**：huggingface 的论文专属入口：HF 最近30天下载=16；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/facebook/vc1-large) · [依据2](https://huggingface.co/facebook/vc1-large/raw/main/README.md) · [依据3](https://huggingface.co/facebook/vc1-large)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/facebookresearch/eai-vc) | GitHub Star 509；GitHub Watch订阅 20；GitHub Fork 47 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/facebook/vc1-large) | HF 最近30天下载 16；HF 仓库累计点赞 9 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2303.18240) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
