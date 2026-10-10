# LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels

**LeWM** · arXiv 2026 · 本版排名 91 · 综合分 **81.2 / 100**

[解读导读](../../../library/lewm.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [arXiv集锦](../../../arxiv/README.md#paper-lewm)

[原文](https://arxiv.org/abs/2603.19312v1) · [PDF](https://arxiv.org/pdf/2603.19312v1) · [阅读卡片](../../../library/lewm.md)

论文出处：[**Lucas Maes / Quentin Le Lidec**](../../origins/papers/lewm.md)<br>[魁北克人工智能研究所（Mila） / 纽约大学 · 另2个机构](../../origins/papers/lewm.md)

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
| 公开与评审 | 70 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 83 | 20% |
| 学术影响 | 70.4 | 10% |
| 近期关注 | 99.8 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 92 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。；独立公开技术检验阶段70，取较高阶段。


编辑深度：选题初读（方法、实验、相关附录）；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels。累计被引 **280**，2025–2026 被引 **至少 277**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2603.19312) · [文献计量条目](https://www.semanticscholar.org/paper/530dab86cb8034bc12a32d21508aaa3f2cc00aa1)

### 影响与关注的计算依据

- **学术影响 70.4**：身份匹配的累计引用C=280，对数压缩上限3000。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2603.19312)
- **近期关注 99.8**：x 的论文专属入口：Views=979252；按1000000上限对数压缩。 [依据1](https://x.com/lucasmaes_/status/2036080584569618741)

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/lucas-maes/le-wm) | GitHub Star 4508；GitHub Watch订阅 50；GitHub Fork 664 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/quentinll/lewm-cube) | HF 最近30天下载 5114；HF 仓库累计点赞 2 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/quentinll/lewm-pusht) | HF 最近30天下载 5467；HF 仓库累计点赞 12 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2603.19312) | HF 论文累计点赞 56 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/quentinll/lewm-pusht) | HF 最近30天下载 3967；HF 仓库累计点赞 15 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [linkedin](https://www.linkedin.com/posts/lucas-maes-736983307_jepa-are-finally-easy-to-train-end-to-end-activity-7441855287990325249-AnZF) | Reactions 1139；Comments 22 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:17:58.829984+08:00 |
| [x](https://x.com/lucasmaes_/status/2036080584569618741) | Views 979252；Likes 3984；Reposts 560；Replies 109；Quotes 101；Bookmarks 3553 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:17:59.066406+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
