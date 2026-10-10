# Flow Matching for Generative Modeling

**Flow Matching** · ICLR 2023 · 本版排名 27 · 综合分 **90.0 / 100**

[解读导读](../../../library/flow-matching.md) · [Diffusion / Transformer 基础](../../../paper-map/README.md#track-diffusion-transformer) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://iclr.cc/virtual/2023/poster/11309) · [PDF](https://arxiv.org/pdf/2210.02747) · [阅读卡片](../../../library/flow-matching.md)

## 机制简析

给噪声与数据之间指定一个条件概率路径，直接回归该路径的目标速度场，训练时不用数值模拟完整 ODE。条件流匹配的目标在梯度层面对应难直接计算的边缘流目标；生成时才用求解器沿学习的速度场从噪声走向数据。原文比较扩散型路径与最优传输型插值，在 ImageNet 检查样本质量、似然和速度。

带着这个问题读：不模拟整条生成轨迹就能训练速度场，π₀ 里的 Flow Matching 损失怎样读？

初读判断：目标等价关系与路径选择构成明确创新，图像对照和通用实现完善；连续动作流匹配教程需要先把这套对象定义清楚。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 92 | 20% |
| 学术影响 | 58.4 | 10% |
| 近期关注 | 70.5 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 98 | 7% |

刊会依据：[ICLR 2023](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://iclr.cc/virtual/2023/poster/11309)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Flow Matching for Generative Modeling。累计被引 106，2025–2026 被引 79；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4303647933) · [文献计量条目](https://openalex.org/W4303647933)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
