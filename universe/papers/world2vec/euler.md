# 潜向量场与Euler残差 · world2vec

预测潜状态变化率，再乘时间间隔更新状态。

动作在区间内恒定，z_next=z+Δt f(z,a)。相对直接MLP输出下一状态，这是残差式潜动力学接口，不是新发明ODE积分。

继续拆：[沿自身预测轨迹训练多步](multistep-rollout.md) · [目标编码与CEM规划](latent-mpc.md) · [改变积分步长与控制频率](retiming.md)。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/pdf/2610.40637v1)
