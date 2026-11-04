# 用条件去噪学习示范动作序列 · UMI

UMI使用Diffusion Policy把同步图像与本体历史映射为未来末端和连续夹爪轨迹分布。

动作先按噪声等级混合，再由观察条件与带噪动作预测噪声；部署时从噪声逐轮恢复动作块。该损失是标准Diffusion Policy教学展开。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

继续拆：[视图数量与历史长度分别计数](method-observation-shapes.md) · [动作horizon与去噪步数不同](method-horizons.md) · [不同任务采用不同视觉编码器](method-backbones.md) · [动态任务保原速，准静态任务放慢](method-frequency-speed.md) · [训练视觉扰动覆盖颜色与小位姿变化](method-augmentation.md)。

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://umi-gripper.github.io/umi.pdf)
