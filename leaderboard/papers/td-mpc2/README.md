# TD-MPC2: Scalable, Robust World Models for Continuous Control

**TD-MPC2** · ICLR 2024 · 本版排名 61 · 综合分 **84.7 / 100**

[解读导读](../../../library/td-mpc2.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://proceedings.iclr.cc/paper_files/paper/2024/hash/cf73d57b6dcda32b293df7c2d5341f49-Abstract-Conference.html) · [PDF](https://proceedings.iclr.cc/paper_files/paper/2024/file/cf73d57b6dcda32b293df7c2d5341f49-Paper-Conference.pdf) · [阅读卡片](../../../library/td-mpc2.md)

论文出处：[Nicklas Hansen · University of California San Diego](../../origins/papers/td-mpc2.md)

## 机制简析

共享潜世界模型、价值和规划结构跨多任务学习，处理不同奖励尺度与动作空间。

带着这个问题读：多任务潜空间规划怎样处理不同动作空间和奖励尺度？

初读判断：大范围连续控制与复用实现有优势；重要的是任务配置和计算预算。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 92 | 20% |
| 学术影响 | 27.4 | 10% |
| 近期关注 | 62.1 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[ICLR 2024](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://proceedings.iclr.cc/paper_files/paper/2024/hash/cf73d57b6dcda32b293df7c2d5341f49-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本；匹配题目：TD-MPC2: Scalable, Robust World Models for Continuous Control。累计被引 **8**，2025–2026 被引 **7**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4387964172) · [文献计量条目](https://openalex.org/W4387964172)

### 影响与关注的计算依据

- **学术影响 27.4**：身份匹配的累计引用C=8，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4387964172)
- **近期关注 62.1**：huggingface 的论文专属入口：HF 最近30天下载=1275；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/nicklashansen/tdmpc2) · [依据2](https://huggingface.co/datasets/nicklashansen/tdmpc2/raw/main/README.md) · [依据3](https://huggingface.co/datasets/nicklashansen/tdmpc2)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/nicklashansen/tdmpc2) | GitHub Star 978；GitHub Watch订阅 7；GitHub Fork 212 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/nicklashansen/tdmpc2) | HF 最近30天下载 1275；HF 仓库累计点赞 8 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/nicklashansen/tdmpc2) | HF 最近30天下载 0；HF 仓库累计点赞 15 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2310.16828) | HF 论文累计点赞 8 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
