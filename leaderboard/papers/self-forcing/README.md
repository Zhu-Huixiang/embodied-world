# Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion

**Self Forcing** · NeurIPS 2025 · 本版排名 53 · 综合分 **85.4 / 100**

[解读导读](../../../library/self-forcing.md) · [视频与序列生成](../../../paper-map/README.md#track-video-generation) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/f4823f831af67a3ef15e41a85434422a-Paper-Conference.pdf) · [阅读卡片](../../../library/self-forcing.md)

论文出处：[Xun Huang · Adobe Research / The University of Texas at Austin](../../origins/papers/self-forcing.md)

## 机制简析

使用模型自己的历史滚动来训练自回归视频生成，减少教师历史与部署历史的分布差异。

带着这个问题读：用模型自己滚出的历史训练，怎样处理自回归误差累积？

初读判断：训练部署差异的处理明确；属于视频生成基础，与机器人性能分别记录。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 84 | 20% |
| 学术影响 | 44.4 | 10% |
| 近期关注 | 88.7 | 5% |
| 复用价值 | 87 | 8% |
| 阅读价值 | 86 | 7% |

刊会依据：[NeurIPS 2025](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion。累计被引 **34**，2025–2026 被引 **34**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4417136857) · [文献计量条目](https://openalex.org/W4417136857)

### 影响与关注的计算依据

- **学术影响 44.4**：身份匹配的累计引用C=34，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4417136857)
- **近期关注 88.7**：近期窗口内创建的专属论文仓库，快照star=3538；按10000上限对数压缩。 [依据1](https://api.github.com/repos/guandeh17/Self-Forcing) · [依据2](https://raw.githubusercontent.com/guandeh17/Self-Forcing/main/README.md)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/guandeh17/Self-Forcing) | GitHub Star 3538；GitHub Watch订阅 22；GitHub Fork 285 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/gdhe17/Self-Forcing) | HF 最近30天下载 16110；HF 仓库累计点赞 131 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2506.08009) | HF 论文累计点赞 32 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
