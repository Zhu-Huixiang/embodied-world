# A review of learning-based dynamics models for robotic manipulation

**Dynamics Review** · Sci. Robot. 2025 · 本版排名 95 · 综合分 **80.3 / 100**

[解读导读](../../../library/learned-dynamics-review.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [Sci. Robot.集锦](../../../venues/Science-Robotics/README.md)

[原文](https://www.science.org/doi/10.1126/scirobotics.adt1497) · [PDF](https://albertboai.com/assets/pdf/2025_scirobotics.adt1497.pdf) · [阅读卡片](../../../library/learned-dynamics-review.md)

论文出处：[**Bo Ai**](../../origins/papers/learned-dynamics-review.md)<br>[加州大学圣迭戈分校 / 斯坦福大学 · 另4个机构](../../origins/papers/learned-dynamics-review.md)

## 机制简析

以 POMDP/控制目标为入口，按像素、latent、粒子、关键点、物体中心表示比较动力学；再讨论感知和控制接口。

带着这个问题读：世界模型该预测像素、latent、粒子还是物体？换种表示会怎样改写感知与规划的代价？

初读判断：统一比较表达能力、样本效率、泛化和感知代价；不将引用的实验当成本综述自有实验。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 92.7 | 30% |
| 创新性 | 76 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 38.6 | 10% |
| 近期关注 | 37.2 | 5% |
| 复用价值 | 91 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[Sci. Robot. 2025](../../../venues/Science-Robotics/README.md)，正式出处见[出版/原文记录](https://www.science.org/doi/10.1126/scirobotics.adt1497)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文方法与实验选题初读；非全文精读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：A review of learning-based dynamics models for robotic manipulation。累计被引 **21**，2025–2026 被引 **21**；快照：2026-10-10T11:44:51+08:00。

[指标记录](https://api.openalex.org/works/W4414285669) · [文献计量条目](https://openalex.org/W4414285669)

### 影响与关注的计算依据

- **学术影响 38.6**：身份匹配的累计引用C=21，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4414285669)
- **近期关注 37.2**：近期已定位引用R=21；数量与每月引用速度各占一半，有效观察期12.7474个月。 [依据1](https://api.openalex.org/works/W4414285669)
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
