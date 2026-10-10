# Modality-Autoregressive World-Action Models

**ModAR** · arXiv 2026 · 本版排名 107 · 综合分 **46.9 / 100**

[原文](https://arxiv.org/abs/2609.17524v1) · [PDF](https://arxiv.org/pdf/2609.17524v1) · [阅读卡片](../../../library/modar.md)

## 机制简析

共享DiT把当前DINO/深度/RGB和配置/任务条件融合，按点轨迹→DINO→深度→RGB块自回归去噪，动作最后生成；上下文加噪避免前一模态误差层层放大。实机去掉收益最小的未来RGB。

带着这个问题读：为什么先预测点轨迹、语义与几何，再给动作，可能比视频动作一起去噪更有效？

初读判断：新意在模态顺序和可控比较，独立IDM、匹配40采样步、模态/顺序/上下文噪声消融支撑机制。实机3任务90rollouts每模型，总体外推有限；仅比较一个反序，按best checkpoint在同批held-out条件报数，不能当跨域无偏评估。代码可复用情况未完整核，reuse不按想象给高分。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 85 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 72 | 8% |
| 阅读价值 | 94 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：选题初读（方法、实验与消融）；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Modality-Autoregressive World-Action Models。累计被引 0，2025–2026 被引 0；快照：2026-10-10T11:42:48+08:00。

[指标记录](https://api.openalex.org/works/W7213403652) · [文献计量条目](https://openalex.org/W7213403652)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
