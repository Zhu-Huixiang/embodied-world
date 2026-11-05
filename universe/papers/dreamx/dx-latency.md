# 小latent减少生成对象，但仍有推理成本 · DreamX

论文Table3每次调用1474ms对Mimic-Video28226ms。

原文给19.1倍比值，未定位两者测时硬件、采样步数和动作块执行配置；H200是训练硬件，不能移作推理测时条件。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
