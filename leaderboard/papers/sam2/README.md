# SAM 2: Segment Anything in Images and Videos

**SAM 2** · ICLR 2025 · 本版排名 24 · 综合分 **90.6 / 100**

[原文](https://openreview.net/forum?id=Ha6RTeWMd0) · [PDF](https://proceedings.iclr.cc/paper_files/paper/2025/file/45c1f6a8cbf2da59ebf2c802b4f742cd-Paper-Conference.pdf) · [阅读卡片](../../../library/sam2.md)

## 机制简析

逐帧图像特征通过记忆注意力读取之前的目标提示与掩码信息，再与当前提示一起预测本帧掩码。记忆编码器把当前预测存入记忆，下一帧继续使用；静态图像相当于记忆为空的视频。原文比较交互次数、速度以及图像和视频分割基准。

带着这个问题读：目标在机器人视野里移动、遮挡后重现，过去的掩码记忆怎样帮它跟住对象？

初读判断：流式记忆和对象持续性问题直接，跨数据集与交互成本评估较完整，代码、模型及视频分割数据公开。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 69.7 | 10% |
| 近期关注 | 88.8 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[ICLR 2025](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://openreview.net/forum?id=Ha6RTeWMd0)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：SAM 2: Segment Anything in Images and Videos。累计被引 264，2025–2026 被引 249；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4401307635) · [文献计量条目](https://openalex.org/W4401307635)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
