# ANYmal parkour: Learning agile navigation for quadrupedal robots

**解读导读** · Sci. Robot. 2024 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：层次四足控制、感知与导航。

[原文入口](https://www.science.org/doi/10.1126/scirobotics.adi7566) · [原文 PDF](https://arxiv.org/pdf/2306.14874) · [作者项目 / 代码入口](https://sites.google.com/leggedrobotics.com/agile-navigation) · [作者与团队](../leaderboard/origins/papers/anymal-parkour.md)

Science Robotics 2024；arXiv 初稿为 2023。

## 先看它做了什么

先训练跳、爬、蹲和行走等低层策略，高层导航策略依据感知重建的环境选择技能和目标。感知模块从遮挡、噪声输入重建障碍，使高层决策了解各技能可完成的动作范围。原文在连续障碍的实机导航中验证模拟训练链路。

## 带着什么问题读

**会跳、会爬的低层技能，怎样被高层导航策略排成一条可走路线？**

## 为什么值得继续读

顶刊将感知、技能与导航串成真实机器人闭环，适合与单策略 Extreme Parkour 比较层次设计的取舍。

证据入口：正式 Science Robotics，具备层次模块、噪声感知、连续实机障碍和对照，科学问题与读图素材都适合精讲。

具身关联：顶刊将感知、技能与导航串成真实机器人闭环，适合与单策略 Extreme Parkour 比较层次设计的取舍。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/anymal-parkour/README.md) · [Sci. Robot.集锦](../venues/Science-Robotics/README.md) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-10。
