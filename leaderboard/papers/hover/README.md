# HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots

**HOVER** · ICRA 2025 · 本版排名 100 · 综合分 **79.6 / 100**

[解读导读](../../../library/hover.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [ICRA集锦](../../../venues/ICRA/README.md)

[原文](https://hover-versatile-humanoid.github.io/) · [PDF](https://arxiv.org/pdf/2410.21229) · [阅读卡片](../../../library/hover.md)

论文出处：[Tairan He / Wenli Xiao · NVIDIA GEAR / NVIDIA 等6个出处](../../origins/papers/hover.md)

## 机制简析

先训练全身 motion oracle；上/下身模式与稀疏 mask 改写任务命令，本体观测 mask 改写状态；DAgger 用 oracle 动作监督学生访问状态，得到一个统一低层策略。

带着这个问题读：一个全身策略怎样接住关节、身体位置、根速度等不同格式的指令？

初读判断：19-DOF 人形和15种以上命令模式有 specialist 对照；预设模式覆盖与自动高层任务规划分开。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 83.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 40.2 | 10% |
| 近期关注 | 35.5 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[ICRA 2025](../../../venues/ICRA/README.md)，正式出处见[出版/原文记录](https://hover-versatile-humanoid.github.io/)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文方法与实验选题初读；非全文精读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots。累计被引 **24**，2025–2026 被引 **24**；快照：2026-10-10T11:44:51+08:00。

[指标记录](https://api.openalex.org/works/W4413918871) · [文献计量条目](https://openalex.org/W4413918871)

### 影响与关注的计算依据

- **学术影响 40.2**：身份匹配的累计引用C=24，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4413918871)
- **近期关注 35.5**：近期已定位引用R=24；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4413918871)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/NVlabs/HOVER) | GitHub Star 765；GitHub Watch订阅 19；GitHub Fork 91 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2410.21229) | HF 论文累计点赞 5 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
