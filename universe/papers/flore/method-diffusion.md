# 运动与力的联合扩散输出 · FLoRe

在条件观测下去噪得到运动关键点和每手力命令。

时间U-Net用FiLM接条件，DDPM训练、16步DDIM采样；H=50覆盖约1.67s，每任务单独policy。

[本篇星系](../flore.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/flore.md) · [原文依据](https://arxiv.org/html/2610.35862v1)
