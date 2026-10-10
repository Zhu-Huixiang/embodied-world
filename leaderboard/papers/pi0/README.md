# π₀: A Vision-Language-Action Flow Model for General Robot Control

**π₀** · RSS 2025 · 本版排名 31 · 综合分 **88.7 / 100**

[解读导读](../../../library/pi0.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss21/p010.html) · [PDF](https://www.roboticsproceedings.org/rss21/p010.pdf) · [阅读卡片](../../../library/pi0.md)

论文出处：[Physical Intelligence · Physical Intelligence](../../origins/papers/pi0.md)

## 机制简析

视觉语言骨干提供语义条件，Flow Matching 动作专家生成连续动作块，再按闭环观测更新。

带着这个问题读：Flow Matching 动作专家怎样接收视觉语言条件？

初读判断：通用VLA与连续动作块的重要接口；适合逐项拆多本体数据和任务协议。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 90 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 69.5 | 10% |
| 近期关注 | 83.1 | 5% |
| 复用价值 | 88 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[RSS 2025](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss21/p010.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：π₀: A Vision-Language-Action Flow Model for General Robot Control。累计被引 **260**，2025–2026 被引 **260**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4414079054) · [文献计量条目](https://openalex.org/W4414079054)

### 影响与关注的计算依据

- **学术影响 69.5**：身份匹配的累计引用C=260，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4414079054)
- **近期关注 83.1**：huggingface 的论文专属入口：HF 仓库累计点赞=310；按1000上限对数压缩。 [依据1](https://huggingface.co/api/models/lerobot/pi0_old) · [依据2](https://huggingface.co/lerobot/pi0_old/raw/main/README.md) · [依据3](https://huggingface.co/lerobot/pi0_old)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/Physical-Intelligence/openpi) | GitHub Star 14155；GitHub Watch订阅 99；GitHub Fork 2536 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/lerobot/pi0_old) | HF 最近30天下载 402；HF 仓库累计点赞 310 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2410.24164) | HF 论文累计点赞 31 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
