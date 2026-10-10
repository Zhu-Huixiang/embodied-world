# An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale

本版阅读优先顺序：4；综合分：95.7 / 100；已评分权重：100%。

[原文](https://iclr.cc/virtual/2021/poster/3013) · [PDF](https://arxiv.org/pdf/2010.11929v2) · [阅读卡片](../../../library/vit.md)

## 机制简析

将图像切成固定大小的 patch，每块展平后线性投影为 token，再加入位置编码送进标准 Transformer。原文以大规模监督预训练和小规模下游微调测试数据规模与视觉归纳偏置的关系。实验覆盖 ImageNet、CIFAR 和 VTAB，机器人中的视觉 backbone 是这条表示路线的后续应用。

带着这个问题读：一张图怎样变成 token 序列，机器人策略拿到的视觉特征来自哪一步？

初读判断：架构变化直接，数据规模与 CNN 对照有解释力，权重与微调实现公开；先读能减少后续 VLA 编码器的理解负担。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 96 | 20% |
| 实验与证据 | 92 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[ICLR 2021](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://iclr.cc/virtual/2021/poster/3013)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale。累计被引 21509，2025–2026 被引 5613；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W3094502228) · [文献计量条目](https://openalex.org/W3094502228)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
