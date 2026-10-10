# EfficientZero V2: Mastering Discrete and Continuous Control with Limited Data

**EfficientZero V2** · ICML 2024 · 本版排名 106 · 综合分 **75.0 / 100**

[解读导读](../../../library/efficientzero-v2.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICML集锦](../../../venues/ICML/README.md)

[原文](https://proceedings.mlr.press/v235/wang24at.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v235/main/assets/wang24at/wang24at.pdf) · [阅读卡片](../../../library/efficientzero-v2.md)

论文出处：[Shengjie Wang / Shaohuai Liu 等3位 · Tsinghua University / Shanghai Qi Zhi Institute 等4个出处](../../origins/papers/efficientzero-v2.md)

## 机制简析

表示函数得到潜状态，动力学函数接收动作并预测潜状态与奖励，策略和值网络为搜索提供先验。连续动作下先采样候选动作，再用基于 Gumbel 的树搜索改善策略，并用搜索产生价值目标以利用旧经验。实验按有限交互预算比较离散和连续、图像和低维输入任务。

带着这个问题读：树搜索怎样跨过离散动作的限制，在连续控制里仍保持样本效率？

初读判断：正式 ICML Spotlight，原文跨三类基准并比较 DreamerV3；连续树搜索与价值估计分别有消融，初读评分保留为编辑判断。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 78 | 8% |
| 阅读价值 | 87 | 7% |

刊会依据：[ICML 2024](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v235/wang24at.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：EfficientZero V2: Mastering Discrete and Continuous Control with Limited Data。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4392427796) · [文献计量条目](https://openalex.org/W4392427796)

### 影响与关注的计算依据

- **学术影响 0.0**：身份匹配的累计引用C=0，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4392427796)
- **近期关注 0.0**：近期已定位引用R=0；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4392427796)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/Shengjiewang-Jason/EfficientZeroV2) | GitHub Star 124；GitHub Watch订阅 2；GitHub Fork 20 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2403.00564) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
