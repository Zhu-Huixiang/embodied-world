# RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control

**RT-2** · CoRL 2023 · 本版排名 69 · 综合分 **84.2 / 100**

[解读导读](../../../library/rt2.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v229/zitkovich23a.html) · [PDF](https://proceedings.mlr.press/v229/zitkovich23a/zitkovich23a.pdf) · [阅读卡片](../../../library/rt2.md)

论文出处：[Anthony Brohan · Google DeepMind](../../origins/papers/rt2.md)

## 机制简析

把机器人动作写成语言模型词表内的编号，将机器人示范与视觉语言任务共同训练以迁移网络语义。

带着这个问题读：文字和动作一起训练，网络知识怎样影响一次操作？

初读判断：把网络知识接入动作的早期路线；跨任务结果有启发，实施门槛较高。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 83 | 20% |
| 学术影响 | 69.8 | 10% |
| 近期关注 | 60.7 | 5% |
| 复用价值 | 68 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[CoRL 2023](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v229/zitkovich23a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本；匹配题目：RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control。累计被引 **267**，2025–2026 被引 **108**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4385473486) · [文献计量条目](https://openalex.org/W4385473486)

### 影响与关注的计算依据

- **学术影响 69.8**：身份匹配的累计引用C=267，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4385473486)
- **近期关注 60.7**：近期已定位引用R=108；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4385473486)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/papers/2307.15818) | HF 论文累计点赞 33 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
