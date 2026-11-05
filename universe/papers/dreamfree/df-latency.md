# H200单chunk计算成本 · DreamFree

分清模型推理延迟和机器人执行时间。

暖机后单H200含客户端预处理、服务端策略、后处理，排除通信和执行：91ms对DreamZero1632ms、pi0.5 81ms；各自部署配置且含编译、CUDAgraph、缓存优化。

继续拆：[积木任务完成时间估计](df-completion.md)。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
