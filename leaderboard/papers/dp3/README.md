# 3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations

**DP3** · RSS 2024 · 本版排名 48 · 综合分 **85.9 / 100**

[解读导读](../../../library/dp3.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss20/p067.html) · [PDF](https://www.roboticsproceedings.org/rss20/p067.pdf) · [阅读卡片](../../../library/dp3.md)

论文出处：[**Yanjie Ze / Gu Zhang**](../../origins/papers/dp3.md)<br>[清华具身智能实验室 / 上海期智研究院 · 另3个机构](../../origins/papers/dp3.md)

## 机制简析

以简洁点云编码器提供三维条件，用扩散生成动作，观察几何表示对泛化的影响。

带着这个问题读：简洁点云表示怎样改变操作策略的泛化？

初读判断：三维条件表示与动作生成分工容易拆；任务、点云处理与泛化协议需一起读。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 84 | 20% |
| 学术影响 | 67.0 | 10% |
| 近期关注 | 73.0 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 89 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p067.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：3D Diffusion Policy: Generalizable Visuomotor Policy Learning via Simple 3D Representations。累计被引 **213**，2025–2026 被引 **205**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4402354045) · [文献计量条目](https://openalex.org/W4402354045)

### 影响与关注的计算依据

- **学术影响 67.0**：身份匹配的累计引用C=213，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4402354045)
- **近期关注 73.0**：近期已定位引用R=205；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4402354045)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/papers/2403.03954) | HF 论文累计点赞 13 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [x](https://x.com/ZeYanjie/status/1765414787775963232?s=20) | Views 97375；Likes 296；Reposts 54；Replies 3；Quotes 12；Bookmarks 138 | 单篇论文入口；截至2026-10-10的累计快照 | 2026-10-10T15:21:08.510974+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
