# FAST: Efficient Action Tokenization for Vision-Language-Action Models

**FAST** · RSS 2025 · 本版排名 64 · 综合分 **84.7 / 100**

[原文](https://www.roboticsproceedings.org/rss21/p012.html) · [PDF](https://www.roboticsproceedings.org/rss21/p012.pdf) · [阅读卡片](../../../library/fast.md)

## 机制简析

时间 DCT 提取动作频率系数，再量化和字节对编码，减少高频轨迹逐时刻离散产生的长序列。

带着这个问题读：为什么在时间频率域压缩，比逐时刻分箱更适合高频动作？

初读判断：压缩动作的表示选择清楚，跨策略应用与效率值得读；是Holo-M的直接前置。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 83 | 20% |
| 学术影响 | 51.9 | 10% |
| 近期关注 | 66.9 | 5% |
| 复用价值 | 85 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[RSS 2025](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss21/p012.html)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：FAST: Efficient Action Tokenization for Vision-Language-Action Models。累计被引 63，2025–2026 被引 63；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4414051084) · [文献计量条目](https://openalex.org/W4414051084)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
