# GR00T N1: An Open Foundation Model for Generalist Humanoid Robots

**GR00T N1** · arXiv 2025 · 本版排名 94 · 综合分 **80.4 / 100**

[解读导读](../../../library/gr00t-n1.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [arXiv集锦](../../../arxiv/README.md#paper-gr00t-n1)

[原文](https://arxiv.org/abs/2503.14734) · [PDF](https://arxiv.org/pdf/2503.14734v2) · [阅读卡片](../../../library/gr00t-n1.md)

论文出处：[**NVIDIA**](../../origins/papers/gr00t-n1.md)<br>[英伟达 GEAR 研究团队 / 英伟达](../../origins/papers/gr00t-n1.md)

## 机制简析

Eagle-2视觉语言middle-layer tokens→DiT交叉注意力；embodiment-specific MLP编码state与noisy action、解码H=16连续动作块，flow-matching训练、K=4步采样。人类latent-action、real robot、DexMimicGen模拟和生成视频IDM/LAPA伪动作组成数据金字塔。

带着这个问题读：Eagle-2视觉语言特征与连续动作流怎样分工，合成视频里的动作标签从哪来，预训练收益又在什么任务上成立？

初读判断：多本体、异源动作监督和公开系统是贡献，dual-system+flow action结构不是首创。24/9/24项仿真协议、GR-1实机与数据规模/神经轨迹消融可核；主任务短程tabletop，不代表全身loco-manipulation泛化，合成轨迹物理真实性与posttrain遗忘有代价。正式刊会未核，按原论文观察。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 91.5 | 10% |
| 近期关注 | 100.0 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 92 | 7% |

公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；当前阶段为预印本公开。


编辑深度：原文机制与实验初读；评分记录：2026-10-10。

计量来源：Semantic Scholar；原研究arXiv ID索引记录（版本合并）；匹配题目：GR00T N1: An Open Foundation Model for Generalist Humanoid Robots。累计被引 **1513**，2025–2026 被引 **至少 1476**；快照：2026-10-10。

[指标记录](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2503.14734) · [文献计量条目](https://www.semanticscholar.org/paper/731c50b0d6af4c1cb8d95f506541681ea487973b)

### 影响与关注的计算依据

- **学术影响 91.5**：身份匹配的累计引用C=1513，对数压缩上限3000。 [依据1](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2503.14734)
- **近期关注 100.0**：近期已定位引用R=1476；数量与每月引用速度各占一半，有效观察期18.7598个月。 [依据1](https://api.semanticscholar.org/graph/v1/paper/731c50b0d6af4c1cb8d95f506541681ea487973b/citations)

[其他计量来源快照](../../metrics.json)分别保留，不相加；本版按登记的身份匹配顺序选源。

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/NVIDIA/Isaac-GR00T) | GitHub Star 8183；GitHub Watch订阅 74；GitHub Fork 1489 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/nvidia/GR00T-N1-2B) | HF 最近30天下载 441；HF 仓库累计点赞 356 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2503.14734) | HF 论文累计点赞 9 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [linkedin](https://www.linkedin.com/feed/update/urn:li:activity:7307882855785762816) | Reactions 3632；Comments 126 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:17:58.888933+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
