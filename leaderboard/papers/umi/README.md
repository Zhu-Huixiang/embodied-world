# Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots

**UMI** · RSS 2024 · 本版排名 21 · 综合分 **90.5 / 100**

[解读导读](../../../library/umi.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss20/p045.html) · [PDF](https://www.roboticsproceedings.org/rss20/p045.pdf) · [阅读卡片](../../../library/umi.md)

论文出处：[Cheng Chi / Zhenjia Xu · Stanford University / Columbia University 等3个出处](../../origins/papers/umi.md)

## 机制简析

手持夹爪上的相机与位姿追踪记录人类示范，政策学习使用相对末端轨迹而非绑定某机器人底座的绝对坐标。部署时匹配观测与动作延迟，双臂任务再加入夹爪之间的相对位置，以保证示范和执行接口一致。抛掷、杯子摆放、衣物折叠与洗碗实验分别检验这些设计。

带着这个问题读：拿手持夹爪采示范，怎样跨过人类手速、机器人延迟和坐标系之间的鸿沟？

初读判断：RSS 正式版与项目包含延迟匹配、相对动作、双夹爪信息的消融和跨硬件实机任务，开放硬件与软件教程，兼具创新和传播价值。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 64.5 | 10% |
| 近期关注 | 68.1 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 98 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p045.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots。累计被引 **174**，2025–2026 被引 **160**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4402354127) · [文献计量条目](https://openalex.org/W4402354127)

### 影响与关注的计算依据

- **学术影响 64.5**：身份匹配的累计引用C=174，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4402354127)
- **近期关注 68.1**：近期已定位引用R=160；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4402354127)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/real-stanford/universal_manipulation_interface) | GitHub Star 1600；GitHub Watch订阅 19；GitHub Fork 291 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2402.10329) | HF 论文累计点赞 15 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
