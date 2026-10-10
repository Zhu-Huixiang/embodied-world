# ANYmal parkour: Learning agile navigation for quadrupedal robots

**ANYmal Parkour** · Sci. Robot. 2024 · 本版排名 33 · 综合分 **89.0 / 100**

[解读导读](../../../library/anymal-parkour.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [Sci. Robot.集锦](../../../venues/Science-Robotics/README.md)

[原文](https://www.science.org/doi/10.1126/scirobotics.adi7566) · [PDF](https://arxiv.org/pdf/2306.14874) · [阅读卡片](../../../library/anymal-parkour.md)

## 机制简析

先训练跳、爬、蹲和行走等低层策略，高层导航策略依据感知重建的环境选择技能和目标。感知模块从遮挡、噪声输入重建障碍，使高层决策了解各技能可完成的动作范围。原文在连续障碍的实机导航中验证模拟训练链路。

带着这个问题读：会跳、会爬的低层技能，怎样被高层导航策略排成一条可走路线？

初读判断：正式 Science Robotics，具备层次模块、噪声感知、连续实机障碍和对照，科学问题与读图素材都适合精讲。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 92.7 | 30% |
| 创新性 | 90 | 20% |
| 实验与证据 | 94 | 20% |
| 学术影响 | 69.5 | 10% |
| 近期关注 | 86.0 | 5% |
| 复用价值 | 82 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[Sci. Robot. 2024](../../../venues/Science-Robotics/README.md)，正式出处见[出版/原文记录](https://www.science.org/doi/10.1126/scirobotics.adi7566)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：ANYmal parkour: Learning agile navigation for quadrupedal robots。累计被引 261，2025–2026 被引 209；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4392763392) · [文献计量条目](https://openalex.org/W4392763392)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
