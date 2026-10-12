# Mobile ALOHA 星系

Mobile ALOHA: Learning Bimanual Mobile Manipulation using Low-Cost Whole-Body Teleoperation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/mobile-aloha.md) · [原文](https://proceedings.mlr.press/v270/fu25b.html) · [评分卡](../../leaderboard/papers/mobile-aloha/README.md)

把双臂关节位置与底盘线/角速度拼成统一动作，遥操作同时记录手臂与底盘；行为克隆直接预测整套动作。训练混入已有静态 ALOHA 示范，检验不同任务、臂安装位置和场景之间的正迁移。原文把自治策略执行与人类遥操作采集分开，比较联合训练和只用移动数据的任务表现。

## 技术挂点

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

## 本篇行星与卫星

- [行为克隆](mobile-aloha/bc.md) · 初读挂点
- [动作块](mobile-aloha/chunk.md) · 初读挂点
- [全身控制与执行](mobile-aloha/wbc.md) · 初读挂点
- [本篇方法链路](mobile-aloha/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
