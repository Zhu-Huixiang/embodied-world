# Deep Whole-Body Control: Learning a Unified Policy for Manipulation and Locomotion

**Deep WBC** · CoRL 2022 · 本版排名 89 · 综合分 **81.5 / 100**

[解读导读](../../../library/deep-whole-body-control.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v205/fu23a.html) · [PDF](https://proceedings.mlr.press/v205/fu23a/fu23a.pdf) · [阅读卡片](../../../library/deep-whole-body-control.md)

论文出处：[**Zipeng Fu / Xuxin Cheng**](../../origins/papers/deep-whole-body-control.md)<br>[卡内基梅隆大学](../../origins/papers/deep-whole-body-control.md)

## 机制简析

同一个网络接收底盘、腿、手臂状态和任务命令，输出六维手臂与十二维腿部关节目标，再由 PD 转为力矩。Advantage Mixing 把移动和操作的收益联系起来，Regularized Online Adaptation 对齐历史估计与训练环境信息。实验比较分开的控制器、未协调策略和适应方法，并在四足机械臂上验证。

带着这个问题读：手臂和腿一起出动作，怎样避免一边拿东西、一边把身体拽倒？

初读判断：有统一与分离策略直接对照、关键训练机制消融和完整实机系统，能具体说明全身控制为什么需要协同。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 41.2 | 10% |
| 近期关注 | 18.8 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[CoRL 2022](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v205/fu23a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Deep Whole-Body Control: Learning a Unified Policy for Manipulation and Locomotion。累计被引 **26**，2025–2026 被引 **6**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4306893292) · [文献计量条目](https://openalex.org/W4306893292)

### 影响与关注的计算依据

- **学术影响 41.2**：身份匹配的累计引用C=26，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4306893292)
- **近期关注 18.8**：近期已定位引用R=6；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4306893292)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/MarkFzp/Deep-Whole-Body-Control) | GitHub Star 404；GitHub Watch订阅 12；GitHub Fork 33 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
