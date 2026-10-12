# OmniH2O 星系

OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning

**导读** · Locomotion 与运动适应

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/omnih2o.md) · [原文](https://proceedings.mlr.press/v270/he25b.html) · [评分卡](../../leaderboard/papers/omnih2o/README.md)

把不同遥操作方式转换成运动学姿态目标，再交给跟踪控制器。特权教师在模拟中学大规模动作，学生用本体历史与稀疏目标通过 DAgger 模仿教师，输出可部署的动作；手部另接姿态到关节控制。原文验证模拟和实机跟踪、不同控制入口及采集示范后的自主技能。

## 技术挂点

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

## 本篇行星与卫星

- [特权训练信息](omnih2o/privileged.md) · 初读挂点
- [教师学生蒸馏](omnih2o/distill.md) · 初读挂点
- [全身控制与执行](omnih2o/wbc.md) · 初读挂点
- [本篇方法链路](omnih2o/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
