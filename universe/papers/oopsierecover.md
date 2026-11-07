# OopsieRecover 星系

OopsieRecover: Learning Transferable VLA Corrections from Semantic Interventions

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/oopsierecover.md) · [原文](https://arxiv.org/abs/2611.08462v1) · [评分卡](../../leaderboard/papers/oopsierecover/README.md)

人接管时提供纠正轨迹、语言和纠正类别。VLM选语义实体种子，分割与深度把区域变成3D点集，质心时间轨迹用于生成gate×(纠正代价+λ任务代价)。触发阈值从同类记录中gate=1的干预前分数取最小；用人类/后续基策略窗口的较低成本及触发检查做经验一致性核验，失败促使程序细化，但预算耗尽仍保留最后程序。部署重新定位实体，从冻结π0.5采样动作块并可加cardinal actions，预测点集后按折扣成本筛最优；仿真用模拟器物理，实机用grasp-based近似。

## 技术挂点

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [点云与三维体素](../concepts/point-cloud.md)：点云用三维点记录几何，网络从点的位置与特征构造空间表示。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [动作条件动力学](../concepts/dynamics.md)：以当前状态和动作预测下一状态或分布，建立“做这个动作会发生什么”的计算接口。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

- [树搜索与轨迹搜索](../concepts/search.md)：展开候选动作或轨迹，用预测价值挑选可执行方案。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [示范模仿](oopsierecover/imitation.md) · 初读挂点
- [空间表示](oopsierecover/spatial.md) · 初读挂点
- [点云与三维体素](oopsierecover/point-cloud.md) · 初读挂点
- [动作表示](oopsierecover/action.md) · 初读挂点
- [动作块](oopsierecover/chunk.md) · 初读挂点
- [动作条件动力学](oopsierecover/dynamics.md) · 初读挂点
- [闭环滚动与历史偏移](oopsierecover/rollout.md) · 初读挂点
- [树搜索与轨迹搜索](oopsierecover/search.md) · 初读挂点
- [泛化评测与遗忘](oopsierecover/benchmark.md) · 初读挂点
- [本篇方法链路](oopsierecover/method-chain.md) · 初读挂点
- [纠正动作与纠正意图不是同一份知识](oopsierecover/oopsierecover-problem.md) · 初读挂点
- [先把谁接管、何时接管记清楚](oopsierecover/oopsierecover-interventions.md) · 初读挂点
- [从语言对象落到三维点集](oopsierecover/oopsierecover-grounding.md) · 初读挂点
- [让模型看实体怎么动，而非整段点云](oopsierecover/oopsierecover-centroids.md) · 初读挂点
- [何时介入与怎样改动作分开](oopsierecover/oopsierecover-cost.md) · 初读挂点
- [用人接管前的状态定阈值](oopsierecover/oopsierecover-calibration.md) · 初读挂点
- [回放检查只检查已有纠正方向](oopsierecover/oopsierecover-verification.md) · 初读挂点
- [修到预算上限也可能留下未通过程序](oopsierecover/oopsierecover-budget.md) · 初读挂点
- [换场景先重新找同一类实体](oopsierecover/oopsierecover-transfer.md) · 初读挂点
- [冻结策略提候选，纠正规则做筛选](oopsierecover/oopsierecover-steering.md) · 初读挂点
- [仿真预测器和实机预测器要分开看](oopsierecover/oopsierecover-dynamics.md) · 初读挂点
- [同纠正数据比较能否换摆放位置](oopsierecover/oopsierecover-sim.md) · 初读挂点
- [实机提高的是完成阶段比例](oopsierecover/oopsierecover-real.md) · 初读挂点
- [纠正数量曲线仍待统一数值](oopsierecover/oopsierecover-scaling.md) · 初读挂点
- [单故障跨场景测试限定了什么](oopsierecover/oopsierecover-detection.md) · 初读挂点
- [感知、预测和候选动作都能卡住恢复](oopsierecover/oopsierecover-limits.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
