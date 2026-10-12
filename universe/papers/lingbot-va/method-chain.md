# 本篇方法链路 · LingBot-VA

因果视频VAE把观测压到48通道latent；Wan2.2-5B视频stream和动作stream经MoT联合处理，chunk间因果、chunk内并行。T5指令条件、真实obs/action写回KV cache、noisy-latent augmentation支持视频部分去噪后解动作；统一双臂30维动作，5.3B总参数。

因果视频VAE把观测压到48通道latent；Wan2.2-5B视频stream和动作stream经MoT联合处理，chunk间因果、chunk内并行。T5指令条件、真实obs/action写回KV cache、noisy-latent augmentation支持视频部分去噪后解动作；统一双臂30维动作，5.3B总参数。

[本篇星系](../lingbot-va.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/lingbot-va.md) · [原文依据](https://www.roboticsproceedings.org/rss22/p016.html)
