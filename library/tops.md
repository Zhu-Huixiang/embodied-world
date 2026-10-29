# TOPS: Reshaping Flow Source and Transport for Multi-Task Robot Manipulation

**解读导读** · arXiv 2026 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：按已知任务重塑flow源分布与输运时序；LIBERO/CALVIN与固定身体单臂实机。

[原文入口](https://arxiv.org/abs/2610.36694v1) · [原文 PDF](https://arxiv.org/pdf/2610.36694v1) · [作者项目 / 代码入口](https://ntumars.github.io/TOPS/) · [作者与团队](../leaderboard/origins/papers/tops.md)

## 先看它做了什么

先用标准flow matching暖启动，把专家动作块沿逆流拉回噪声空间，按训练任务建立bank，再以低秩协方差高斯混合MPPCA拟合任务源。根据源/动作协方差的高斯最优输运方向识别需要扩张的轴，只在这些方向采用先慢后快插值，其他方向保留线性。固定源和schedule继续训练同一速度网络；语言selector选已知任务源。推理的一步采用依序两次网络求值的schedule-aware两半步方法，即NFE=2，不是一次前向。

## 带着什么问题读

**多任务动作流为什么都要从同一个高斯出发、沿同一条直线走？换出发点和速度安排，能否少算几次网络？**

## 为什么值得继续读

直接重设计生成策略的源分布、训练路径和数值求解，提供逐模块消融、匹配NFE、π0.5迁移及实机多任务比较。

证据入口：Table 1主实验三训练run：LIBERO-10从标准FM的53.44±2.93到TOPS69.67±0.61；每policy call延迟49.4→8.2ms（RTX PRO 6000），对应NFE20→2。LIBEROPlus27.11→35.29，口径为排除全0 Camera类的2100变体。π0.5相同14K训练预算下LIBEROPlus64.4→69.0、CALVIN ABC→D 3.033→3.744，为单checkpoint。实机八任务各20次，TOPS124/160=77.50%，FM82/160=51.25%，仅用Galaxea R1 Lite右臂和夹爪，其他身体固定。

具身关联：服务低延迟多任务操作策略，研究动作生成路径对成功率和网络求值预算的影响。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/tops.md) · [七维评分与雷达](../leaderboard/papers/tops/README.md) · [arXiv集锦](../arxiv/README.md#paper-tops) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-29。
