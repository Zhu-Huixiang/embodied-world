# RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots

**RoboCasa** · RSS 2024 · 本版排名 76 · 综合分 **83.2 / 100**

[解读导读](../../../library/robocasa.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://roboticsproceedings.org/rss20/p050.html) · [PDF](https://www.roboticsproceedings.org/rss20/p050.pdf) · [阅读卡片](../../../library/robocasa.md)

论文出处：[Soroush Nasiriany · UT Austin Robot Perception and Learning Lab（RPL） / The University of Texas at Austin 等3个出处](../../origins/papers/robocasa.md)

## 机制简析

在厨房仿真中同时扩展可交互家具、物体、布局与视觉纹理，再把基础技能组合成长任务。人类示范与自动轨迹生成共同提供训练数据，模型在不同数据规模和任务条件下学习。原文的重点是模拟多样性和合成数据是否形成可测的性能增长，并探索向真实任务迁移。

带着这个问题读：真实数据太贵，家居仿真的场景、任务与示范各要扩到什么程度才有用？

初读判断：RSS PDF 提供场景/资产/任务/数据四支柱、规模实验与真实迁移线索，平台公开且持续维护；主干证据为仿真，真实迁移仍需逐项精读。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 17.3 | 10% |
| 近期关注 | 62.2 | 5% |
| 复用价值 | 97 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://roboticsproceedings.org/rss20/p050.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots。累计被引 **3**，2025–2026 被引 **3**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4399424845) · [文献计量条目](https://openalex.org/W4399424845)

### 影响与关注的计算依据

- **学术影响 17.3**：身份匹配的累计引用C=3，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4399424845)
- **近期关注 62.2**：huggingface 的论文专属入口：HF 最近30天下载=1283；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/nvidia/RoboCasa-Cosmos-Policy) · [依据2](https://huggingface.co/datasets/nvidia/RoboCasa-Cosmos-Policy/raw/main/README.md) · [依据3](https://huggingface.co/datasets/nvidia/RoboCasa-Cosmos-Policy)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/robocasa/robocasa) | GitHub Star 1794；GitHub Watch订阅 13；GitHub Fork 265 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/nvidia/RoboCasa-Cosmos-Policy) | HF 最近30天下载 1283；HF 仓库累计点赞 9 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2406.02523) | HF 论文累计点赞 11 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
