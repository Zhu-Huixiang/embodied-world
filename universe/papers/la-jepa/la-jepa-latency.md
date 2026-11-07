# 一次策略调用快，不等于机器人控制频率 · La-JEPA

延迟覆盖文本编码、输入传输和动作回传，但不含机器人通信与模拟。

batch1、20次warmup后100次中位数、同一未给具体型号的consumer GPU；10步优化S17.78ms/B25.16ms/L59.72ms，Fast-WAM88.09ms/Faster-WAM50.96ms。输入分辨率、帧数与精度随原生实现不同，π0.5动作horizon另为10。

继续拆：[CUDA图可逐位一致，编译版本另做闭环核对](la-jepa-compile.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
