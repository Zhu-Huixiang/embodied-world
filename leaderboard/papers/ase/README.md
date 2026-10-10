# ASE: Large-Scale Reusable Adversarial Skill Embeddings for Physically Simulated Characters

**ASE** · SIGGRAPH / TOG 2022 · 本版排名 52 · 综合分 **85.5 / 100**

[解读导读](../../../library/ase.md) · [动作先验与全身技能](../../../paper-map/README.md#track-motion-priors) · [SIGGRAPH / TOG集锦](../../../venues/SIGGRAPH-TOG/README.md)

[原文](https://xbpeng.github.io/projects/ASE/) · [PDF](https://xbpeng.github.io/projects/ASE/ASE_2022.pdf) · [阅读卡片](../../../library/ase.md)

论文出处：[**Xue Bin Peng**](../../origins/papers/ase.md)<br>[加州大学伯克利分校 / 英伟达 · 另1个机构](../../origins/papers/ase.md)

## 机制简析

将潜技能条件与对抗动作先验联合训练，再让高层策略选择可复用的技能嵌入。

带着这个问题读：连续技能潜变量怎样组织可重复使用的动作？

初读判断：可复用技能接口值得与机器人动作latent比较；初读分清训练奖励和高层控制。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.4 | 30% |
| 创新性 | 90 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 67.4 | 10% |
| 近期关注 | 60.1 | 5% |
| 复用价值 | 88 | 8% |
| 阅读价值 | 91 | 7% |

刊会依据：[SIGGRAPH / TOG 2022](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://xbpeng.github.io/projects/ASE/)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：ASE。累计被引 **219**，2025–2026 被引 **105**；快照：2026-10-10T11:39:22+08:00。

[指标记录](https://api.openalex.org/works/W4229044820) · [文献计量条目](https://openalex.org/W4229044820)

### 影响与关注的计算依据

- **学术影响 67.4**：身份匹配的累计引用C=219，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4229044820)
- **近期关注 60.1**：近期已定位引用R=105；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4229044820)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/nv-tlabs/ASE) | GitHub Star 1128；GitHub Watch订阅 20；GitHub Fork 152 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [github](https://github.com/xbpeng/MimicKit) | GitHub Star 2372；GitHub Watch订阅 27；GitHub Fork 294 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
