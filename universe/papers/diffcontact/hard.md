# 保留硬接触前向 · DiffContact

模拟器仍按硬接触求解并推进实际训练轨迹。

RaiSim以1ms子步前向推进，控制步25ms；松弛用于反向评估，不能说硬接触物理本身已被变光滑。

继续拆：[点足与接触几何的边界](geometry.md)。

[本篇星系](../diffcontact.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/diffcontact.md) · [原文依据](https://arxiv.org/html/2610.35852v1)
