# Differentiable Contact Dynamics for Legged Locomotion: Policy Learning and Contact-Implicit Trajectory Optimization

**解读导读** · arXiv 2026 · [Locomotion 与运动适应](../paper-map/README.md#track-locomotion)

研究范围：解析接触梯度、BPTT足式策略学习与接触隐式轨迹优化；45kg四足点足接触模型及实机策略。

[原文入口](https://arxiv.org/abs/2610.35852v1) · [原文 PDF](https://arxiv.org/pdf/2610.35852v1) · [作者项目 / 代码入口](https://diffcontact.github.io) · [作者与团队](../leaderboard/origins/papers/diffcontact.md)

## 先看它做了什么

前向继续用硬接触模拟器生成轨迹，只在反向替换接触冲量的敏感度。方法对含de Saxcé修正的库仑摩擦二阶锥互补条件做完整锥中心路径松弛，从硬接触解出发用Newton迭代找到反向求导的评估点，组装状态/动作转移Jacobian，再供BPTT更新策略或DDP/iLQR优化轨迹。法向与切向一起松弛，梯度才有机会指向离地、粘住和滑动这些邻近模式；松弛参数趋零时回到固定接触模式的精确敏感度。

## 带着什么问题读

**脚从粘地到滑动，精确梯度为何可能指不出路？保留硬接触前向、只松弛反向梯度，能换来什么又付出什么？**

## 为什么值得继续读

在同一硬接触前向与任务目标下，直接比较精确、仅法向松弛和完整摩擦锥三种反向梯度；机制推导、数值可行性、学习对照和实机部署互相照应。

证据入口：Fig.7：单仿真环境BPTT，trot/pace各100,000控制步、108s训练后无微调上45kg四足；gait-free另为160,000步、172s。Fig.9–10最小能学trot配置：BPTT1环境约1e5样本/1.8min，PPO128环境约1e7/17.7min；两者学习估计器不同。Fig.11检查Newton收敛和摩擦锥可行性；CITO的base-pose与拉扰恢复比较属于仿真。

具身关联：给接触丰富的足式学习和轨迹优化提供可解析反传的控制接口，重点解决接触模式边界附近的训练信号。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/diffcontact.md) · [七维评分与雷达](../leaderboard/papers/diffcontact/README.md) · [arXiv集锦](../arxiv/README.md#paper-diffcontact) · [地图方向](../paper-map/README.md#track-locomotion) · [首页](../README.md)

元数据核对：2026-10-28。
