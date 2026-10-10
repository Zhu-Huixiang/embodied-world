# ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills

**ASAP** · RSS 2025 · 本版排名 43 · 综合分 **87.1 / 100**

[解读导读](../../../library/asap.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss21/p066.html) · [PDF](https://agile.human2humanoid.com/static/asap.pdf) · [阅读卡片](../../../library/asap.md)

## 机制简析

先在模拟里训练人类动作跟踪策略，再在实机执行并记录轨迹。用真实轨迹训练 delta action 模型，找出能让模拟运动贴近真实运动的动作修正，把它接回模拟器后微调跟踪策略。原文比较跨模拟器和 Unitree G1 实机迁移，并对照系统辨识、域随机化与动力学残差。

带着这个问题读：模拟和实机差一点，为什么补动作残差比盲目加大随机化更有针对性？

初读判断：正式 RSS、两阶段数据链路明确，跨模拟器和实机与多种差距补偿基线比较；追读时能细讲残差学习而非只看动作视频。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 50.0 | 10% |
| 近期关注 | 64.5 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[RSS 2025](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss21/p066.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills。累计被引 54，2025–2026 被引 54；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4414051111) · [文献计量条目](https://openalex.org/W4414051111)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
