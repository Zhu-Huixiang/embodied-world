# LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels

**LeWM** · arXiv 2026 · 本版排名 104 · 综合分 **48.2 / 100**

[原文](https://arxiv.org/abs/2603.19312v1) · [PDF](https://arxiv.org/pdf/2603.19312v1) · [阅读卡片](../../../library/lewm.md)

## 机制简析

ViT将每帧变成192维CLS表征；动作AdaLN条件的Transformer预测下个latent。MSE预测+SIGReg随机投影高斯正则共同训练，无EMA/stop-gradient/重建。部署用latent目标距离和CEM选动作，再MPC重规划。

带着这个问题读：两项损失怎样让像素JEPA不坍缩，又把每帧压成一个可规划的token？

初读判断：把原本依赖冻结基础视觉模型或多项正则的像素JEPA简化成清晰防坍缩目标；4个仿真环境、速度/固定预算、latent物理probe和消融充分。实机与长程控制覆盖仍窄，证据分不按基础模型规模或作者名抬高；开源资源完整。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 83 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 92 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：选题初读（方法、实验、相关附录）；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels。累计被引 0，2025–2026 被引 0；快照：2026-10-10T11:42:48+08:00。

[指标记录](https://api.openalex.org/works/W7140141371) · [文献计量条目](https://openalex.org/W7140141371)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
