# cuRoboV2-Fast: Fast Torque-Limited Collision-Free Motion Planning

**解读导读** · arXiv 2026 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：Panda离线规划、Panda/G1计算内核、YAM模拟与实机抓放；实机时间基于已完成周期。

[原文入口](https://arxiv.org/abs/2611.06913v1) · [原文 PDF](https://arxiv.org/pdf/2611.06913v1) · [作者项目 / 代码入口](https://research.nvidia.com/labs/lpr/curobov2-fast/) · [作者与团队](../leaderboard/origins/papers/curobov2-fast.md)

## 先看它做了什么

用三次B样条降低轨迹优化变量耦合；直线种子不足时GPU双向RRT补路线。随后TimeOpt固定几何、以路径速度平方样条非均匀分配时间，局部支持产生带状Newton系统，预测校正复用Cholesky。运动学、碰撞与RNEA直接梯度共同减少每次迭代成本，负载惯量可运行时更新。

## 带着什么问题读

**当规划只占抓取周期的1%，怎样同时缩短求解时间与受力矩限制的真实运动？**

## 为什么值得继续读

分离少迭代、低迭代成本和固定路径时间优化三种收益，有匹配种子收敛消融、负载基准与实机耗时链路；是可追溯独立研究，非仅软件版号。

证据入口：Fig12在3kg/RTX5090下4.43ms对cuRoboV2 65.13ms，Fast每负载2590查询重复两次；运动质量以1599全共有有效查询比较。Fig11的93共有有效查询，TimeOpt相对均匀精修后再缩短运动15.7%。YAM/RTX6000Ada完成周期5.93对9.07秒，约50对15次完成周期；不是总抓取成功率。

具身关联：直接连接碰撞自由几何、负载动力学、GPU优化与真实机械臂执行；速度与成功率及约束口径可分开学。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/curobov2-fast.md) · [七维评分与雷达](../leaderboard/papers/curobov2-fast/README.md) · [arXiv集锦](../arxiv/README.md#paper-curobov2-fast) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-11-06。
