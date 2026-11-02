# TouchBridge 星系

TouchBridge: Tactile-Conditioned Human-to-Robot Transfer for Dexterous Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/touchbridge.md) · [原文](https://arxiv.org/abs/2610.40349v1) · [评分卡](../../leaderboard/papers/touchbridge/README.md)

TouchBridge让人类手套和Wuji灵巧手共享指尖触觉布局及腕相机视角。Tac-Retarget联合优化两手基座SE(3)与关节，匹配指尖位姿、触觉加权接触中心及活跃taxel支撑，并沿用TopoRetarget的距离加权Laplacian思想建立触觉激活的双手接触图。接触时减弱位姿跟踪，并用响应相关几何位移补偿顺应性。SAM2/ProPainter移除人手、渲染机器人外观，固定场景AprilTag消除头部相机运动后转换动作，用转换后的视觉/状态动作微调GR00T N1.7。触觉只服务离线重定向，不输入运行策略。

## 技术挂点

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [运动重定向](touchbridge/retarget.md) · 初读挂点
- [跨本体数据](touchbridge/cross-body.md) · 初读挂点
- [示范模仿](touchbridge/imitation.md) · 初读挂点
- [行为克隆](touchbridge/bc.md) · 初读挂点
- [动作表示](touchbridge/action.md) · 初读挂点
- [动作块](touchbridge/chunk.md) · 初读挂点
- [空间表示](touchbridge/spatial.md) · 初读挂点
- [表征空间](touchbridge/representation.md) · 初读挂点
- [机器人数据与评测](touchbridge/data.md) · 初读挂点
- [泛化评测与遗忘](touchbridge/benchmark.md) · 初读挂点
- [本篇方法链路](touchbridge/method-chain.md) · 初读挂点
- [位姿对应为什么保不住接触](touchbridge/tb-problem.md) · 初读挂点
- [人机视觉与指尖触觉共设计](touchbridge/tb-hardware.md) · 初读挂点
- [AprilTag与指尖坐标标定](touchbridge/tb-calibration.md) · 初读挂点
- [双手基座与关节联合优化](touchbridge/tb-objective.md) · 初读挂点
- [接触中心与活跃taxel支撑](touchbridge/tb-contact.md) · 初读挂点
- [触觉激活的双手接触图](touchbridge/tb-contact-graph.md) · 初读挂点
- [接触后放松位姿约束](touchbridge/tb-weighting.md) · 初读挂点
- [响应相关的几何顺应补偿](touchbridge/tb-compliance.md) · 初读挂点
- [移除人手再渲染机器人外观](touchbridge/tb-visual.md) · 初读挂点
- [固定场景坐标中的动作转换](touchbridge/tb-action-anchor.md) · 初读挂点
- [触觉用于离线转换而非策略输入](touchbridge/tb-policy.md) · 初读挂点
- [四任务等量遥操与人类数据对照](touchbridge/tb-real-eval.md) · 初读挂点
- [匹配初始场景下的轨迹回放](touchbridge/tb-replay.md) · 初读挂点
- [采集效率与总体成本分开](touchbridge/tb-collection.md) · 初读挂点
- [用仿真接触误差诊断重定向](touchbridge/tb-sim-contact.md) · 初读挂点
- [去接触项与去接触图的闭环消融](touchbridge/tb-ablation.md) · 初读挂点
- [预训练动作先验的作用](touchbridge/tb-pretrain.md) · 初读挂点
- [单平台规模与工程复用边界](touchbridge/tb-limits.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
