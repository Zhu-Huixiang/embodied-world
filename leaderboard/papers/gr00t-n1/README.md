# GR00T N1: An Open Foundation Model for Generalist Humanoid Robots

**GR00T N1** · arXiv 2025 · 本版排名 103 · 综合分 **51.9 / 100**

[解读导读](../../../library/gr00t-n1.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [arXiv集锦](../../../arxiv/README.md#paper-gr00t-n1)

[原文](https://arxiv.org/abs/2503.14734) · [PDF](https://arxiv.org/pdf/2503.14734v2) · [阅读卡片](../../../library/gr00t-n1.md)

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
| 发表与刊会 | 0 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 22.4 | 10% |
| 近期关注 | 28.8 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 92 | 7% |

发表与刊会：预印本公开，正式发表贡献记0；创新与实验单独计分。


编辑深度：原文机制与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：GR00T N1: An Open Foundation Model for Generalist Humanoid Robots。累计被引 5，2025–2026 被引 5；快照：2026-10-10T11:42:48+08:00。

[指标记录](https://api.openalex.org/works/W4414901575) · [文献计量条目](https://openalex.org/W4414901575)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
