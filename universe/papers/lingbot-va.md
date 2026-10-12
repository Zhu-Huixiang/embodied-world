# LingBot-VA 星系

Causal World Modeling for Robot Control

**导读** · 视频动作模型与视觉推理

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/lingbot-va.md) · [原文](https://www.roboticsproceedings.org/rss22/p016.html) · [评分卡](../../leaderboard/papers/lingbot-va/README.md)

因果视频VAE把观测压到48通道latent；Wan2.2-5B视频stream和动作stream经MoT联合处理，chunk间因果、chunk内并行。T5指令条件、真实obs/action写回KV cache、noisy-latent augmentation支持视频部分去噪后解动作；统一双臂30维动作，5.3B总参数。

## 技术挂点

- [世界动作联合建模](../concepts/wam.md)：把未来状态或视频与动作放进联合条件生成过程，让视觉动态和行动相互约束。

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

## 本篇行星与卫星

- [世界动作联合建模](lingbot-va/wam.md) · 初读挂点
- [变分自编码器 VAE](lingbot-va/vae.md) · 初读挂点
- [因果序列建模](lingbot-va/causal.md) · 初读挂点
- [闭环滚动与历史偏移](lingbot-va/rollout.md) · 初读挂点
- [本篇方法链路](lingbot-va/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
