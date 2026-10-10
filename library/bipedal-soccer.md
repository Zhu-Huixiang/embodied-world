# Learning agile soccer skills for a bipedal robot with deep reinforcement learning

出处：Science-Robotics 2024。研究范围：双足全身 RL 与实机行为组合。

[原文入口](https://www.science.org/doi/10.1126/scirobotics.adi8022) · [原文 PDF](https://arxiv.org/pdf/2304.13653) · [作者项目 / 代码入口](https://deepmind.google/research/publications/31284/)

Science Robotics 2024；评测对象是低成本小型双足机器人和简化一对一足球。

阅读问题：**踢球、摔倒再爬起和防守，怎样被训练成会连续切换的全身行为？**

收录理由：顶刊实机双足敏捷行为与战术组合，任务和视频容易吸引兴趣；同时能具体解释奖励、频率、随机化与行为组合。

证据入口：正式 Science Robotics，真实硬件与脚本基线、多技能指标和训练设计实验，比单段炫技视频有更完整证据。

具身关联：顶刊实机双足敏捷行为与战术组合，任务和视频容易吸引兴趣；同时能具体解释奖励、频率、随机化与行为组合。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/bipedal-soccer/README.md)

机制简析：先学习起身和足球等技能，再训练能在比赛状态下组合动作的策略；底层动作为二十维关节位置目标。MPO 更新策略和值函数，系统辨识、针对性的动力学随机化和扰动帮助模拟策略迁移到真实机器人。论文用一对一足球与脚本控制器对比行走、转向、起身和踢球表现。
<!-- discovery:end -->
