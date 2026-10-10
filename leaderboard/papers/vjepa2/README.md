# V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning

**V-JEPA 2** · arXiv 2025 · 本版排名 88 · 综合分 **81.9 / 100**

[解读导读](../../../library/vjepa2.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [arXiv集锦](../../../arxiv/README.md#paper-vjepa2)

[原文](https://arxiv.org/abs/2506.09985) · [PDF](https://arxiv.org/pdf/2506.09985) · [阅读卡片](../../../library/vjepa2.md)

论文出处：[**Mahmoud Assran**](../../origins/papers/vjepa2.md)<br>[Meta FAIR 研究院 / 魁北克人工智能研究所（Mila） · 另1个机构](../../origins/papers/vjepa2.md)

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
| 公开与评审 | 60 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 84.4 | 10% |
| 近期关注 | 100.0 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 97 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：原文方法与实验选题初读；非全文精读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning。累计被引 **859**，2025–2026 被引 **至少 832**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2506.09985) · [文献计量条目](https://www.semanticscholar.org/paper/b202faf38efbffcb26470c702e1140b047d6f6e7)

### 影响与关注的计算依据

- **学术影响 84.4**：身份匹配的累计引用C=859，对数压缩上限3000。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2506.09985)
- **近期关注 100.0**：近期已定位引用R=832；数量与每月引用速度各占一半，有效观察期15.9671个月。 [依据1](https://api.semanticscholar.org/graph/v1/paper/b202faf38efbffcb26470c702e1140b047d6f6e7/citations)

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/facebookresearch/jepa) | GitHub Star 4173；GitHub Watch订阅 52；GitHub Fork 423 | 其他研究入口；截至2026-10-10的累计快照 | 2026-10-10 |
| [github](https://github.com/facebookresearch/vjepa2) | GitHub Star 4744；GitHub Watch订阅 54；GitHub Fork 589 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/facebook/vjepa2-vitg-fpc64-256) | HF 最近30天下载 92830；HF 仓库累计点赞 57 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2506.09985) | HF 论文累计点赞 36 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [linkedin](https://www.linkedin.com/posts/aiatmeta_were-sharing-v-jepa-2-a-new-world-model-activity-7338575662955286528-V6IJ) | Reactions 2701；Comments 75 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:21:08.510882+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
