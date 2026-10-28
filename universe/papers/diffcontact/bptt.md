# 20步短段策略反传 · DiffContact

沿20个控制步把代价梯度传回策略参数。

H=20覆盖0.5s，无末端critic；37维状态含nq=19、nv=18，12维关节力矩，策略以PD关节目标接入。

继续拆：[同前向三种梯度对照](ablate.md) · [短时训练后上四足实机](hardware.md) · [PPO样本和时间对照](method-ppo.md)。

[本篇星系](../diffcontact.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffcontact.md) · [原文依据](https://arxiv.org/html/2610.35852v1)
