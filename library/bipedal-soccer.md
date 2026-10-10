# Learning agile soccer skills for a bipedal robot with deep reinforcement learning

**解读导读** · Sci. Robot. 2024 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：双足全身 RL 与实机行为组合。

[原文入口](https://www.science.org/doi/10.1126/scirobotics.adi8022) · [原文 PDF](https://arxiv.org/pdf/2304.13653) · [作者项目 / 代码入口](https://deepmind.google/research/publications/31284/)

Science Robotics 2024；评测对象是低成本小型双足机器人和简化一对一足球。

## 先看它做了什么

先学习起身和足球等技能，再训练能在比赛状态下组合动作的策略；底层动作为二十维关节位置目标。MPO 更新策略和值函数，系统辨识、针对性的动力学随机化和扰动帮助模拟策略迁移到真实机器人。论文用一对一足球与脚本控制器对比行走、转向、起身和踢球表现。

## 带着什么问题读

**踢球、摔倒再爬起和防守，怎样被训练成会连续切换的全身行为？**

## 为什么值得继续读

顶刊实机双足敏捷行为与战术组合，任务和视频容易吸引兴趣；同时能具体解释奖励、频率、随机化与行为组合。

证据入口：正式 Science Robotics，真实硬件与脚本基线、多技能指标和训练设计实验，比单段炫技视频有更完整证据。

具身关联：顶刊实机双足敏捷行为与战术组合，任务和视频容易吸引兴趣；同时能具体解释奖励、频率、随机化与行为组合。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/bipedal-soccer/README.md) · [Sci. Robot.集锦](../venues/Science-Robotics/README.md) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-10。
