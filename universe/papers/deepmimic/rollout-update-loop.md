# 从交互batch到网络更新 · DeepMimic

actor采动作收集转移，critic拟合λ-return，actor用优势更新。

每batch4096、minibatch256；这是在线模拟采样而非固定离线示范学习。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#6-训练)

继续拆：[PPO的有方向裁剪](ppo-clipped-surrogate.md) · [统一超参及本体步长](training-hyperparameters.md)。

[本篇星系](../deepmimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文依据](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf)
