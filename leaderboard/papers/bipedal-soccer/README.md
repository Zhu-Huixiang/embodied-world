# Learning agile soccer skills for a bipedal robot with deep reinforcement learning

本版阅读优先顺序：35；综合分：88.3 / 100；已评分权重：100%。

[原文](https://www.science.org/doi/10.1126/scirobotics.adi8022) · [PDF](https://arxiv.org/pdf/2304.13653) · [阅读卡片](../../../library/bipedal-soccer.md)

## 机制简析

先学习起身和足球等技能，再训练能在比赛状态下组合动作的策略；底层动作为二十维关节位置目标。MPO 更新策略和值函数，系统辨识、针对性的动力学随机化和扰动帮助模拟策略迁移到真实机器人。论文用一对一足球与脚本控制器对比行走、转向、起身和踢球表现。

带着这个问题读：踢球、摔倒再爬起和防守，怎样被训练成会连续切换的全身行为？

初读判断：正式 Science Robotics，真实硬件与脚本基线、多技能指标和训练设计实验，比单段炫技视频有更完整证据。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 92.7 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 64.3 | 10% |
| 近期关注 | 78.7 | 5% |
| 复用价值 | 83 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[Sci. Robot. 2024](../../../venues/Science-Robotics/README.md)，正式出处见[出版/原文记录](https://www.science.org/doi/10.1126/scirobotics.adi8022)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Learning agile soccer skills for a bipedal robot with deep reinforcement learning。累计被引 171，2025–2026 被引 132；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4394674699) · [文献计量条目](https://openalex.org/W4394674699)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
