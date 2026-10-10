# Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware

**ACT / ALOHA** · RSS 2023 · 本版排名 14 · 综合分 **91.6 / 100**

[解读导读](../../../library/act.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss19/p016.html) · [PDF](https://www.roboticsproceedings.org/rss19/p016.pdf) · [阅读卡片](../../../library/act.md)

论文出处：[**Tony Z. Zhao**](../../origins/papers/act.md)<br>[斯坦福 IRIS 实验室 / 伯克利 RAIL 实验室 · 另1个机构](../../origins/papers/act.md)

## 机制简析

把一段动作联合预测，条件变分自编码器吸收示范差异，时间集成融合重叠预测减轻误差积累。

带着这个问题读：Action chunking 与时间集成怎样处理示范中的误差累积？

初读判断：低成本双臂硬件与动作分块相互支撑，适合同时读数据系统和策略。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 92 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 80.5 | 10% |
| 近期关注 | 93.5 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[RSS 2023](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss19/p016.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware。累计被引 **630**，2025–2026 被引 **544**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4385430674) · [文献计量条目](https://openalex.org/W4385430674)

### 影响与关注的计算依据

- **学术影响 80.5**：身份匹配的累计引用C=630，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4385430674)
- **近期关注 93.5**：huggingface 的论文专属入口：HF 最近30天下载=47499；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/lerobot/aloha_sim_insertion_human) · [依据2](https://huggingface.co/datasets/lerobot/aloha_sim_insertion_human/raw/main/README.md) · [依据3](https://huggingface.co/datasets/lerobot/aloha_sim_insertion_human)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/tonyzhaozh/act) | GitHub Star 2264；GitHub Watch订阅 19；GitHub Fork 426 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/lerobot/aloha_sim_insertion_human) | HF 最近30天下载 47499；HF 仓库累计点赞 13 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/lerobot/act_aloha_sim_transfer_cube_human) | HF 最近30天下载 2914；HF 仓库累计点赞 38 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2304.13705) | HF 论文累计点赞 9 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
