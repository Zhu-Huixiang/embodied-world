# Attention Is All You Need

**Transformer** · NeurIPS 2017 · 本版排名 8 · 综合分 **94.3 / 100**

[原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html) · [PDF](https://papers.neurips.cc/paper_files/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf) · [阅读卡片](../../../library/attention.md)

## 机制简析

输入 token 先做词嵌入和位置编码，再由多头注意力计算每个位置该从哪些位置取信息。编码器使用全序列自注意力；解码器用因果遮罩阻止读取未来 token，并通过交叉注意力接收编码器输出。原文在两项 WMT 翻译任务比较质量、训练成本与不同注意力配置。

带着这个问题读：Q、K、V 到底在计算什么，为什么这套序列计算能连接视觉、语言和动作？

初读判断：纯注意力替代循环网络的计算改动清晰，翻译对照和结构消融完整，官方实现公开；具身价值来自下游共享结构。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 99 | 20% |
| 实验与证据 | 94 | 20% |
| 学术影响 | 95 | 10% |
| 近期关注 | 60 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[NeurIPS 2017](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

影响与关注采用独立证据评分：

- **学术影响 95**：自注意力序列建模成为图像token与机器人动作块的共同架构前置；ACT原文明确采用Transformer并引用Vaswani2017，ViT采用标准Transformer编码器，π₀.₅继续将它用于多模态动作。这些跨表示/控制路线的直接采用支持共同基础档。 [依据1](https://www.roboticsproceedings.org/rss19/p016.pdf) · [依据2](https://arxiv.org/pdf/2010.11929v2) · [依据3](https://arxiv.org/html/2504.16054v1)
- **近期关注 60**：2025年的π₀.₅使用多模态Transformer和N×N注意力mask，V-JEPA 2采用ViT视频编码器并在位置编码比较中直接引用Vaswani2017；两条独立研究路线继续使用其结构，按多个方法采用档评分。 [依据1](https://arxiv.org/html/2504.16054v1) · [依据2](https://arxiv.org/html/2506.09985v1)

原始引用记录与编辑证据分分别保留，计算细则见评分说明。

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
