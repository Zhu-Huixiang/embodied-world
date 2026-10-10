# RVT: Robotic View Transformer for 3D Object Manipulation

**RVT** · CoRL 2023 · 本版排名 101 · 综合分 **79.5 / 100**

[解读导读](../../../library/rvt.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v229/goyal23a.html) · [PDF](https://proceedings.mlr.press/v229/goyal23a/goyal23a.pdf) · [阅读卡片](../../../library/rvt.md)

论文出处：[Ankit Goyal · NVIDIA](../../origins/papers/rvt.md)

## 机制简析

RGB-D 先变成点云，再从机器人工作区周围的虚拟相机重渲染多张视图；Transformer 在视图内及视图间聚合信息。多视图动作热图反投影得到夹爪位置，其他头预测姿态与夹爪状态。原文把成功率、训练达到相同性能所需时间和推理速度分别与 PerAct 对比，并展示真实少示范操作。

带着这个问题读：体素太贵，重渲染几张虚拟视图能保住 3D 信息吗？

初读判断：PMLR 正式页给出 RLBench 与实机证据、PerAct 速度及成功率对照，代码和模型开放；新增表示的作用可通过直接对照讲清。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 24.3 | 10% |
| 近期关注 | 17.1 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 90 | 7% |

刊会依据：[CoRL 2023](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v229/goyal23a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：RVT: Robotic View Transformer for 3D Object Manipulation。累计被引 **6**，2025–2026 被引 **5**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4382334328) · [文献计量条目](https://openalex.org/W4382334328)

### 影响与关注的计算依据

- **学术影响 24.3**：身份匹配的累计引用C=6，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4382334328)
- **近期关注 17.1**：近期已定位引用R=5；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4382334328)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/nvlabs/rvt) | GitHub Star 409；GitHub Watch订阅 10；GitHub Fork 61 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2306.14896) | HF 论文累计点赞 2 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
