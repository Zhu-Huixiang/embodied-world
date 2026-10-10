# DeepMimic: Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills

**DeepMimic** · SIGGRAPH / TOG 2018 · 本版排名 23 · 综合分 **90.2 / 100**

[解读导读](../../../library/deepmimic.md) · [动作先验与全身技能](../../../paper-map/README.md#track-motion-priors) · [SIGGRAPH / TOG集锦](../../../venues/SIGGRAPH-TOG/README.md)

[原文](https://xbpeng.github.io/projects/DeepMimic/) · [PDF](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf) · [阅读卡片](../../../library/deepmimic.md)

论文出处：[**Xue Bin Peng**](../../origins/papers/deepmimic.md)<br>[加州大学伯克利分校 / 不列颠哥伦比亚大学](../../origins/papers/deepmimic.md)

## 机制简析

任务奖励与参考动作跟踪奖励共同训练物理角色策略，使动作技能能在动态扰动后恢复。

带着这个问题读：模仿奖励与任务奖励怎样把动作片段变成可恢复的控制技能？

初读判断：示范驱动物理控制的基础路线；公开实现利于机制实验。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.4 | 30% |
| 创新性 | 96 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 85.1 | 10% |
| 近期关注 | 73.0 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[SIGGRAPH / TOG 2018](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://xbpeng.github.io/projects/DeepMimic/)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：DeepMimic。累计被引 **906**，2025–2026 被引 **206**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W2796290181) · [文献计量条目](https://openalex.org/W2796290181)

### 影响与关注的计算依据

- **学术影响 85.1**：身份匹配的累计引用C=906，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W2796290181)
- **近期关注 73.0**：近期已定位引用R=206；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W2796290181)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/xbpeng/DeepMimic) | GitHub Star 3109；GitHub Watch订阅 104；GitHub Fork 533 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [github](https://github.com/xbpeng/MimicKit) | GitHub Star 2372；GitHub Watch订阅 27；GitHub Fork 294 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/1804.02717) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
