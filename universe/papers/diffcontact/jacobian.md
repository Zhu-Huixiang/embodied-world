# 冲量敏感度与转移Jacobian · DiffContact

将接触冲量对状态/动作的变化组装为动力学导数。

配合Pinocchio刚体解析导数形成f_x和f_u，分别供BPTT和DDP/iLQR反传。

继续拆：[20步短段策略反传](bptt.md) · [接触隐式轨迹优化](cito.md)。

[本篇星系](../diffcontact.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffcontact.md) · [原文依据](https://arxiv.org/html/2610.35852v1)
