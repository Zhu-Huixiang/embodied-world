# Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion

本版阅读优先顺序：16；综合分：83.8 / 100；已评分权重：100%。

[原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/f4823f831af67a3ef15e41a85434422a-Paper-Conference.pdf) · [阅读卡片](../../../library/self-forcing.md)

## 机制简析

使用模型自己的历史滚动来训练自回归视频生成，减少教师历史与部署历史的分布差异。

带着这个问题读：用模型自己滚出的历史训练，怎样处理自回归误差累积？

初读判断：训练部署差异的处理明确；属于视频生成基础，与机器人性能分别记录。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 84 | 20% |
| 学术影响 | 44.4 | 10% |
| 近期关注 | 57.2 | 5% |
| 复用价值 | 87 | 8% |
| 阅读价值 | 86 | 7% |

刊会依据：[NeurIPS 2025](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html)；采用2026-10-09刊会快照。


编辑深度：选题初读；评分记录：2026-10-09T18:35:28+08:00。

计量版本：正式刊会版本；OpenAlex题目：Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion。累计被引 34，2025–2026 被引 34；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4417136857) · [文献计量条目](https://openalex.org/W4417136857)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
