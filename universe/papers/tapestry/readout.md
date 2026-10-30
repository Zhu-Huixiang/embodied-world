# 复用视频输出层和转置读出 · TAPESTRY

动作读出使用预训练unembedding，再通过输入矩阵的转置回到动作空间。

动作接口新增参数只有64×20=1280；W、patch嵌入/输出与DiT共同微调，VAE和T5-XXL冻结。转置读出不是保证精确逆变换。

[本篇星系](../tapestry.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tapestry.md) · [原文依据](https://arxiv.org/pdf/2610.36823v1)
