# V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning

**V-JEPA 2** · arXiv 2025 · 本版排名 102 · 综合分 **54.1 / 100**

[解读导读](../../../library/vjepa2.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [arXiv集锦](../../../arxiv/README.md#paper-vjepa2)

[原文](https://arxiv.org/abs/2506.09985) · [PDF](https://arxiv.org/pdf/2506.09985) · [阅读卡片](../../../library/vjepa2.md)

## 机制简析

masked video encoder/EMA目标先学表征；冻结编码器后训300M block-causal 动作 predictor，自回归预测未来 latent；MPC 最小化目标图 latent L1。

带着这个问题读：先看无动作标签视频，再给少量机器人交互，潜空间怎样变成 Franka 规划器？

初读判断：22M视频预训练与62小时DROID交互分工清楚；两实验室Franka与摄像机/步长敏感性有证据。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 22.4 | 10% |
| 近期关注 | 28.8 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 97 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：原文方法与实验选题初读；非全文精读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning。累计被引 5，2025–2026 被引 5；快照：2026-10-10T11:44:51+08:00。

[指标记录](https://api.openalex.org/works/W4417261359) · [文献计量条目](https://openalex.org/W4417261359)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
