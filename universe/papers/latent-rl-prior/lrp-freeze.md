# 冻结decoder并保留本体条件路径 · Latent RL Prior

视觉适配不更新预训练动作decoder，以动作监督训练条件入口。

DINOv2-Small ViT-S/14编码多摄像头历史，视觉Q-Former产生context；梯度经冻结decoder回到视觉路径，冻结参数不等于切断梯度。

继续拆：[直接预测latent，不先猜物理状态](lrp-latent.md) · [显式桥接也只有动作监督](lrp-explicit.md) · [视觉小步更新，动作先验保持冻结](lrp-adaptation-rate.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
