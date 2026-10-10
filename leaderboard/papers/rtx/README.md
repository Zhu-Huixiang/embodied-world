# Open X-Embodiment: Robotic Learning Datasets and RT-X Models

**Open X-Embodiment** · ICRA 2024 · 本版排名 58 · 综合分 **84.8 / 100**

[解读导读](../../../library/rtx.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [ICRA集锦](../../../venues/ICRA/README.md)

[原文](https://ieeexplore.ieee.org/document/10611477) · [PDF](https://arxiv.org/pdf/2310.08864) · [阅读卡片](../../../library/rtx.md)

论文出处：[Open X-Embodiment Collaboration · Open X-Embodiment Collaboration / Stanford IRIS（Intelligence through Robotic Interaction at Scale） 等12个出处](../../origins/papers/rtx.md)

## 机制简析

先把各实验室的轨迹变成统一数据格式，并以夹爪参考系中的位置、姿态和夹爪开合统一动作接口；未使用的动作分量按数据约定处理。RT-1-X 和 RT-2-X 在这个混合数据上训练，再与各机器人自己的专用数据策略比较。它检验的不是同一机器人多收点数据，而是别的机器人经验能否改善当前机器人。

带着这个问题读：不同机器人的动作坐标和观测并不一致，怎样把它们混成能产生正迁移的数据？

初读判断：IEEE 正式入口确认 ICRA，官方奖项页确认获奖，原项目给出多平台正迁移及 RT-2-X 新技能测试；标准化数据和开放代码具有直接复用价值。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 83.0 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 57.9 | 10% |
| 近期关注 | 42.0 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[ICRA 2024](../../../venues/ICRA/README.md)，正式出处见[出版/原文记录](https://ieeexplore.ieee.org/document/10611477)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Open X-Embodiment: Robotic Learning Datasets and RT-X Models。累计被引 **102**，2025–2026 被引 **37**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4387764390) · [文献计量条目](https://openalex.org/W4387764390)

### 影响与关注的计算依据

- **学术影响 57.9**：身份匹配的累计引用C=102，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4387764390)
- **近期关注 42.0**：近期已定位引用R=37；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4387764390)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/google-deepmind/open_x_embodiment) | GitHub Star 2059；GitHub Watch订阅 28；GitHub Fork 129 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2310.08864) | HF 论文累计点赞 3 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
