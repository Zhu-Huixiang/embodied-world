# 删除已错过执行时刻的动作前缀 · UMI

动作预测从最后图像拍摄时刻开始，观测、推理与执行延迟会消耗一段时间。

按硬件检查目标时间，只执行尚未过期部分；不是让机器人补跑所有过去时刻的命令。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#42-pd12动作算出来还得来得及执行)

继续拆：[臂与夹爪提前不同时间发令](method-command-ahead.md)。

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://www.roboticsproceedings.org/rss20/p045.pdf)
