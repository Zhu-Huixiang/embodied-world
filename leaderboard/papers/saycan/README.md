# Do As I Can, Not As I Say: Grounding Language in Robotic Affordances

**SayCan** · CoRL 2022 · 本版排名 36 · 综合分 **87.7 / 100**

[解读导读](../../../library/saycan.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v205/ichter23a.html) · [PDF](https://proceedings.mlr.press/v205/ichter23a/ichter23a.pdf) · [阅读卡片](../../../library/saycan.md)

论文出处：[Michael Ahn · Robotics at Google / Everyday Robots](../../origins/papers/saycan.md)

## 机制简析

高层指令与已执行步骤送给语言模型，为每个候选技能估计它对任务的适用性；技能价值函数再估计当前场景下的执行成功可能。两者合并后选择技能、实际执行并把步骤加入上下文，直到选出结束。原文分开报告计划与执行，因而能看清语言推理和物理技能各自卡在哪里。

带着这个问题读：语言模型觉得该做的事，机器人做得到吗？两个概率相乘到底解决什么？

初读判断：PMLR 正式论文与项目页给出真实厨房任务、语言模型替换、可供性约束实例及开源桌面版；创新是接口与组合机制，低层技能仍是独立预训练模块。

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
| 实验与证据 | 89 | 20% |
| 学术影响 | 78.0 | 10% |
| 近期关注 | 64.6 | 5% |
| 复用价值 | 79 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CoRL 2022](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v205/ichter23a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Do As I Can, Not As I Say: Grounding Language in Robotic Affordances。累计被引 **515**，2025–2026 被引 **133**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4224912544) · [文献计量条目](https://openalex.org/W4224912544)

### 影响与关注的计算依据

- **学术影响 78.0**：身份匹配的累计引用C=515，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4224912544)
- **近期关注 64.6**：近期已定位引用R=133；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4224912544)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/google-research/google-research) | GitHub Star 38887；GitHub Watch订阅 791；GitHub Fork 8476 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2204.01691) | HF 论文累计点赞 1 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
