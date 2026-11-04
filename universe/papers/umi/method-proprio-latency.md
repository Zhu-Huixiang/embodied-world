# 本体延迟区分精确时间与近似测法 · UMI

有发送时间的Franka使用接收减发送；缺硬件时间的UR5和夹爪用一半ping往返时间近似。

不同设备的测法精度不同，不能把近似单向时延说成每帧精确测量。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#42-pd12动作算出来还得来得及执行)

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://umi-gripper.github.io/umi.pdf)
