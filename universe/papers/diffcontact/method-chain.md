# 本篇方法链路 · DiffContact

前向继续用硬接触模拟器生成轨迹，只在反向替换接触冲量的敏感度。方法对含de Saxcé修正的库仑摩擦二阶锥互补条件做完整锥中心路径松弛，从硬接触解出发用Newton迭代找到反向求导的评估点，组装状态/动作转移Jacobian，再供BPTT更新策略或DDP/iLQR优化轨迹。法向与切向一起松弛，梯度才有机会指向离地、粘住和滑动这些邻近模式；松弛参数趋零时回到固定接触模式的精确敏感度。

前向继续用硬接触模拟器生成轨迹，只在反向替换接触冲量的敏感度。方法对含de Saxcé修正的库仑摩擦二阶锥互补条件做完整锥中心路径松弛，从硬接触解出发用Newton迭代找到反向求导的评估点，组装状态/动作转移Jacobian，再供BPTT更新策略或DDP/iLQR优化轨迹。法向与切向一起松弛，梯度才有机会指向离地、粘住和滑动这些邻近模式；松弛参数趋零时回到固定接触模式的精确敏感度。

[本篇星系](../diffcontact.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffcontact.md) · [原文依据](https://arxiv.org/abs/2610.35852v1)
