# PHC 星系

Perpetual Humanoid Control for Real-time Simulated Avatars

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/phc.md) · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html) · [评分卡](../../leaderboard/papers/phc/README.md)

目标条件的物理控制器接收参考姿态或关键点，输出仿真动作以保持平衡并跟踪。渐进乘性策略按难动作扩展容量，保留已有跟踪技能，再加入失败状态恢复，避免新增任务覆盖旧技能。实验对比大规模动作跟踪、噪声姿态与跌倒恢复。

## 技术挂点

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

- [分层技能与计划](../concepts/skills.md)：高层选择目标或技能，低层负责具体执行，层次之间有明确接口。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

## 本篇行星与卫星

- [动作先验](phc/motion-prior.md) · 初读挂点
- [分层技能与计划](phc/skills.md) · 初读挂点
- [全身控制与执行](phc/wbc.md) · 初读挂点
- [本篇方法链路](phc/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
