# cuRoboV2-Fast 星系

cuRoboV2-Fast: Fast Torque-Limited Collision-Free Motion Planning

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文](https://arxiv.org/abs/2611.06913v1) · [评分卡](../../leaderboard/papers/curobov2-fast/README.md)

用三次B样条降低轨迹优化变量耦合；直线种子不足时GPU双向RRT补路线。随后TimeOpt固定几何、以路径速度平方样条非均匀分配时间，局部支持产生带状Newton系统，预测校正复用Cholesky。运动学、碰撞与RNEA直接梯度共同减少每次迭代成本，负载惯量可运行时更新。

## 技术挂点

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

## 本篇行星与卫星

- [动作表示](curobov2-fast/action.md) · 初读挂点
- [空间表示](curobov2-fast/spatial.md) · 初读挂点
- [本篇方法链路](curobov2-fast/method-chain.md) · 初读挂点
- [路径短不等于执行快](curobov2-fast/fast-problem.md) · 初读挂点
- [与早期cuRobo分开核身份](curobov2-fast/fast-lineage.md) · 初读挂点
- [先直线、必要时RRT再精修](curobov2-fast/fast-pipeline.md) · 初读挂点
- [有界双向并行RRT](curobov2-fast/fast-rrt.md) · 初读挂点
- [粗路线不等于可执行轨迹](curobov2-fast/fast-route-validation.md) · 初读挂点
- [三次B样条位置控制点](curobov2-fast/fast-position-spline.md) · 初读挂点
- [按控制点收集梯度](curobov2-fast/fast-gradient-gather.md) · 初读挂点
- [固定路径上的非均匀时间分配](curobov2-fast/fast-timeopt.md) · 初读挂点
- [速度加速度jerk与力矩约束](curobov2-fast/fast-sampled-constraints.md) · 初读挂点
- [固定路径力矩仿射化](curobov2-fast/fast-affine-torque.md) · 初读挂点
- [局部支持带来的带状Newton系统](curobov2-fast/fast-banded.md) · 初读挂点
- [共享连杆wrench与Jacobian列](curobov2-fast/fast-kinematics.md) · 初读挂点
- [包围盒剪枝与半段距离复用](curobov2-fast/fast-collision.md) · 初读挂点
- [RNEA物理逆动力学](curobov2-fast/fast-rnea.md) · 初读挂点
- [运行时更新负载惯量](curobov2-fast/fast-payload.md) · 初读挂点
- [抓取与转移分两次规划](curobov2-fast/fast-grasp.md) · 初读挂点
- [同IK种子的收敛消融](curobov2-fast/fast-convergence.md) · 初读挂点
- [TimeOpt额外收益](curobov2-fast/fast-timing-ablation.md) · 初读挂点
- [三档负载全链规划评测](curobov2-fast/fast-payload-benchmark.md) · 初读挂点
- [Jetson时间口径](curobov2-fast/fast-embedded.md) · 初读挂点
- [模块时延不等于完整规划](curobov2-fast/fast-kernel-benchmark.md) · 初读挂点
- [五物体模拟抓放](curobov2-fast/fast-simulation.md) · 初读挂点
- [YAM实机感知与抓取集成](curobov2-fast/fast-real-system.md) · 初读挂点
- [已完成周期时间与成功率分开](curobov2-fast/fast-completed-cycle.md) · 初读挂点
- [规划约束与执行反馈差别](curobov2-fast/fast-execution-limits.md) · 初读挂点
- [接触成功成为剩余瓶颈](curobov2-fast/fast-limit.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
