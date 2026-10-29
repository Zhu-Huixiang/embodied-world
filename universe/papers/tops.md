# TOPS 星系

TOPS: Reshaping Flow Source and Transport for Multi-Task Robot Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tops.md) · [原文](https://arxiv.org/abs/2610.36694v1) · [评分卡](../../leaderboard/papers/tops/README.md)

先用标准flow matching暖启动，把专家动作块沿逆流拉回噪声空间，按训练任务建立bank，再以低秩协方差高斯混合MPPCA拟合任务源。根据源/动作协方差的高斯最优输运方向识别需要扩张的轴，只在这些方向采用先慢后快插值，其他方向保留线性。固定源和schedule继续训练同一速度网络；语言selector选已知任务源。推理的一步采用依序两次网络求值的schedule-aware两半步方法，即NFE=2，不是一次前向。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

- [分布偏移](../concepts/shift.md)：测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。

## 本篇行星与卫星

- [Flow Matching](tops/flow.md) · 初读挂点
- [动作表示](tops/action.md) · 初读挂点
- [动作块](tops/chunk.md) · 初读挂点
- [示范模仿](tops/imitation.md) · 初读挂点
- [泛化评测与遗忘](tops/benchmark.md) · 初读挂点
- [分布偏移](tops/shift.md) · 初读挂点
- [本篇方法链路](tops/method-chain.md) · 初读挂点
- [标准FM暖启动](tops/warmup.md) · 初读挂点
- [专家动作逆映射的任务bank](tops/reverse-bank.md) · 初读挂点
- [低秩高斯混合源](tops/mppca.md) · 初读挂点
- [语言选择已知任务源](tops/selector.md) · 初读挂点
- [协方差与扩张方向](tops/covariance.md) · 初读挂点
- [扩张轴先慢后快插值](tops/schedule.md) · 初读挂点
- [一次积分步与两次网络求值](tops/solver.md) · 初读挂点
- [同训练run与推理预算比较](tops/benchmark-budget.md) · 初读挂点
- [扰动与跨环境评估](tops/ood-protocol.md) · 初读挂点
- [π0.5迁移](tops/transfer.md) · 初读挂点
- [固定身体的八类单臂任务](tops/hardware.md) · 初读挂点
- [源、路径和求解器的联合消融](tops/component-ablation.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
