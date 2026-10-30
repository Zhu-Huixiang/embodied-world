# Gaussian Distillation of Flow Policies

**解读导读** · arXiv 2026 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：预训练flow动作策略的高斯读出蒸馏；RoboCasa365与LIBERO-Long仿真。

[原文入口](https://arxiv.org/abs/2610.40271v1) · [原文 PDF](https://arxiv.org/pdf/2610.40271v1) · [作者与团队](../leaderboard/origins/papers/gar.md)

## 先看它做了什么

GAR冻结原策略的视觉语言骨干和动作Transformer，把固定噪声在t=0的一次前向特征接给小读出：仿射修正预测连续动作均值，池化后128单元MLP预测方差或Cholesky因子，另一仿射头预测离散命令的伯努利概率。训练目标来自已部署教师反复采样的经验矩与命令频率，均值用最小二乘，协方差用按坐标归一的误差及对数方差项，离散命令用交叉熵。推理直接采样高斯连续动作和独立伯努利命令，不再积分速度场；可写闭式动作似然。论文先检验固定观测下教师平移/旋转分布的高斯近似，再检查控制表现和近似的代价。

## 带着什么问题读

**动作流真的需要反复积分才能做得好，还是冻结内部特征后，用一个高斯读出就能保留大部分控制能力？**

## 为什么值得继续读

直接检验生成动作分布的复杂度与控制收益是否相称，并以同一教师的原多步、原单步、只预测均值、高斯对角/全协方差等对照拆开机制；提供两教师、两仿真基准、误差诊断、成本拆分和不确定度。

证据入口：Table 2：RoboCasa365 50任务、每任务每策略50次，Xiaomi-Robotics-1由58.24%到对角GAR57.64%，GR00T N1.5由23.08%到21.92%；原始单步为55.76%/19.28%。Table 11：RTX4090上全策略延迟220.25→115.36ms（1.91倍）、68.01→43.30ms（1.57倍）。LIBERO-Long Xiaomi-Robotics-0为483/500→477/500。RoboCasa各读出一份拟合checkpoint；Table 13的成功差95%区间为[-2.84,1.60]/[-3.04,0.68]个百分点，描述该checkpoint/任务集内episode不确定度，不构成等效性检验。全部机器人控制实验为仿真。

具身关联：服务机器人动作块低延迟生成与可计算似然，帮助判断VLA/flow策略哪些随机性和网络计算真正影响闭环任务。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/gar.md) · [七维评分与雷达](../leaderboard/papers/gar/README.md) · [arXiv集锦](../arxiv/README.md#paper-gar) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-30。
