# 适配观测并不要求目标也随之漂移 · La-JEPA

未来编码开销更大，目标是否适配需单独检验。

未来16帧是当前2帧的8倍编码token，最终观测在线编码、未来读预存特征。L模型用EMA适配未来目标81.65%对冻结目标82.26%（原管线、不同选中步数），未给出提升证据，故保留冻结目标。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
