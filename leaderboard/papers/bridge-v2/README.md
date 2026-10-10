# BridgeData V2: A Dataset for Robot Learning at Scale

**BridgeData V2** · CoRL 2023 · 本版排名 78 · 综合分 **83.1 / 100**

[解读导读](../../../library/bridge-v2.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v229/walke23a.html) · [PDF](https://proceedings.mlr.press/v229/walke23a/walke23a.pdf) · [阅读卡片](../../../library/bridge-v2.md)

论文出处：[Homer Walke · UC Berkeley / Stanford University 等4个出处](../../origins/papers/bridge-v2.md)

## 机制简析

统一低成本机械臂平台收集语言标注轨迹，同时主动变化物体、相机、场景和工作台位置。策略可按目标图或自然语言训练，测试再拆开已见任务的视觉变化与新物体、新环境泛化。不同离线学习方法、数据规模和模型容量在同一数据上比较，让数据多样性的作用有可检查的落点。

带着这个问题读：机器人数据怎样覆盖场景差异，才会支持跨环境与跨机构技能迁移？

初读判断：CoRL 正式版与项目提供多环境数据、多个离线算法及数据/容量研究，开放数据、预训练模型和硬件指南复用价值很高；贡献主要在可泛化数据基础设施。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 32.0 | 10% |
| 近期关注 | 73.7 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 90 | 7% |

刊会依据：[CoRL 2023](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v229/walke23a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：BridgeData V2: A Dataset for Robot Learning at Scale。累计被引 **12**，2025–2026 被引 **3**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4386185624) · [文献计量条目](https://openalex.org/W4386185624)

### 影响与关注的计算依据

- **学术影响 32.0**：身份匹配的累计引用C=12，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4386185624)
- **近期关注 73.7**：huggingface 的论文专属入口：HF 最近30天下载=4829；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/nvidia/BridgeData2_LeRobot_v3) · [依据2](https://huggingface.co/datasets/nvidia/BridgeData2_LeRobot_v3/raw/main/README.md) · [依据3](https://huggingface.co/datasets/nvidia/BridgeData2_LeRobot_v3)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/rail-berkeley/bridge_data_v2) | GitHub Star 292；GitHub Watch订阅 11；GitHub Fork 35 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/nvidia/BridgeData2_LeRobot_v3) | HF 最近30天下载 4829；HF 仓库累计点赞 12 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2308.12952) | HF 论文累计点赞 3 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
