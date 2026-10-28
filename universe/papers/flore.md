# FLoRe 星系

Learning Force-Reactive Humanoid Loco-Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/flore.md) · [原文](https://arxiv.org/abs/2610.35862v1) · [评分卡](../../leaderboard/papers/flore/README.md)

双手持夹爪记录腕部图像、六轴接触力/力矩和身体运动，先做无机器人示范，再补成机器人可跟踪的全身参考。每任务一套扩散策略读取两张224×224腕图、14维相对状态和双手wrench历史，同时生成运动关键点与每手力指令；高层动作块交给低层全身控制器。低层将力误差积分换成手部位置目标偏移：命令方向持续调力，其余方向保持顺应，真实腕部传感器闭合反馈环。力不是只在训练时当标签，而是从示范、策略输入/输出一路接到执行。

## 技术挂点

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

- [仿真到实机](../concepts/sim2real.md)：处理仿真动力学、感知和真实系统间的差异，通过随机化、辨识、残差或适配来迁移。

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

## 本篇行星与卫星

- [示范模仿](flore/imitation.md) · 初读挂点
- [扩散去噪](flore/diffusion.md) · 初读挂点
- [动作块](flore/chunk.md) · 初读挂点
- [全身控制与执行](flore/wbc.md) · 初读挂点
- [仿真到实机](flore/sim2real.md) · 初读挂点
- [运动重定向](flore/retarget.md) · 初读挂点
- [动作表示](flore/action.md) · 初读挂点
- [机器人数据与评测](flore/data.md) · 初读挂点
- [本篇方法链路](flore/method-chain.md) · 初读挂点
- [带力示范采集](flore/demo.md) · 初读挂点
- [示范补全与运动参考](flore/method-retarget.md) · 初读挂点
- [图像、14维状态与wrench历史](flore/observation.md) · 初读挂点
- [运动与力的联合扩散输出](flore/method-diffusion.md) · 初读挂点
- [力误差积分到位置偏移](flore/integral.md) · 初读挂点
- [命令方向跟力与其他方向顺应](flore/compliance.md) · 初读挂点
- [跟力精度与运动误差的取舍](flore/sim.md) · 初读挂点
- [三类G1接触任务](flore/hardware.md) · 初读挂点
- [力命令与力观测的分路消融](flore/ablation.md) · 初读挂点
- [实机跟力响应时间](flore/response.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
