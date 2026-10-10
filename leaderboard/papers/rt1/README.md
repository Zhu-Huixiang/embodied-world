# RT-1: Robotics Transformer for Real-World Control at Scale

**RT-1** · RSS 2023 · 本版排名 16 · 综合分 **91.2 / 100**

[解读导读](../../../library/rt1.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss19/p025.html) · [PDF](https://roboticsproceedings.org/rss19/p025.pdf) · [阅读卡片](../../../library/rt1.md)

论文出处：[**Anthony Brohan**](../../origins/papers/rt1.md)<br>[谷歌机器人研究团队 / Everyday Robots · 另1个机构](../../origins/papers/rt1.md)

## 机制简析

图像先经语言条件的 EfficientNet 提取特征，再由 TokenLearner 压成少量视觉 token；Transformer 融合短时历史并输出离散动作。动作同时覆盖机械臂、底盘和停止模式，策略以闭环方式反复读取图像。原文分别检验新指令、干扰物、新背景以及跨机器人数据混合的效果。

带着这个问题读：大量真实机器人数据究竟需要什么策略结构才能吃进去，TokenLearner 为何是关键？

初读判断：RSS 正式 PDF 与项目页给出 BC-Z、Gato 对照、数据量/数据多样性消融和真实厨房评估，证据丰富；开源模型和数据提供复用入口。

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
| 实验与证据 | 92 | 20% |
| 学术影响 | 80.9 | 10% |
| 近期关注 | 89.2 | 5% |
| 复用价值 | 86 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[RSS 2023](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss19/p025.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：RT-1: Robotics Transformer for Real-World Control at Scale。累计被引 **651**，2025–2026 被引 **464**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4385430679) · [文献计量条目](https://openalex.org/W4385430679)

### 影响与关注的计算依据

- **学术影响 80.9**：身份匹配的累计引用C=651，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4385430679)
- **近期关注 89.2**：近期已定位引用R=464；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4385430679)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/google-research/robotics_transformer) | GitHub Star 1741；GitHub Watch订阅 0；GitHub Fork 205 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2212.06817) | HF 论文累计点赞 6 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
