# DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset

**DROID** · RSS 2024 · 本版排名 25 · 综合分 **90.1 / 100**

[解读导读](../../../library/droid.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss20/p120.html) · [PDF](https://www.roboticsproceedings.org/rss20/p120.pdf) · [阅读卡片](../../../library/droid.md)

论文出处：[**Alexander Khazatsky / Karl Pertsch**](../../origins/papers/droid.md)<br>[斯坦福 IRIS 实验室 / 伯克利 RAIL 实验室 · 另14个机构](../../origins/papers/droid.md)

## 机制简析

不同机构使用一致的机械臂、相机与遥操作平台，把设备移到大量真实场景收集示范，保存同步视觉、动作、语言及相机标定。训练时混入这些跨场景经验，再测试任务性能、鲁棒性与泛化。可迁移的核心不只是轨迹数量，而是场景、相机与交互位置覆盖。

带着这个问题读：机器人长期困在少数桌面场景里，分布式真实数据能把泛化边界推远多少？

初读判断：RSS 论文与项目给出跨环境数据分布、策略训练证据、开放数据/硬件及校准更新，具备实质可复用基础设施；数据贡献与算法创新分开评价。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 61.9 | 10% |
| 近期关注 | 94.2 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p120.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset。累计被引 **141**，2025–2026 被引 **137**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4402354047) · [文献计量条目](https://openalex.org/W4402354047)

### 影响与关注的计算依据

- **学术影响 61.9**：身份匹配的累计引用C=141，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4402354047)
- **近期关注 94.2**：huggingface 的论文专属入口：HF 最近30天下载=51341；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/cadene/droid) · [依据2](https://huggingface.co/datasets/cadene/droid/raw/main/README.md) · [依据3](https://huggingface.co/datasets/cadene/droid)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/droid-dataset/droid) | GitHub Star 448；GitHub Watch订阅 8；GitHub Fork 100 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [github](https://github.com/droid-dataset/droid_policy_learning) | GitHub Star 305；GitHub Watch订阅 5；GitHub Fork 30 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/cadene/droid) | HF 最近30天下载 51341；HF 仓库累计点赞 29 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2403.12945) | HF 论文累计点赞 2 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
