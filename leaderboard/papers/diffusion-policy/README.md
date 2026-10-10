# Diffusion Policy: Visuomotor Policy Learning via Action Diffusion

**Diffusion Policy** · RSS 2023 · 本版排名 12 · 综合分 **92.6 / 100**

[解读导读](../../../library/diffusion-policy.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss19/p026.html) · [PDF](https://www.roboticsproceedings.org/rss19/p026.pdf) · [阅读卡片](../../../library/diffusion-policy.md)

论文出处：[**Cheng Chi**](../../origins/papers/diffusion-policy.md)<br>[哥伦比亚大学具身智能团队 / 丰田研究院 · 另1个机构](../../origins/papers/diffusion-policy.md)

## 机制简析

对多步动作条件去噪，用视觉观测约束动作分布，滚动执行一段后再次观测与重规划。

带着这个问题读：为什么要对一段动作分布去噪，再滚动执行？

初读判断：动作分布与闭环执行的清楚范式；丰富任务对照和可复用代码是阅读优势。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 96 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 78.1 | 10% |
| 近期关注 | 87.8 | 5% |
| 复用价值 | 95 | 8% |
| 阅读价值 | 98 | 7% |

刊会依据：[RSS 2023](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss19/p026.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Diffusion Policy: Visuomotor Policy Learning via Action Diffusion。累计被引 **517**，2025–2026 被引 **405**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4385403811) · [文献计量条目](https://openalex.org/W4385403811)

### 影响与关注的计算依据

- **学术影响 78.1**：身份匹配的累计引用C=517，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4385403811)
- **近期关注 87.8**：huggingface 的论文专属入口：HF 最近30天下载=24473；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/lerobot/pusht) · [依据2](https://huggingface.co/datasets/lerobot/pusht/raw/main/README.md) · [依据3](https://huggingface.co/datasets/lerobot/pusht)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/real-stanford/diffusion_policy) | GitHub Star 4618；GitHub Watch订阅 20；GitHub Fork 853 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/lerobot/pusht) | HF 最近30天下载 24473；HF 仓库累计点赞 59 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/lerobot/diffusion_pusht) | HF 最近30天下载 8829；HF 仓库累计点赞 65 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2303.04137) | HF 论文累计点赞 6 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
