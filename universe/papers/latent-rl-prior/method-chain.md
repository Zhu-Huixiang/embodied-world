# 本篇方法链路 · Latent RL Prior

先微调SimToolReal teacher并收集100000条成功程序化姿态对齐轨迹，将特权历史经state tokenizer/Q-Former压为任务context；flow-matching动作transformer通过cross-attention读context，通过AdaLN读本体历史与flow time。视觉阶段冻结decoder，只以动作flow loss训练DINOv2-Small与视觉Q-Former，直接生成latent而不需要特权/latent标签；双臂的两组queries共同自注意力协调后，分别结合各臂本体进入共享单臂decoder。

先微调SimToolReal teacher并收集100000条成功程序化姿态对齐轨迹，将特权历史经state tokenizer/Q-Former压为任务context；flow-matching动作transformer通过cross-attention读context，通过AdaLN读本体历史与flow time。视觉阶段冻结decoder，只以动作flow loss训练DINOv2-Small与视觉Q-Former，直接生成latent而不需要特权/latent标签；双臂的两组queries共同自注意力协调后，分别结合各臂本体进入共享单臂decoder。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/abs/2611.08458v1)
