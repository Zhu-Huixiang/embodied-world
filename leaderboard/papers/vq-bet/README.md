# Behavior Generation with Latent Actions

**VQ-BeT** · ICML 2024 · 本版排名 89 · 综合分 **81.2 / 100**

[解读导读](../../../library/vq-bet.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [ICML集锦](../../../venues/ICML/README.md)

[原文](https://proceedings.mlr.press/v235/lee24y.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v235/main/assets/lee24y/lee24y.pdf) · [阅读卡片](../../../library/vq-bet.md)

## 机制简析

第一阶段用残差向量量化编码器把连续动作或动作块压成分层码，解码器还原动作；第二阶段 Transformer 根据观测与可选目标预测这些离散码和修正量。一次前向生成替代扩散多步去噪，同时保留行为分布的多种模式。原文比较条件/无条件任务、仿真和真实长程操作，以及推理时延。

带着这个问题读：动作先压成分层离散码，能否保留多种操作方式，同时省掉扩散反复采样？

初读判断：ICML 正式稿与项目提供与 BeT、Diffusion Policy 的多任务和速度对照，真实长程任务与开放实现支撑复用；部分任务没有优势，评分以整体机制和证据覆盖为准。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 17.3 | 10% |
| 近期关注 | 22.3 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[ICML 2024](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v235/lee24y.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Behavior Generation with Latent Actions。累计被引 3，2025–2026 被引 3；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4392538920) · [文献计量条目](https://openalex.org/W4392538920)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
