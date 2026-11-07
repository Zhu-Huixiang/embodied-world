# CUDA图可逐位一致，编译版本另做闭环核对 · La-JEPA

减少启动开销与重编计算图不是同一执行变更。

原kernel CUDA graphs经36次replay/模型可逐位重现；编译后有小幅动作差。2000回合原管线闭环比较未发现显著差异，但不等于数学等价；模拟主结果eager、实机使用compiled。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
