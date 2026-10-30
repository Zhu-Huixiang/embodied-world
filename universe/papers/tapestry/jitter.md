# 多步去噪为何越修越抖 · TAPESTRY

用二阶有限差分测动作抖动，并用teacher forcing区分输入偏离与模型输出偏差。

50个验证动作块在低噪声时刻的预测抖动增大；t=99的均值0.284对GT0.166，单步t=999为0.152。调度器等控制支持作者诊断；视频频谱测的是像素，不是VAE latent。

[本篇星系](../tapestry.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tapestry.md) · [原文依据](https://arxiv.org/pdf/2610.36823v1)
