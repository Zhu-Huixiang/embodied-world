# 动态任务保原速，准静态任务放慢 · UMI

抛掷采用20Hz并按演示原速执行，其余任务为10Hz并以0.5倍演示速度执行。

调的是期望目标的时间间隔，环境采样频率与网络实际推理调用频率也要分开。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://umi-gripper.github.io/umi.pdf)
