# OpenVLA: An Open-Source Vision-Language-Action Model

**OpenVLA** · CoRL 2024 · 本版排名 65 · 综合分 **84.5 / 100**

[解读导读](../../../library/openvla.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v270/kim25c.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/kim25c/kim25c.pdf) · [阅读卡片](../../../library/openvla.md)

论文出处：[**Moo Jin Kim / Karl Pertsch 等3位**](../../origins/papers/openvla.md)<br>[斯坦福 IRIS 实验室 / 伯克利 RAIL 实验室 · 另4个机构](../../origins/papers/openvla.md)

## 机制简析

把预训练视觉语言骨干适配到机器人示范，输出离散动作编号，并提供高效微调路线。

带着这个问题读：视觉特征融合、动作分箱和高效适配各自解决哪一层问题？

初读判断：公开模型/适配生态便于复用；是离散VLA入门的重要对照。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 83 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 47.8 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[CoRL 2024](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v270/kim25c.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本；匹配题目：OpenVLA: An Open-Source Vision-Language-Action Model。累计被引 **45**，2025–2026 被引 **42**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4399695759) · [文献计量条目](https://openalex.org/W4399695759)

### 影响与关注的计算依据

- **学术影响 47.8**：身份匹配的累计引用C=45，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4399695759)
- **近期关注 100**：huggingface 的论文专属入口：HF 最近30天下载=151901；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/openvla/openvla-7b) · [依据2](https://huggingface.co/openvla/openvla-7b/raw/main/README.md) · [依据3](https://huggingface.co/openvla/openvla-7b)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/openvla/openvla) | GitHub Star 7128；GitHub Watch订阅 32；GitHub Fork 857 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/openvla/modified_libero_rlds) | HF 最近30天下载 14600；HF 仓库累计点赞 78 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/openvla/openvla-7b) | HF 最近30天下载 151901；HF 仓库累计点赞 262 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2406.09246) | HF 论文累计点赞 47；HF 论文讨论评论累计数 1 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
