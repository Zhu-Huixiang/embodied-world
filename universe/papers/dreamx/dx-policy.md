# 控制时预测code而非生成未来视频 · DreamX

当前画面和指令预测compact latent，单独Action DiT输出低层动作。

动作token可读取latent特征，反向读取关闭；人类视频监督latent，机器人示范另监督动作。视频迁移解码器与下游策略不要混为一次推理。

继续拆：[预训练与任务微调两笔成本](dx-policy-training.md) · [双臂YAM的14维绝对动作](dx-real-setup.md) · [小latent减少生成对象，但仍有推理成本](dx-latency.md) · [latent条件是否真被动作头用到](dx-policy-ablation.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
