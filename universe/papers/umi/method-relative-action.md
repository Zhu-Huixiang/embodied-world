# 整段未来轨迹共享当前参考帧 · UMI

同一次预测内每个未来SE(3)目标都相对当前末端，而不是相对上一步。

当前参考位姿的逆乘未来目标得到相对变换；执行时再左乘本轮固定参考位姿恢复机器人目标。4×4是齐次变换形状，不是网络动作维数。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#43-pd21相对目标为什么不等于逐步增量)

继续拆：[本体历史也使用相对位姿](method-relative-history.md)。

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://www.roboticsproceedings.org/rss20/p045.pdf)
