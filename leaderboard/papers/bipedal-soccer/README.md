# Learning agile soccer skills for a bipedal robot with deep reinforcement learning

**Bipedal Soccer** · Sci. Robot. 2024 · 本版排名 37 · 综合分 **87.6 / 100**

[解读导读](../../../library/bipedal-soccer.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [Sci. Robot.集锦](../../../venues/Science-Robotics/README.md)

[原文](https://www.science.org/doi/10.1126/scirobotics.adi8022) · [PDF](https://arxiv.org/pdf/2304.13653) · [阅读卡片](../../../library/bipedal-soccer.md)

论文出处：[Tuomas Haarnoja / Ben Moran 等4位 · Google DeepMind / University College London](../../origins/papers/bipedal-soccer.md)

## 机制简析

先学习起身和足球等技能，再训练能在比赛状态下组合动作的策略；底层动作为二十维关节位置目标。MPO 更新策略和值函数，系统辨识、针对性的动力学随机化和扰动帮助模拟策略迁移到真实机器人。论文用一对一足球与脚本控制器对比行走、转向、起身和踢球表现。

带着这个问题读：踢球、摔倒再爬起和防守，怎样被训练成会连续切换的全身行为？

初读判断：正式 Science Robotics，真实硬件与脚本基线、多技能指标和训练设计实验，比单段炫技视频有更完整证据。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 92.7 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 64.3 | 10% |
| 近期关注 | 64.5 | 5% |
| 复用价值 | 83 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[Sci. Robot. 2024](../../../venues/Science-Robotics/README.md)，正式出处见[出版/原文记录](https://www.science.org/doi/10.1126/scirobotics.adi8022)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Learning agile soccer skills for a bipedal robot with deep reinforcement learning。累计被引 **171**，2025–2026 被引 **132**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4394674699) · [文献计量条目](https://openalex.org/W4394674699)

### 影响与关注的计算依据

- **学术影响 64.3**：身份匹配的累计引用C=171，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4394674699)
- **近期关注 64.5**：近期已定位引用R=132；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4394674699)
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
