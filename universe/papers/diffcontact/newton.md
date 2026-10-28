# 从硬接触解求反向评估点 · DiffContact

Newton迭代先解松弛关系，再在该点求敏感度。

从硬接触解初始化，正则化与偏移改善收敛；每接触点3维，多个接触联合求解。

继续拆：[冲量敏感度与转移Jacobian](jacobian.md) · [Newton残差与锥可行性](feasible.md)。

[本篇星系](../diffcontact.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffcontact.md) · [原文依据](https://arxiv.org/html/2610.35852v1)
