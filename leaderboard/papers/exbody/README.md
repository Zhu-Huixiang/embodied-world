# Expressive Whole-Body Control for Humanoid Robots

**ExBody** · RSS 2024 · 本版排名 47 · 综合分 **85.9 / 100**

[解读导读](../../../library/exbody.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss20/p107.html) · [PDF](https://www.roboticsproceedings.org/rss20/p107.pdf) · [阅读卡片](../../../library/exbody.md)

论文出处：[Xuxin Cheng / Yandong Ji · University of California San Diego / MIT 等3个出处](../../origins/papers/exbody.md)

## 机制简析

从人类动作库筛选并重定向姿态，训练时要求机器人上半身跟随关节和关键点目标。下半身放松逐关节模仿约束，改为跟随根速度和姿态命令，以留出平衡和行走空间。原文对照完整身体跟踪、分开策略与初始化方式，实机展示行走和表达动作。

带着这个问题读：上半身想照着人动，下半身还得站稳，这两种目标怎么兼容？

初读判断：正式 RSS，核心约束改动与完整跟踪基线直接比较，sim-to-real 与实机动作支持其科学问题。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 56.3 | 10% |
| 近期关注 | 54.5 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p107.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Expressive Whole-Body Control for Humanoid Robots。累计被引 **90**，2025–2026 被引 **77**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4402354017) · [文献计量条目](https://openalex.org/W4402354017)

### 影响与关注的计算依据

- **学术影响 56.3**：身份匹配的累计引用C=90，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4402354017)
- **近期关注 54.5**：近期已定位引用R=77；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4402354017)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/chengxuxin/expressive-humanoid) | GitHub Star 499；GitHub Watch订阅 8；GitHub Fork 38 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2402.16796) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
